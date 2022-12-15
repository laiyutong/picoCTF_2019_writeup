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
<pre class="text">
                                     1 1 1 1 1 1 1 1 1 1 2 2 2 2 2 2 2 2 2 2 3 3 
           pos： 0 1 2 3 4 5 6 7 8 9 0 1 2 3 4 5 6 7 8 9 0 1 2 3 4 5 6 7 8 9 0 1   
(0,7,1)          j U 5 t _ a _ s
(8,15,1)                         1 m p l 3 _ a n 
(16,32,2)                                        4   r   m   4   u   1   b   8
(31,16,-2)                                         g   4   _   _   _   f   3   0
</pre>


<h2>Flag</h2>
<code>picoCTF{}</code>
