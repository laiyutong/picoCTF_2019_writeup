<h1>vault-door-3</h1>
AUTHOR: MARK E. HAASE<br>
POINTS: 200

<h2>Category</h2>
Reverse Engineering

<h2>Problem Description</h2>
This vault uses for-loops and byte arrays.<br>
The source code for this vault is here: <a href="https://github.com/laiyutong/picoCTF_2019_writeup/blob/main/Reverse%20Engineering/vault-door-3/VaultDoor3.java">VaultDoor3.java</a>

<h2>Hints</h2>
Make a table that contains each value of the loop variables and the corresponding buffer index that it writes to.

<h2>Solution</h2>
The string <code>jU5t_a_sna_3lpm18gb41_u_4_mfr340</code> is given by the <code>checkPassword()</code> in <a href="https://github.com/laiyutong/picoCTF_2019_writeup/blob/main/Reverse%20Engineering/vault-door-3/VaultDoor3.java">VaultDoor3.java</a><br>
Accordingly, we need to reverse engineer <code>jU5t_a_sna_3lpm18gb41_u_4_mfr340</code>.<br><br>
Writing a python script and using <code>jU5t_a_sna_3lpm18gb41_u_4_mfr340</code> as input to reverse as shown below.<br>
<pre class="text">
def checkPassword(password):
    if (len(password) != 32):
        return False
    buffer = [""]*32
    print(buffer)
    for i in range(8):
        buffer[i] = password[i]
    for i in range(8, 16):
        buffer[i] = password[23-i]
    for i in range(16, 32, 2):
        buffer[i] = password[46-i]
    for i in range(31, 16, -2):
        buffer[i] = password[i] 
    print(''.join(buffer))
checkPassword("jU5t_a_sna_3lpm18gb41_u_4_mfr340")
</pre>

<pre class="text">
                                     1 1 1 1 1 1 1 1 1 1 2 2 2 2 2 2 2 2 2 2 3 3 
           pos： 0 1 2 3 4 5 6 7 8 9 0 1 2 3 4 5 6 7 8 9 0 1 2 3 4 5 6 7 8 9 0 1   
(0,7,1)          j U 5 t _ a _ s
(8,15,1)                         1 m p l 3 _ a n 
(16,32,2)                                        4   r   m   4   u   1   b   8
(31,16,-2)                                         g   4   _   _   _   f   3   0
</pre>
You can get the flag by sorting the string！

<h2>Flag</h2>
<code>picoCTF{jU5t_a_s1mpl3_an4gr4m_4_u_1fb380}</code>
