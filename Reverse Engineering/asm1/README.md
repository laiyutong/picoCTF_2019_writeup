<h1>asm1</h1>
AUTHOR: SANJAY C<br>
POINTS: 200

<h2>Category</h2>
Reverse Engineering

<h2>Problem Description</h2>
What does asm1(0x6fa) return?<br>
Submit the flag as a hexadecimal value (starting with '0x').<br>
NOTE: Your submission for this question will NOT be in the normal flag format.<br>
<a href="https://github.com/laiyutong/picoCTF_2019_writeup/blob/main/Reverse%20Engineering/asm1/test.S">Source</a>


<h2>Hints</h2>
assembly <a href="https://www.tutorialspoint.com/assembly_programming/assembly_conditions.htm">conditions</a>

<h2>Solution</h2>
<pre class="text">
Explain：
    DWORD PTR [] means "the size of the target operand is 32 bits"
    ESP is the current stack pointer.
    EBP is the base pointer for the current stack frame.<br>
    <img src="https://github.com/laiyutong/picoCTF_2019_writeup/blob/main/Reverse%20Engineering/asm1/EBP%26ESP.png" alt="EBP&ESP">
</pre>

<code>(0x6fa)</code> as a parameter is being put into the stack and located at <code>[ebp+0x8]</code> due to two lines below.<br>

<pre class="text">
line 2  <+0>:	push   ebp          //pushes asm1(0x6fa) into ebp
line 3  <+1>:	mov    ebp,esp      //the value(0x6fa) of ebp is moved into esp
</pre>

Jump to <code><asm1+37></code>(line 14) because the value <code>(0x6fa)</code> of [ebp+0x8] is greater than <code>0x3a2</code>.
<pre class="text">
line 4  <+3>:	cmp    DWORD PTR [ebp+0x8],0x3a2    //compare the value of [ebp+0x8] and 0x3a2
line 5  <+10>:	jg     0x512 <asm1+37>              //Jump if  the value of [ebp+0x8] Greater than 0x3a2
</pre>

<pre class="text">
line 14  <+37>:	cmp    DWORD PTR [ebp+0x8],0x6fa
line 15  <+44>:	jne    0x523 <asm1+54>
</pre>

<pre class="text">
line 16  <+46>:	mov    eax,DWORD PTR [ebp+0x8]
line 17  <+49>:	sub    eax,0x12
line 18  <+52>:	jmp    0x529 <asm1+60>
</pre>

<pre class="text">
line 21  <+60>:	pop    ebp
line 22  <+61>:	ret 
</pre>


<h2>Flag</h2>
<code>0x6e8</code>
