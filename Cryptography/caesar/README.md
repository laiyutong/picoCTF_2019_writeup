<h1>caesar</h1>
AUTHOR: SANJAY C/DANIEL TUNITIS<br>
POINTS: 100

<h2>Category</h2>
Cryptography

<h2>Problem Description</h2>
Decrypt this <a href="https://github.com/laiyutong/picoCTF_2019_writeup/blob/main/Cryptography/caesar/ciphertext">message</a>.

<h2>Hints</h2>
caesar cipher <a href="https://privacycanada.net/classical-encryption/caesar-cipher/">tutorial</a>

<h2>Solution</h2>
You should know <a href="https://en.wikipedia.org/wiki/Caesar_cipher">Caesar cipher</a> before
decrypt <code>picoCTF{dspttjohuifsvcjdpoabrkttds}</code><br><br>

Simply put, all letters in the plaintext are shifted backwards (or forwards)<br>
by a fixed number in the alphabet and then replaced with ciphertext.<br><br>
The Caesar cipher is a very easy to break encryption method that can be cracked using <code>Brute-force attack</code>.

Here is an <a href="https://www.mymathtables.com/calculator/digital/caesar-cipher-encript-decript-converter.html">Online Cryptography Caesar Cipher Converter</a>.<br>
Paste the ciphertext to the bloack of <code>Enter Text</code> and you can get the flag(plaintext) in the block of <code>result</code>.

<h2>Flag</h2>
<code>picoCTF{crossingtherubiconzaqjsscr}</code>
