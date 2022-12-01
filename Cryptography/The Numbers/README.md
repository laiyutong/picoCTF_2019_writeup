<h1>
The Numbers
</h1>
AUTHOR: DANNY<br>
POINTS: 100

<h2>Category</h2>
Cryptography

<h2>Problem Description</h2>
The <a href="https://github.com/laiyutong/picoCTF_2019_writeup/blob/main/Cryptography/The%20Numbers/the_numbers.png">numbers</a>... what do they mean?

<h2>Hints</h2>
The flag is in the format PICOCTF{}

<h2>Solution</h2>
The sequence of umbers in picture corresponds with the format PICOCTF{ <code>flag</code> }.<br>
Therefore, I observed the association between letters and numbers,<br>
and I realized the number is encrypted using a
<a href="https://en.wikipedia.org/wiki/Substitution_cipher">Substitution cipher</a>：
<a href="https://zh.wikipedia.org/wiki/A1Z26%E5%AF%86%E7%A2%BC">A1Z26 cipher</a> method.<br>
You will get the flag after decryption！


<img src="https://github.com/laiyutong/picoCTF_2019_writeup/blob/main/Cryptography/The%20Numbers/the_numbers.png" alt="the_numbers" width=50%>

<h2>Flag</h2>
<code>picoctf{thenumbersmason}</code>
