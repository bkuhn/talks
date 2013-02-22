% Affero GPLv3: Why It Exists &amp; Who It's For?
% Bradley M. Kuhn
% Saturday 23 February 2013

# A Brief History of Affero GPL

+ Imagine the turn of the century.

+ The so-called Application Service Provider loophole.

+ In early 2001, someone said to me at an event:
         - &ldquo;I won't release my web application code at all, because the GPL is the BSD license of the web.&rdquo;

# Was this a loophole?

+ Well, it wasn't *really* a loophole

+ GPLv2 didn't (couldn't?) foresee web applications.
      + client/server barely existed when it was written.

+ Copyleft's copyright hack centered around distribution.

# The Catalyst

<img src="henry-poole.jpg" align="right"  />

+ Henry (sometimes Henri) Poole forms Allseer.
       + Which becomes Affero.

+ Web service company to encourage non-profit donations.

+ Henry points out: we have no copyleft.

# Public Performance?

+ Is it defined for software?

+ If it were, would it be enough of a copyleft hack?

+ I've long supported it as an &ldquo;at worst, a no-op&rdquo; addition.
      + I've been unable to persuade anyone else.

# Affero Idea: Inspiration

<img src="ouroboros.png" align="right"  />

+ The classic Computer Science ouroboros:

+ The program that prints its own source

+ Sometimes called &ldquo;quine&rdquo;

# Affero Idea: Inspiration

<p>GPLv2&sect;2(c):</p>

<span class="fitonslide">

<p>If the modified program normally reads commands interactively when run,
    you must cause it, when started running for such interactive use in
    the most ordinary way, to print or display an announcement including
    an appropriate copyright notice and a notice that there is no warranty
    (or else, saying that you provide a warranty) and that users may
    redistribute the program under these conditions, and telling the user
    how to view a copy of this License.  (Exception: if the Program itself
    is interactive but does not normally print such an announcement, your
    work based on the Program is not required to print an announcement.)
</p>

</span>

# Merging the Two

+ Precedent has thus been set:
      - GPL can require a &ldquo;feature preservation for freedom&rdquo;

+ mid 2002-09: I suggest a print-your-own-source feature for GPLv2.2&sect;2(d).

+ Lawyers draft, ditching the CS-y focus of print-your-own-source:
     + &ldquo;download my CCS now&rdquo; feature preservation instead.

+ Henry is excited.

+ Affero GPL v1 is born.

# Affero GPL v1 is Born

<p>AGPLv1&sect;2(d)</p>

<span class="fitonslide">

<p>If the Program as you received it is intended to interact with users
through a computer network and if, in the version you received, any user
interacting with the Program was given the opportunity to request
transmission to that user of the Program's complete source code, you must
not remove that facility from your modified version of the Program or work
based on the Program, and must offer an equivalent opportunity for all
users interacting with your Program through a computer network to request
immediate transmission by HTTP of the complete source code of your
modified version or other derivative work.</p>

</span>

# The Great Stallman Stalling, 2002-2006

+ RMS agrees to make:
     - AGPLv1&sect;2(d) == GPL v2.2&sect;2(d)

+ For various (mostly bad) reasons, GPLv2.2 is never released.
    - Yes, I have a copy if you really want one.

+ Affero, Inc. (the company) goes bankrupt.

+ For various (mostly bad) reasons, the &ldquo;FSF team&rdquo; forks &hellip;
      + &hellip; and I fall into (victim to?) a long distraction.

+ GPLv3 process begins.

# Wait, What?!?!

+ By the time I realize what had happened &hellip;
      + &hellip; Affero clause isn't in GPLv3 drafts!

+ Henry, fortunately, insists on license upgrade for AGPLv1.

+ AGPLv3 is born.
    + But not released until 19 November 2007
    + Fontana writes AGPLv2 (transitional).

# Affero Clause: Current

AGPLv3&sect;13

<span class="fitonslide">

<p>Notwithstanding any other provision of this License, if you modify the
Program, your modified version must prominently offer all users
interacting with it remotely through a computer network (if your version
supports such interaction) an opportunity to receive the Corresponding
Source of your version by providing access to the Corresponding Source
from a network server at no charge, through some standard or customary
means of facilitating copying of software.  This Corresponding Source
shall include the Corresponding Source for any work covered by version 3
of the GNU General Public License that is incorporated pursuant to the
following paragraph.</p>

<p>Notwithstanding any other provision of this License, you have
permission to link or combine any covered work with a work licensed
under version 3 of the GNU General Public License into a single
combined work, and to convey the resulting work.  The terms of this
License will continue to apply to the part which is the covered work,
but the work with which it is combined will remain governed by version
3 of the GNU General Public License.</p>

