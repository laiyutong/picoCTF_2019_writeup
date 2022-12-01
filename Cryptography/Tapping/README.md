<h1>Tapping</h1>
AUTHOR: DANNY<br>
POINTS: 200

<h2>Category</h2>
Cryptography

<h2>Problem Description</h2>
Theres tapping coming in from the wires.<br> 
What's it saying <code>nc jupiter.challenges.picoctf.org 21610</code>.<br>

<h2>Hints</h2>
1.What kind of encoding uses dashes and dots?<br>
2.The flag is in the format PICOCTF{}<br>

<h2>Solution</h2>
I used <code>Kali</code> to run <code>nc jupiter.challenges.picoctf.org 21610</code> when I saw the keyword <code>nc</code>.<br>

<a href="https://www.linuxfordevices.com/tutorials/netcat-command-in-linux">Netcat Command in Linux – A Complete Guide</a><br><br>
The result of picture as below seems like <a href="https://en.wikipedia.org/wiki/Morse_code">Morse Code</a>：<br>
<img src="https://github.com/laiyutong/picoCTF_2019_writeup/blob/main/Cryptography/Tapping/nc.PNG" alt="nc">

Find an <a href="http://www.unit-conversion.info/texttools/morse-code/">online tool</a> to put in the Morse code,<br>
or you can decrypt by yourself using the Morse code table.<br>
<img src="https://github.com/laiyutong/picoCTF_2019_writeup/blob/main/Cryptography/Tapping/Morse%20Code.jpg" alt="Morse" width="45%"><br>
You will get the flag！

<h2>Flag</h2>
<code>picoctf{m0rs3c0d31sfun3902019519}</code>

