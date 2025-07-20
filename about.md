---
layout: page
title: "About Feed"
permalink: /about/
---

<style>
@import url('https://fonts.googleapis.com/css?family=Orbitron:wght@700&display=swap');
body .feed-about { font-family: 'Orbitron', monospace, Arial, sans-serif; }
.feed-glitch {
  position: relative;
  color: #ff003c;
  display: inline-block;
  font-size: 2.2rem;
  letter-spacing: 0.09em;
  font-family: 'Orbitron', monospace, Arial, sans-serif;
  text-shadow: 1px 0 10px #00fff7, -1px 0 10px #ff003c, 0 0 5px #00fff7;
  animation: feed-glitch 2.6s infinite linear alternate;
  text-transform: uppercase;
  z-index: 1;
  user-select: none;
}
.feed-glitch::before,
.feed-glitch::after {
  content: attr(data-glitch);
  position: absolute;
  left: 0;
  width: 100%;
  opacity: 0.6;
  pointer-events: none;
}
.feed-glitch::before {
  color: #00fff7;
  top: 2px;
  left: 2px;
  animation: feed-glitch-before 2.6s infinite linear alternate-reverse;
}
.feed-glitch::after {
  color: #ff003c;
  top: -2px;
  left: -2px;
  animation: feed-glitch-after 2.4s infinite linear alternate;
}

