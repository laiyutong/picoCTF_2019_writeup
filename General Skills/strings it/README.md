<h1>strings it</h1>
AUTHOR: SANJAY C/DANNY TUNITIS<br>
POINTS: 100

<h2>Category</h2>
General Skills

<h2>Problem Description</h2>
Can you find the flag in <a href="https://github.com/laiyutong/picoCTF_2019_writeup/blob/main/General%20Skills/strings%20it/strings">file</a> without running it?

<h2>Hints</h2>
<a href="https://linux.die.net/man/1/strings">strings</a>

<h2>Solution</h2>
<code>strings</code> looks for a printable string in an object file or binary.<br>
The output results of <code>strings</code> are very large,<br> 
so I used <code>grep</code> to find the keyword I need and I got the flag！.
<img src="https://github.com/laiyutong/picoCTF_2019_writeup/blob/main/General%20Skills/strings%20it/strings.png" alt="strings">

<h2>Flag</h2>
<code>picoCTF{5tRIng5_1T_827aee91}</code>
