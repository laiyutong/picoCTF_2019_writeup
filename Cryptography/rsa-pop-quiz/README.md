<h1>rsa-pop-quiz</h1>
AUTHOR: WPARKS/NMONTIERTH<br>
POINTS: 200

<h2>Category</h2>
Cryptography

<h2>Problem Description</h2>
Class, take your seats!<br>
It's PRIME-time for a quiz... <code>nc jupiter.challenges.picoctf.org 58617</code>

<h2>Hints</h2>
<a href="https://simple.wikipedia.org/wiki/RSA_algorithm">RSA info

<h2>Solution</h2>
You need to answer several questions about RSA.<br><br>
1. Yes； n = q * p
<pre class="text">
#### NEW PROBLEM ####
q : 60413
p : 76753
##### PRODUCE THE FOLLOWING ####
n
IS THIS POSSIBLE and FEASIBLE? (Y/N):Y
#### TIME TO SHOW ME WHAT YOU GOT! ###
n: 4636878989
Outstanding move!!!
</pre>
2. Yes； q = n / p
<pre class="text">
#### NEW PROBLEM ####
p : 54269
n : 5051846941
##### PRODUCE THE FOLLOWING ####
q
IS THIS POSSIBLE and FEASIBLE? (Y/N):Y
#### TIME TO SHOW ME WHAT YOU GOT! ###
q: 93089          
Outstanding move!!!
</pre>
3. No；We know toitent(n) = (p-1) * (q-1) but we don't have the toitent.
<pre class="text">
#### NEW PROBLEM ####
e : 3
n : 12738162802910546503821920886905393316386362759567480839428456525224226445173031635306683726182522494910808518920409019414034814409330094245825749680913204566832337704700165993198897029795786969124232138869784626202501366135975223827287812326250577148625360887698930625504334325804587329905617936581116392784684334664204309771430814449606147221349888320403451637882447709796221706470239625292297988766493746209684880843111138170600039888112404411310974758532603998608057008811836384597579147244737606088756299939654265086899096359070667266167754944587948695842171915048619846282873769413489072243477764350071787327913
##### PRODUCE THE FOLLOWING ####
q
p
IS THIS POSSIBLE and FEASIBLE? (Y/N):N
Outstanding move!!!
</pre>

<pre class="text">
</pre>

<pre class="text">
</pre>

<pre class="text">
</pre>

<pre class="text">
</pre>

<pre class="text">
</pre>

<pre class="text">
</pre>
  
<h2>Flag</h2>
<code>picoCTF{}</code>
