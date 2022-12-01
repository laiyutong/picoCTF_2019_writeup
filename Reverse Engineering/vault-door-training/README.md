<h1>vault-door-training</h1>
AUTHOR: MARK E. HAASE<br>
POINTS: 50

<h2>Category</h2>
Reverse Engineering

<h2>Problem Description</h2>
Your mission is to enter Dr. Evil's laboratory and retrieve the blueprints for his Doomsday Project.<br> 
The laboratory is protected by a series of locked vault doors.<br>
Each door is controlled by a computer and requires a password to open.<br> 
Unfortunately, our undercover agents have not been able to obtain the secret passwords for the vault doors,<br>
but one of our junior agents obtained the source code for each vault's computer!<br>
You will need to read the source code for each level to figure out what the password is for that vault door.<br>
As a warmup, we have created a replica vault in our training facility.<br>
The source code for the training vault is here: <a href="https://github.com/laiyutong/picoCTF_2019_writeup/blob/main/Reverse%20Engineering/vault-door-training/VaultDoorTraining.java">VaultDoorTraining.java

<h2>Hints</h2>
The password is revealed in the program's source code.

<h2>Solution</h2>
The flag can be found in the last paragraph of source code as long as you read the hint！<br><br>
The last paragraph of source code is as follows：<br>
<pre class="text">
<code>public boolean checkPassword(String password) {
        return password.equals("w4rm1ng_Up_w1tH_jAv4_eec0716b713");
}
</code></pre>
  
<h2>Flag</h2>
<code>picoCTF{w4rm1ng_Up_w1tH_jAv4_eec0716b713}</code>

