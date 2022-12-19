<h1>shark on wire 1</h1>
AUTHOR: DANNY<br>
POINTS: 150

<h2>Category</h2>
Forensics

<h2>Problem Description</h2>
We found this <a href="https://github.com/laiyutong/picoCTF_2019_writeup/blob/main/Forensics/shark%20on%20wire%201/capture.pcap">packet capture</a>. Recover the flag.

<h2>Hints</h2>
1.Try using a tool like Wireshark.<br>
2.What are streams?

<h2>Solution</h2>
Since <a href="https://www.comparitech.com/net-admin/pcap-guide/">PCAP</a> files can be used to view TCP/IP and UDP network packets,<br>
using wireshark to open <a href="https://github.com/laiyutong/picoCTF_2019_writeup/blob/main/Forensics/shark%20on%20wire%201/capture.pcap">packet capture</a>.

<a href="https://www.wireshark.org/docs/wsug_html_chunked/ChAdvFollowStreamSection.html">streams</a>
<img src="https://github.com/laiyutong/picoCTF_2019_writeup/blob/main/Forensics/shark%20on%20wire%201/wireshark.png" alt="wireshark">

<h2>Flag</h2>
<code>picoCTF{StaT31355_636f6e6e}</code>
