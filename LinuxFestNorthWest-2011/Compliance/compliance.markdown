% 12 Years of GPL Compliance: A Historical Perspective
% Bradley M. Kuhn
% Friday 29 April 2011

# My History

+ Worked my first GPL enforcement case in 1999 (as FSF volunteer).

+ Started working for FSF in 2000 (until 2005).

+ Worked at SFLC from 2005-2010.

+ Now Executive Director of Software Freedom Conservancy.

+ Plurality of my time since 1999 has been spent on GPL enforcement.

# Earliest Copylefted Programs

+ GNU Emacs: AFAIK Emacs' copyleft never been violated.

+ GCC: much more interesting to proprietary software companies.

+ Who was the first GPL violator?

# The NeXT Shall be First

<img src="steve-jobs-next.jpg" align="right"  />

+ Objective-C front end.

# Earliest Post I Could Find
<span class="fitonslide">
<p>
Path: utzoo!utgpu!jarvis.csri.toronto.edu!mailrus!cs.utexas.edu!usc!apple!bbn!bbn.com!bpalmer<br/>
From: bpal...@bbn.com (Brian Palmer)<br/>
Newsgroups: gnu.misc.discuss<br/>
Subject: Objective Gnu?<br/>
Message-ID: &lt;5768@bbn.COM&gt;<br/>
Date: 19 Sep 89 15:36:16 GMT<br/>
</p>

<p>In "The NeXT Book" by Bruce Webster, he says: (page 134):</p>
<p>
	Objective C is based on the Gnu C compiler developed by
	Richard Stallman.  Release 0.9 has merged the Objective
	C syntax with the the Gnu C compiler to speed up compilation
	and to produce faster, more efficient code.
</p>


<p>Are they using FSF software in their product? Or is Webster just badly
explaining the situation ...  and Objective C is just preprocessing and
passing C to gcc.</p>

<p>Otherwise Gang, I see a Copyleft violation right?</p>
<br/>
Brian
</span>


# NeXT Answers

<span class="fitonslide">
<p>
Path: utzoo!utgpu!jarvis.csri.toronto.edu!rutgers!apple!gem.mps.ohio-state.edu!tut.cis.ohio-state.edu!NEXT.COM!Matthew_Self<br/>
From: Matthew_S...@NEXT.COM<br/>
Newsgroups: gnu.gcc<br/>
Subject: Objective-C front end for GCC from NeXT<br/>
Message-ID: &lt;8909210104.AA14825@batcomputer.NeXT.COM&gt;<br/>
Date: 21 Sep 89 01:01:50 GMT<br/>
Sender: dae...@tut.cis.ohio-state.edu<br/>
</p>

<p>In response to Steve Simmons' inquiry about an Objective-C
front-end for GCC, NeXT will be making our modifications to
GCC for Objective-C available very soon.</p>

<p>Once GCC-1.36 is released (any day now), I will create a patch
kit which will be announced on this mailing list.  (The modifications
are very small.)</p>
<br/>

Matthew Self
</span>


# Thus Begins Jobs' GPL hatred.

<img src="steve-jobs-bond.jpg" align="right"  />

+ Apple to this day works hard to ditch GCC.

+ Funds LLVM.

+ Spreads FUD about GPLv3.

# Tar Wars

<img width="274" height="383" align=right src="tar-wars.gif"/>

<p> A long time ago, in a city far far away, the Empires had taken GNU tar
and placed it into proprietary backup solutions.  A small band of freedom
fighters enforced the GPL to liberate users who were opressed by the
proprietary nature of GPL violators.</p>

# Tar Wars

+ Tape backup systems essential in late 1990s.

+ Many companies made forks of GNU Tar, and violated.

+ Sysadmins were good at finding these violations.

+ All but one violator came into compliance.

# Courts may never give compliance.

+ Last GNU tar enforcement I ever did was circa mid-2002.

+ Company decided to *remove* tar &amp; rewrite rather than compliance.

+ Let's sue!

+ Lawyers told me court wouldn't give compliance as a rememdy.

+ Courts usually give money and an injuction
     - Company already gave latter of their own accord (de-facto)

# Coalition of the Willing

FIXME: photo of a WRT54G

+ Spring 2003: dozens of reports on WRT54G.

