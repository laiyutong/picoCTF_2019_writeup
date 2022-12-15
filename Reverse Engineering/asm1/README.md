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
    ESP is the current stack pointer.
    EBP is the base pointer for the current stack frame.<br>
    <img src="https://github.com/laiyutong/picoCTF_2019_writeup/blob/main/Reverse%20Engineering/asm1/EBP%26ESP.png" alt="EBP&ESP">
    DWORD PTR [] means "the size of the target operand is 32 bits"
</pre>

<code>(0x6fa)</code> as a parameter is being put into the stack and located at <code>[ebp+0x8]</code> due to two lines below.<br>

<pre class="text">
<+0>:	push   ebp          //pushes asm1(0x6fa) into ebp
<+1>:	mov    ebp,esp      //the value(0x6fa) of ebp is moved into esp
</pre>

<pre class="text">
<+3>:	cmp    DWORD PTR [ebp+0x8],0x3a2
<+10>:	jg     0x512 <asm1+37>
</pre>

<pre class="text">
<+37>:	cmp    DWORD PTR [ebp+0x8],0x6fa
<+44>:	jne    0x523 <asm1+54>
</pre>

<pre class="text">
<+46>:	mov    eax,DWORD PTR [ebp+0x8]
<+49>:	sub    eax,0x12
<+52>:	jmp    0x529 <asm1+60>
</pre>

<pre class="text">
<+60>:	pop    ebp
<+61>:	ret 
</pre>


<h2>Flag</h2>
<code>0x6e8</code>
