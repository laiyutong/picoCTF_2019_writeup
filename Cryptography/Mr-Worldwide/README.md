<h1>Mr-Worldwide</h1>
AUTHOR: DANNY<br>
POINTS: 200

<h2>Category</h2>
Cryptography

<h2>Problem Description</h2>
A musician left us a <a href="https://github.com/laiyutong/picoCTF_2019_writeup/blob/main/Cryptography/Mr-Worldwide/message.txt">message</a>. What's it mean?
<pre text="des">picoCTF{(35.028309, 135.753082)(46.469391, 30.740883)(39.758949, -84.191605)(41.015137, 28.979530)(24.466667, 54.366669)(3.140853, 101.693207)_(9.005401, 38.763611)(-3.989038, -79.203560)(52.377956, 4.897070)(41.085651, -73.858467)(57.790001, -152.407227)(31.205753, 29.924526)}</pre>

<h2>Hints</h2>
(None)

<h2>Solution</h2>
Message looks like the longitude and latitude, so search it in <code>Google Map</code> and note the <code>first letter</code> of the location.<br>
Put all the letters together and you can get flag！<br><br>
<pre class="text">
"K"yoto, Japan                      (35.028309, 135.753082)
"O"dessa, Ukraine                   (46.469391, 30.740883)
"D"ayton, United States             (39.758949, -84.191605)
"I"stanbul, Turkey                  (41.015137, 28.979530)
"A"bu Dhabi, United Arab Emirates   (24.466667, 54.366669)
"K"uala Lumpur, Malaysia            (3.140853, 101.693207)
----------------------------------------------------------
"A"ddis Ababa, Ethiophia            (9.005401, 38.763611)
"L"oja, Ecuador                     (-3.989038, -79.203560)
"A"msterdam, Netherlands            (52.377956, 4.897070)
"S"leepy Hollow, United States      (41.085651, -73.858467)
"K"odiak, United States             (57.790001, -152.407227)
"A"lexandria, Egypt                 (31.205753, 29.924526)
</pre>

<h2>Flag</h2>
<code>picoCTF{KODIAK_ALASKA}</code>