+ Discussions begin with Cisco (who'd bought Linksys just weeks before)

+ Story hits slashdot 2003-06-08

+ FSF puts together group to do enforcement.
     - key members: Erik Andersen (BusyBox) &amp; Harald Welte (Linux)

# Compliance Takes Soooo Long

+ FSF represents the coalition.

+ Broadcom is discovered as upstream.

+ WRT54G source is released (but wireless driver kept proprietary).

+ Broadcom argues FCC prohibits; FSF agrees not to pursue (can't really anyway).

+ WRT54G releases spawns OpenWRT community.

+ Harald is frustrated.

# GPL-violations.org

+ FSF was initially shy about lawsuits.

+ Harald disagreed with FSF strategy (in hindsight, he was right).

+ launches multiple lawsuits in Germany (about 8 between 2005-2008).

+ Quite successful, although has same &ldquo;courts generally only grant injunction&rdquo; again.

# GCC Redux, 2003-2005

+ Embedded systems become major part of industry.

+ GCC is best compiler.

+ Many companies start making GCC-based toolchains.

+ Focus of post-WRT54G enforcement at FSF.

# Funding Crisis for Enforcement

+ FSF had hoped to raise funds &ldquo;certifying compliance&rdquo;.

+ You can't break even on this for less than $10,000/release.

+ No one is willing to pay (still true today, AFAICT).

+ Those who'd know enough to buy services think they'll get away with violations anyway.

# Money

+ No one in non-profits is getting rich from this.

+ Who should pay for enforcement: 
     - Compilers or Violators?
     - Individual donors.

+ There must be a deterrent.

+ Non-profit enforcement == accountability.

+ Confidentiality is something violators ask for.

# Enforcement Corruption: MySQL

<img width="274" height="383" align=right src="marten-mickos.jpg"/>

+ Proprietary relicensing (by holding all copyright).

+ GPL enforcement with profit as its primary (and only?) goal.

+ MySQL would shake down GPL users to buy proprietary licenses they didn't need.

+ I wish I'd identified this as corruption sooner.

# Embedded Violations Prevalent

+ Erik Andersen becomes exasperated.
     - post-Linksys compliance, router &amp; NAS market is a violation haven.

+ Eirk asks for help.

+ Conservancy becomes his enforcement agent (and gets some others &copy; assignment)

+ Conservancy has had > 100 (now > 300) GPL violations queued for action since 2007.

# The Era of GPL Litigation

+ Lawsuits become necessary.
     - Dan Ravicher &amp; Aaron Williamson file some in USA.

+ Focus is to settle:
     - What we want more than anything else is full compliance &hellip;
     - &hellip; on *all* GPL'd and LGPL'd components &hellip;
     - &hellip; no judge will grant us all that &hellip;
     - &hellip; so we work hard to settle on that request &hellip;
     - &hellip; taking money &amp; injunctions only as a consolation prize.

+ But why is full compliance so hard for these companies?

# The Upstream Problem

<img align=left src="michael-scott.jpg"/>

When I said that I was king of forwards, you got to understand that I
don't come up with this stuff. I just forward it along. You wouldn't
arrest a guy who was just passing drugs from one guy to another.

<p align="right">
 -- Michael Scott, *The Office* 
</p>

FIXME: which episode?

# Suppliers Bully OEMs, AFAICT 

FIXME: cop image?

+ I'd be the worst cop in the world.

+ No one ever turns &ldquo;states' evidence&rdquo;
     - &hellip; at least they don't for _me_, anyway.

+ Me: &ldquo;Please, just tell me on the record your supplier violator&rdquo;

+ Them: &ldquo;We'll work with our upstream to get into compliance.&rdquo;

# Linksys Redux

+ 2003-2004, everything they put out is VxWorks.

+ Circa late 2004, BusyBox/Linux &amp; GNU/Linux slowly becomes the Linksys default again.

+ FSF finally gets fed up and sues.

# C&CS Remains Hardest Part

+ GPL/LGPL is by far the most popular software license.
     - Shown clearly in Google Code Search (proprietary data) &amp;
     - SourceForge License Data (open data)

+ GPLv2: &ldquo;scripts to control compilation and installation of the executable&rdquo;

+ GPLv3: &ldquo;Install Information&rdquo;

# Today.

<img align="right" height="473" width="557" src="DQWindmill.gif"/>

+ I continue on GPL enforcement for Conservancy projects.
     - new reports at least once a week.

+ Matthew Garrett works hard on Android device compliance.

+ FSF is overwhelmed with violation reports.

+ Armijn (of gpl-violations.org) volunteers sporadically.

# Today.

<img align="right" height="473" width="557" src="DQWindmill.gif"/>

+ GPL Violations *are* *everywhere*.

+ I'll take an even money bet for (almost) any amount:
     - Give me an hour, an Internet connection, and my laptop &hellip;
     - &amp; I'll find you a GPL-violating firmware I've never seen before.

# More Info / Talk License

+ Conservancy Website: http://sfconservancy.org/

+ My blog: ebb.org/bkuhn/blog

+ Personal Microblog: @bkuhn (on identi.ca)

+ Conservancy Microblog: @conservancy (on identi.ca and twitter)

This talk and the slides are:

Copyright &copy; 2008, 2009, 2010, 2011 Bradley M. Kuhn.

<img src="cc-by-sa-3-0_88x31.png"/>
<a href="http://creativecommons.org/licenses/by-sa/3.0/us/">This presentation and these slides are licensed under a <a href="http://creativecommons.org/licenses/by-sa/3.0/us/">Creative Commons Attribution-Share Alike 3.0 United States License</a>.
            
