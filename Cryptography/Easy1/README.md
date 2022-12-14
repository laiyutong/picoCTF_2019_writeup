<h1>Easy1</h1>
AUTHOR: ALEX FULTON/DANNY<br>
POINTS: 100

<h2>Category</h2>
Cryptography

<h2>Problem Description</h2>
The one time pad can be cryptographically secure,but not when you know the key.<br>
Can you solve this?<br>
We've given you the encrypted flag, key, and a table to help <code>UFJKXQZQUNB</code> with the key of <code>SOLVECRYPTO</code>.<br>
Can you use this 
<a href="https://github.com/laiyutong/picoCTF_2019_writeup/blob/main/Cryptography/Easy1/table.txt">table</a> to solve it?

<h2>Hints</h2>
1.Submit your answer in our flag format.<br>
&ensp;For example, if your answer was 'hello', you would submit 'picoCTF{HELLO}' as the flag.<br>
2.Please use <code>all caps</code> for the message.


<h2>Solution</h2>
The <a href="https://github.com/laiyutong/picoCTF_2019_writeup/blob/main/Cryptography/Easy1/table.txt">table</a>
of <a href="https://en.wikipedia.org/wiki/Vigen%C3%A8re_cipher">Vigenère cipher</a>is used for encryption and decryption.<br>

The plaintext is the top row, corresponding to the key in the first column on the left,<br>
a ciphertext will be generated in the middle area.<br>

You can get the flag by using <a href="https://www.dcode.fr/vigenere-cipher">online tool</a>！

<h2>Flag</h2>
<code>picoCTF{CRYPTOISFUN}</code>
