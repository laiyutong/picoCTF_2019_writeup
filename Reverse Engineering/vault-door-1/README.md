<h1>vault-door-1</h1>
AUTHOR: MARK E. HAASE<br>
POINTS: 100

<h2>Category</h2>
Reverse Engineering

<h2>Problem Description</h2>
This vault uses some complicated arrays!<br>
I hope you can make sense of it, special agent.<br>
The source code for this vault is here: <a href="https://github.com/laiyutong/picoCTF_2019_writeup/blob/main/Reverse%20Engineering/vault-door-1/VaultDoor1.java">VaultDoor1.java

<h2>Hints</h2>
Look up the charAt() method online.

<h2>Solution</h2>
About charAt() method：<a href="https://www.geeksforgeeks.org/java-string-charat-method-example/">Java String charAt() method with example</a><br>
In brief, you can get the flag by sorting the index of charAt() method.<br><br>

Using the python script as below to get the flag！
<pre class="text">
<code>password = [None] *32          
<br>         
password[0]  = 'd'  
password[29] = '3'  
password[4]  = 'r'  
password[2]  = '5'  
password[23] = 'r'  
password[3]  = 'c'  
password[17] = '4'  
password[1]  = '3'  
password[7]  = 'b'  
password[10] = '_'  
password[5]  = '4'  
password[9]  = '3'  
password[11] = 't'  
password[15] = 'c'  
password[8]  = 'l'  
password[12] = 'H'  
password[20] = 'c'  
password[14] = '_'  
password[6]  = 'm'  
password[24] = '5'  
password[18] = 'r'  
password[13] = '3'  
password[19] = '4'  
password[21] = 'T'  
password[16] = 'H'  
password[27] = 'f'  
password[30] = 'b'  
password[25] = '_'  
password[22] = '3'  
password[28] = '6'  
password[26] = 'f'  
password[31] = '0'
<br>
print("picoCTF{{{}}}".format(''.join(password)))</code>
</pre>
online practice：<a href="https://replit.com/languages/python3">replit</a>

<h2>Flag</h2>
<code>picoCTF{ca1cu1at1ng_Mach1n3s_477ce}</code>
