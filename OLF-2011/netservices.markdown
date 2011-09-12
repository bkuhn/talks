% With Software As a Service,<br/> Is Only the Network Luddite Free?
% Bradley M. Kuhn
% Saturday 10 September 2011

# In The Beginning ...

<img align=right src="pdp-10.jpg" />

+ There was a computer.

+ There were terminals.

+ There were users.

+ ... and the users had freedom.

# Ye Ol' Four Freedoms

+ to use.

+ to learn and modify for yourself.

+ to copy and share.

+ to modify and share modified versions.

# &hellip; Then Freedom Eluded Us

+ They built licensing walls.

+ By separating the software from the computer.

<img align=right src="berlin-wall-build.jpg" />
</center>

+ Who Invented Licensing?

# Who Invented Licensing?
<br/>
Some think he did:
<br/>
<img src="bill-gates-arrest.jpg" align="left"  />
<p>As the majority of hobbyists must be aware, most of you steal your software. &hellip; [If] software is something to share &hellip; You prevent good software from being written.</p>

<br clear="all"/>

+ Gates convinces IBM to license rather then acquire DOS.

# Who Fixed this Problem?

# Who Fixed this Problem?

<center>
<br/>
<br/>
<img src="rms-current.jpg"  />
</center>

# RMS

<img align=right src="rms-book-cover.jpg"  />

+ Job at MIT's AI lab in late 1970s and early 1980s.

+ Programming their PDP-10!

+ In the Golden Age.

# MIT AI Lab: The Golden Age

<img src="pdp-10-2.jpg" align="right"  />

 - academic computing.
 - software sharing.
 - no licenses!

# MIT AI Lab

<img src="ai-lab-tear-down.jpg" align="right"  />

MIT changed.

# MIT AI Lab

<cite>patents == $$$</cite>

# MIT AI Lab

<cite>spin-offs == $$$</cite>

# GNU

<img src="gnu-hacker.jpg" align="right"/>

+ Changes the world.

+ For the user of individual computers.

+ No reason now not to have freedom on your own machine.

# Internet changes little (to start)

+ Client/Server computing.

+ Freedom implications are basically the same.

+ Example: The Email System.

# Email: The MTA

+ Yours has freedom: (postfix, exim, sendmail).

+ Plenty of proprietary ones: (exchange).

+ RFCs define interoperability.

+ We protocol-analyze &amp; reimplement RFC-less protocols: (OpenChange).

# Email: The MUA

+ Yours has freedom: (Thunderbird, mutt, Gnus)

+ Plenty of proprietary ones: (outlook)

# The Great Fear: SaaS

+ SaaS: Software as a Service

+ True &ldquo;SaaS&rdquo; would end software freedom.

+ Imagine: GCC as an network service.

+ SaaS == your private computing done elsewhere.

+ Copyleft proponents all feared this threat.

# A New Era of Computing?

Anyone know what this is?

<img src="cloud-unicode.png" width="773" height="339" align="center" />

&#x2601;

# New Era: Cloud Computing?

<img src="cloud-unicode.png" width="580" height="254" align="center" />

+ Unicode Character 'CLOUD' (U+2601)
+ Given what this looks like &hellip;
     + &hellip; Unicode committee was omniscient.

<style type="text/css">
.medium {
 font-size: 90pt
 }
</style>
<p align="center">
<span class="medium">&#x2601;</span>
</p>

# Cloud Computing: What changed?

+ The Browser as application delivery platform.

+ AJAX.

+ Whose computing is done where?

+ Cloud Computing: more complicated than SaaS.

+ Interesting applications are collaboration.

# Email becomes Gmail

+ "The experience"

+ Effectively: Thin Client.

+ Mixes Up Free again: Price vs. Freedom.

+ RFCs no longer enough.

+ We're back to proprietary "lock-in".