</span>

# The Affero Clause

<img src="jfk-bay-of-pigs.jpg" align="right"  />

<p>There's an old saying that victory has a hundred fathers and defeat is an orphan.</p>

<span class="fitonslide">
<p align=right>
 &mdash; John F. Kennedy
</p>
</span>

# What happened in the meantime?

+ The rise of:
       + Ruby on Rails
       + AJAX (remember that it was once called that?)
       + &ldquo;Release everything but your secret sauce&rdquo; (cf: <a href="http://tom.preston-werner.com/2011/11/22/open-source-everything.html">Preston's *Open Source (Almost) Everything*</a>)
       
+ Web developers didn't pick copyleft &hellip;
       + &hellip; maybe because we hadn't given them a copyleft.
       + permissive MIT license &amp; 3-clause BSD rules the web.

+ This is server-side, trade-secret software.

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

# The Client Proprietary (aka Javascript Trap)

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
 &mdash; Erik Meijer of Microsoft, on 5 July 2011.
</p>
</span>

# The Application

<img src="dark-ages.jpg" align="right"  />

+ Today, most new applications deploy online &hellip;
       + as a mix of trade-secret server-side plus proprietary client-side Javascript &hellip;
       + from infrastructure-level like OpenStack  &hellip;
       + to *even* developer tools like GitHub/BitBucket (!) &hellip;
       + to end-user applications: FaceBook, Twitter, GooglePlus.

+ The dark ages are coming!

# Dark Ages? Really?

<img src="monk-scriptorium.jpg" align="right"  />

+ The developers (monks) have the source code (books).

# Dark Ages? Really?

<img src="serfs-pray.jpg" align="right"  />

+ The people (users) trust the power of the church (Facebook).

# Dark Ages? Really?

<img width="664" height="448" src="monks.jpg" align="right"  />

+ We cloistered few shall have freedom:
      + source code haves and have-nots  &hellip;
      + &hellip; (again!)

# Generational Change

+ Has today's developer chased a bug from the top to the bottom?

+ Will tomorrow's developer ever need to?
       + Is the complexity too much anyway?

+ Will tomorrow's developer care?
       + The past cloistered missed Free Software entirely, after all.

# Hindsight

+ Maybe this was inevitable?
      + Even if GPLv2.2 came out in mid-2002 &hellip;
      + Generational disconnect was the primary factor.

+ Who's AGPLv3 for today?

# The Great Abuse

<img width="274" height="383" align=right src="marten-mickos.jpg"/>

+ Proprietary relicensing (by holding all copyright).

+ License enforcement with profit as its primary (and only?) goal.

+ MySQL would shake down GPL users to buy proprietary licenses they didn't need.

+ More copyleft means more shakedowns.

+ Most common use of AGPLv3 today.

+ It makes me sick.

# Community Development

+ AGPLv3's intended for community development.

+ Lots of copyright holders:
        + all bound to each other by copyleft.

+ The great trust of copyleft.

+ Sadly, few are writing this code.

# The Great Marketing Challenge

+ The Free Software Twitter exists &hellip;
      + &hellip; StatusNet; it's AGPLv3'd
      + &hellip;  but it's a ghost-town compared to Twitter.

+ The Free Software tumblr/flickr exists &hellip;
      + &hellip; GNU Mediagoblin; it's AGPLv3'd
      + &hellip;  but it's a ghost-town compared to tumblr/flickr.

+ We're back to catching up to proprietary software:
      + Like GNU had to catch up to Unix.
      + That took almost 20 years!

# More Info / Talk License

+ URLs / Social Networking / Email:
     - Conservancy: sfconservancy.org &amp; @conservancy
     - Me: faif.us, ebb.org/bkuhn &amp; @bkuhn (identi.ca only)
     - Slides at: ebb.org/bkuhn/talks &amp; gitorious.org/bkuhn/talks (source)

<span class="fitonslide">
<p>Presentation and slides are: Copyright &copy; 2008, 2009, 2010, 2011, 2012, 2013 Bradley M. Kuhn, and are licensed under the <a href="http://creativecommons.org/licenses/by-sa/3.0/usa/">Creative Commons Attribution-Share Alike (CC-By-SA) 3.0 United States License</a>. <img src="cc-by-sa-3-0_88x31.png"/></p>

<p>Some images included herein are &copy;'ed by others. I believe my use of those images is fair use under USA &copy; law.  However, I suggest you remove such images if you redistribute these slides under CC-By-SA-USA 3.0.
</p>
</span>
