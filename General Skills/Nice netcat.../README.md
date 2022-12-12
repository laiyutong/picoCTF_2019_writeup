<h1>Nice netcat...</h1>
AUTHOR: SYREAL<br>
POINTS: 15

<h2>Category</h2>
General Skills

<h2>Problem Description</h2>
There is a nice program that you can talk to by using this command in a shell:<br>
<code>$ nc mercury.picoctf.net 21135</code>, but it doesn't speak English...

<h2>Hints</h2>
1.You can practice using netcat with this picoGym problem: <a href="https://play.picoctf.org/practice/challenge/34">what's a netcat?</a><br>
2.You can practice reading and writing ASCII with this picoGym problem: <a href="https://play.picoctf.org/practice/challenge/22">Let's Warm Up</a>

<h2>Solution</h2>
After executing <code>nc mercury.picoctf.net 21135</code> in linux,
you will find that the output is all numbers.<br>
<img src="https://i.imgur.com/WfQoXAX.png" alt="ncoutput">
Because it may be related to ASCII, write a python shell to convert numbers to letters.<br>
<img src="https://i.imgur.com/1pe3Zwc.png" alt="change.py" width="27%">
Take the output of <code>nc mercury.picoctf.net 21135</code> as the input of pyhton shell and execute it,<br> and you will get the flag！<br>
<img src="https://i.imgur.com/2WvKATD.png" alt="sol">

<h2>Flag</h2>
<code>picoCTF{g00d_k1tty!_n1c3_k1tty!_afd5fda4}</code>