# Talk about Obfuscated!
<span class="fitonslide">
<pre>
try{function e(b){throw b;}var i=void 0,k=null;
function aa(){return function(b){return b}}
function m(){return function(){}}
function ba(b){return function(a){this[b]=a}}
function o(b){ return function(){return this[b]}}
function p(b){return function(){return b}}var q;
function da(b,a,c){b=b.split(".");c=c||ea;
!(b[0]in c)&&c.execScript&&c.execScript("var "+b[0]);
for(var d;b.length&&(d=b.shift());)
!b.length&&s(a)?c[d]=a:c=c[d]?c[d]:c[d]={}}
function fa(b,a){for(var c=b.split("."),d=a||ea,f;f=c.shift();)
if(t(d[f]))d=d[f];else return k;return d}function u(){}
function ga(b){b.va=function $(){return b.xY||(b.xY=new b)}}
function ia(b){var a=typeof b;if(a=="object")if(b){
if(b instanceof Array)return"array";else if(b instanceof Object)return a;
var c=Object.prototype.toString.call(b);if(c=="[object Window]")
return"object";if(c=="[object Array]"||typeof b.length=="number"&&
typeof b.splice!="undefined"&&typeof b.propertyIsEnumerable!="undefined"
&&!b.propertyIsEnumerable("splice"))return"array";
if(c=="[object Function]"||typeof b.call!="undefined"&&
typeof b.propertyIsEnumerable!="undefined"&&!b.propertyIsEnumerable("call"))
return"function"}else return"null";
else if(a=="function"&&typeof b.call=="undefined")return"object";return a}function s(b){return b!==i}function ja(b){return b===k}function t(b){return b!=k}function ka(b){return ia(b)=="array"}function la(b){var a=ia(b);return a=="array"||a=="object"&&typeof b.length=="number"}function ma(b){return typeof b=="string"}function na(b){return typeof b=="boolean"}function oa(b){return typeof b=="number"}function pa(b){return ia(b)=="function"}
</pre>

# The Javascript Problem

  + Microsoft **gets** this:
       + the platform for future of proprietariness &hellip;
       + &hellip; is already on your computer.

  + You might run a software freedom operating system &hellip;
       + &hellip; but how much proprietary runs in your browser?
       + Effectively, &ldquo;Compressed&rdquo; Javascript is a proprietary binary.

***

> JavaScript is an assembly language. JavaScript + HTML is like a .NET assembly. The browser can execute it, but no human should care what's there.

<span class="fitonslide">
<p align=right>
 &mdash; Erik Meijer of Microsoft on 5 July 2011.
</p>
</span>

# Users and &ldquo;The Cloud&rdquo;

<center>
<img src="cloud-bad.jpg"  />
</center>

# Users and &ldquo;The Cloud&rdquo;

<center>
<img src="cloud-symptoms-with-apps.jpg"  />
</center>

<p>Even *Worse* Than Proprietary Apps and OS'es</p>

# The Bigger Challenge

+ Not merely a question of code and licensing.

+ A question of community source+data control.

+ Power to transport: applications, data, human connections.

+ Autonomy: of code, of data, of community.

# How Do We Start?

<img src="cloud-bad-with-bird-on-left.jpg" align="right"/>

+ Infrastructure that respects freedom.

+ Empower the user: give them **all** the code.

+ Link to your Javascript source repository.

+ Explain what code runs on server &amp;  **share that code**.

# New Code's Needed, Too

+ User communities need ability to transplant.

+ Reclaim your data; relocate your community.

+ Truly distributed data.

+ This programming is  **tough**.

# Projects to Look At

+ Run NoScript plugin to at least see what proprietary Javascript you're getting.

+ status.net / identi.ca
     + DTRT in this regard for Microblogging
     + Follow me there: 'bkuhn'
     + Losing Free Software Community lately to Google Plus

+ MediaGoblin (replaces Flickr &amp; Picasso) 

+ Jesse Vincent's Prophet, CouchDB, and other truly decentralized data stores.

# License To Look At

+ GPL is the BSD of Network Service.

+ Affero GPL.

+ Extends copyleft to network service world.

+ Handles the code side well.

+ Very few applications use AGPL, though!

# Techniques to Look At

+ Deployed applications auto-give users source.

+ Data is downloadable in community-chunks.

# "Future" of the Cloud

<img width=433 height=388 src="cloud-disappear.jpg" align="right"/>

+ Disjoint but Integrated.

+ Portable and Autonomous.

+ Developers will decide next direction.

+ Ask **the** question in Cloud projects:
      + Are we respecting the users' freedom and autonomy?

+ The data is theirs; we are *their* custodians.

# More Info and This Talk's License

+ More Info: 
    + http://gnu.org/philosophy/who-does-that-server-really-serve.html
    + Oggcast: faif.us ; Blog: ebb.org/bkuhn/blog 
    + identi.ca: @bkuhn

<p>Presentation &amp; slides: Copyright &copy; 2008&mdash;2011 Bradley M. Kuhn.  License: <a href="http://creativecommons.org/licenses/by-sa/3.0/us">Creative Commons Attribution-Share Alike (CC-By-SA) 3.0 United States License</a>. <img src="cc-by-sa-3-0_88x31.png"/></p>

<p>Some images included herein are &copy;'ed by others. I believe my use of those images is fair use under USA &copy; law.  However, I suggest you remove such images if you redistribute these slides under CC-By-SA.
</p>