@keyframes feed-glitch {
  0% { text-shadow: 1px 0 8px #00fff7, -1px 0 8px #ff003c; }
  8% { text-shadow: 0 0 16px #00fff7, 0 0 12px #ff003c; }
  16% { text-shadow: 4px 2px 12px #00fff7, -4px -2px 16px #ff003c; }
  36% { text-shadow: 0 4px 24px #ff003c, 0 -2px 18px #00fff7; }
  60% { text-shadow: 1px 0 8px #00fff7, -1px 0 8px #ff003c; }
  80% { text-shadow: 0 0 0 #fff; }
  100% { text-shadow: 2px 0 16px #00fff7, -2px 0 16px #ff003c; }
}
@keyframes feed-glitch-before {
  0% { clip-path: inset(0 0 60% 0); }
  20% { clip-path: inset(60% 0 0 0); }
  40% { clip-path: inset(0 30% 40% 0); }
  60% { clip-path: inset(40% 0 0 30%); }
  80% { clip-path: inset(0 60% 0 0); }
  100% { clip-path: inset(0 0 50% 0); }
}
@keyframes feed-glitch-after {
  0% { clip-path: inset(60% 0 0 0); }
  20% { clip-path: inset(0 0 60% 0); }
  40% { clip-path: inset(0 0 40% 30%); }
  60% { clip-path: inset(30% 40% 0 0); }
  80% { clip-path: inset(0 0 60% 0); }
  100% { clip-path: inset(50% 0 0 0); }
}

.feed-flicker {
  animation: feed-flicker 1s infinite alternate;
  color: #fff700;
  background: rgba(13,11,31,0.66);
  padding: 0.2em 0.5em;
  border-radius: 5px;
  font-size: 1.22em;
  font-family: monospace;
}
@keyframes feed-flicker {
  0%, 100% { opacity: 0.85; filter: blur(0.5px); }
  10% { opacity: 0.3; filter: blur(1.5px); }
  20% { opacity: 1; filter: blur(0.3px); }
  50% { opacity: 0.66; filter: blur(1.2px); }
  80% { opacity: 1; }
}

.feed-encrypt {
  font-family: 'Fira Mono', monospace;
  color: #00fff7;
  background: #191430;
  border-radius: 3px;
  padding: 0.6em 0.8em;
  margin: 1.5em 0;
  letter-spacing: 0.14em;
  font-size: 0.98em;
  word-break: break-all;
  filter: blur(0.6px);
  opacity: 0.82;
  animation: encrypt-flash 3.2s infinite alternate;
}
@keyframes encrypt-flash {
  0%,100% { filter: blur(0.7px); opacity: 0.82;}
  40% { filter: blur(2.7px); opacity: 0.5;}
  80% { filter: blur(0.2px); opacity: 1;}
}

.feed-bio {
  font-family: 'Orbitron', Arial, monospace;
  color: #fff;
  margin-top: 2em;
  margin-bottom: 1em;
  font-size: 1.2em;
  letter-spacing: 0.06em;
  line-height: 1.7;
  text-shadow: 0 0 10px #00fff7;
}

.feed-odd {
  color: #ff2ffb;
  font-family: 'Fira Mono', monospace;
  font-size: 1.12em;
  background: linear-gradient(90deg, #0d0b1f 90%, #ff003c 100%);
  border-radius: 9px;
  padding: 0.6em 1.1em;
  margin: 1.4em 0;
  letter-spacing: 0.22em;
  text-shadow: 0 0 12px #ff003c;
  animation: feed-oddglitch 2.2s infinite alternate;
}
@keyframes feed-oddglitch {
  0%,100% { opacity: 1; }
  9% { opacity: 0.3; }
  33% { opacity: 0.7; }
  55% { opacity: 0.53; }
}

.feed-ascii {
  font-family: monospace;
  font-size: 1em;
  color: #fff700;
  background: #0d0b1f;
  padding: 0.7em 0.6em 0.6em 0.6em;
  border-radius: 6px;
  box-shadow: 0 0 10px #ff003c;
  margin: 2em 0;
  letter-spacing: 0.11em;
  animation: ascii-flicker 1.5s infinite alternate;
}
@keyframes ascii-flicker {
  0%,100% { opacity: 0.87; }
  10% { opacity: 0.47; }
  66% { opacity: 1; }
}
</style>

<div class="feed-about">

<span class="feed-glitch" data-glitch="F̸̤͈̏̈́E̷͎͗͒Ę̴̩͗D̴̦̍">F̸̤͈̏̈́E̷͎͗͒Ę̴̩͗D̴̦̍</span>
<br>
<span class="feed-flicker">&lt;Night City Persona File&gt;</span>

<div class="feed-encrypt">
01101001 01100100 01100101 01101110 01110100 01101001 01110100 01111001 <br>
01001101 01100101 00111010 00100000 01010011 01111001 01101110 01110100 01101000 01000101 01110100 01101001 01100011 01001011 01100001 01101100 01100101 01101001 01100100<br>
<span style="color:#ff003c;">//ACCESS RESTRICTED//</span>
</div>

<div class="feed-bio">
<span class="feed-flicker">Who is Feed?</span>
<br>
<span style="color:#ff003c;">&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;</span>
<span style="color:#fff700;">Nobody. Everybody.</span>
<br><br>
<span class="feed-odd">[Online, I am: <span style="color:#00fff7;">a datastream, a glitch, a meme with a pulse.</span>]</span>
<br>
<span class="feed-odd">[Offline, I am: <span style="color:#ff2ffb;">an apparition in layers, face half-lost behind tangled hair and a biohaz mask that reads: "DO NOT FEED".</span>]</span>
<br>
<span style="color:#00fff7;">My voice is scrambled. My feeds are filtered. My shadow is encrypted. No one meets Feed—only the mask, only the stream.</span>
</div>

<div class="feed-encrypt">
<span style="letter-spacing:0.33em;">
{▒▒▒▒▒▒▒▒▒▒▒▒▒▒▒▒▒▒▒▒▒▒▒▒▒▒▒▒▒▒▒▒▒▒▒▒▒▒▒▒▒▒▒▒▒▒▒▒▒▒▒▒▒▒▒▒▒▒▒▒▒▒▒▒▒▒▒▒▒▒▒▒▒▒▒▒▒▒▒▒▒▒▒▒▒▒▒▒▒▒▒▒▒▒▒▒▒▒▒▒▒▒▒▒▒▒▒▒▒▒▒▒}<br>
<span style="color:#fff700;">ERROR: RealNameNotFoundException</span>
<br>
{▒▒▒▒▒▒▒▒▒▒▒▒▒▒▒▒▒▒▒▒▒▒▒▒▒▒▒▒▒▒▒▒▒▒▒▒▒▒▒▒▒▒▒▒▒▒▒▒▒▒▒▒▒▒▒▒▒▒▒▒▒▒▒▒▒▒▒▒▒▒▒▒▒▒▒▒▒▒▒▒▒▒▒▒▒▒▒▒▒▒▒▒▒▒▒▒▒▒▒▒▒▒▒▒▒▒▒}
</span>
</div>

<div class="feed-flicker" style="margin-top: 2.5em;">
<span style="color:#ff003c;">You want a face, a name, a story?</span>
<br>
<span style="color:#00fff7;">You get a signal, a tag, a transmission.</span>
<br>
<span style="color:#fff700;">This is all you get.</span>
</div>

<div class="feed-ascii">
<pre>
   .-._   _ _ _ _ _ _ _ _
.-''-.__.-'00  '-' ' ' ' ' ' '  ' '-.
/--.--,--/--/--/--/--/--/--/--/--/--/
/--.--,--/--/--/--/--/--/--/--/--/--/
`--'--'  `--'  `--'  `--'  `--'  `--'
</pre>
</div>

<div class="feed-odd">
<span style="color:#fff700;">"Feed"</span> is a persona, a process, a packet.<br>
I am <span style="color:#00fff7;text-shadow:0 0 18px #00fff7;">not</span> a person.<br>
Or maybe I am.<br>
Does it matter?
</div>

<div class="feed-encrypt" style="font-size:1.1em;">
<span style="color:#ff003c;">[TRANSMISSION ENDS]</span><br>
01000110 01100101 01100101 01100100 00100000 01110111 01100001 01110011 00100000 01101000 01100101 01110010 01100101<br>
<span style="color:#00fff7;">You never saw me.</span>
</div>

</div>
