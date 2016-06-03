% Tales from 20 Years of Copyleft Enforcement
% Bradley M. Kuhn
% Friday 3 June 2016

# The Guiding Moral Theory

> Fighting for software freedom means trying to build a world where every
> user has the unencumbered, inalienable right to copy, share, modify,
> redistribute, upgrade and improve all the software on which they rely.

# The Final Goal

> IMO, the final goal of the software freedom movement is to change the world
> so that all software available is Free Software, giving every users those
> key inalienable rights.

# What is Copyleft?

+ Fundamentally, copyleft is a strategy, not a moral imperative onto itself.

+ We must never forget: the goal is software freedom.

+ Copyleft is simply a tool to help us get there.

# Formal Definition of Copyleft

<hr/>

> Copyleft is a strategy of utilizing copyright law to pursue the policy goal
> of fostering &amp; encouraging the equal &amp; inalienable right to copy,
> share, modify &amp; improve creative works of authorship. Copyleft &hellip;
> describes any method that utilizes the copyright system to achieve the
> aforementioned goal. Copyleft as a concept is usually implemented in the
> details of a specific copyright license &hellip; Copyright holders of
> creative work can unilaterally implement these licenses for their own works
> to build communities that collaboratively share &amp; improve those
> copylefted creative works.

<span class="fitonslide"> <p align=right> &mdash; Definition of copyleft from
copyleft.org </p> </span>

# What is GPL Enforcement?

+ Broadly, GPL enforcement is the process of ensuring that redistributors
  grant the rights that copyleft assures.

+ The primary goals are:
     + ensure that the users of a product containing copylefted works can
       participate upstream by testing, building, and enhancing the work on
       the actual device.
     + help distributor themselves join and contribute back to the upstream
       project.

+ [*The Principles of Community-Oriented GPL Enforcement* at sfconservancy.org/linux-compliance/principles.html](https://sfconservancy.org/linux-compliance/principles.html).

# But It's Not *Really* About Upstream.

+ Nevertheless, enforcement pursues that second goal only indirectly.

+ GPL compliance is usually *not* about what to do upstream.

+ GPL is a license made for the users, not the developers.
     + Who, of course, may be future developers.

+ The main policy goal:
     + Ensure the user can exercise the freedom to modify the software &hellip;
     + &hellip; in a manner that's real and concrete, not theoretical.

# Earliest Copyleft Programs

<img src="emacs.png" align="right" />

+ GNU Emacs: was the first GPL'd program.

+ AFAIK Emacs' copyleft never been violated.

# Second Copyleft Program

<img src="gcc_sm.png" align="right" width="440" height="508"  />

+ GCC: second GPL'd program.
     + much more interesting to proprietary software companies.

+ So, who was the first GPL violator?

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

# Tar Wars

<img width="274" height="383" align=right src="tar-wars.gif"/>

<p> A long time ago, in a city far far away, the Empires had taken GNU tar
and placed it into proprietary backup solutions.  A small band of freedom
fighters enforced the GPL to liberate users who were oppressed by the
proprietary nature of GPL violators.</p>

# Tar Wars

+ Tape backup systems essential in late 1990s.

+ Many companies made forks of GNU Tar, and violated.

+ Sysadmins were good at finding these violations.

+ All but one violator came into compliance.

# Court May Not Mandate Source Release

+ Last GNU tar enforcement I ever did was circa mid-2002.

+ Company decided to *remove* tar &amp; rewrite rather than compliance.

+ Let's sue!

+ Lawyers told me courts are unlikely to order a source release as a remedy.

+ Courts usually give money and an injunction
     - Company already gave latter of their own accord (de-facto injunction)

# Coalition of the Willing

<img align=right src="wrt54g.png"/>

+ Spring 2003: dozens of reports on WRT54G.

+ Discussions begin with Cisco (who'd bought Linksys just weeks before)

+ Story hits slashdot on 2003-06-08

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

<img align=right src="harald-welte.jpg"/>

+ FSF was initially shy about lawsuits.

+ Harald disagreed with FSF strategy (in hindsight, he was right).

+ launches multiple lawsuits in Germany (about 8 between 2005-2008).

+ Quite successful, although has in some cases, courts only grant injunction.

# GCC Redux, 2003-2005

+ Embedded systems become major part of industry.

+ GCC is the best compiler.

+ Many companies start making GCC-based toolchains.

+ Focus of post-WRT54G enforcement at FSF.

# Enforcement Corruption: MySQL

<img width="274" height="383" align=right src="marten-mickos.jpg"/>

+ Proprietary relicensing (by holding all copyright).

+ GPL enforcement with profit as its primary (and only?) goal.

+ MySQL would shake down GPL users to buy proprietary licenses they didn't need.

+ I wish I'd identified this as corruption sooner.

+ Most for-profit enforcers do not follow [*The Principles of Community-Oriented GPL Enforcement*](https://sfconservancy.org/linux-compliance/principles.html).

# Embedded Violations Prevalent

+ Erik Andersen becomes exasperated by mid-2006.
     - post-Linksys compliance, router &amp; NAS market is a violation haven.

+ Erik asks for help.

+ Conservancy becomes his enforcement agent (&amp; receive some others' &copy; assignment)

+ Conservancy has had > 100 GPL violations queued for action since 2007.
     - Conservancy's list is now > 300

# The First Era of GPL Litigation

+ Lawsuits become undeniably necessary.
     - Dan Ravicher &amp; Aaron Williamson file some in USA: for Conservancy &amp; Erik.

+ Focus is to settle:
     - More than anything else, we want full compliance &hellip;
     - &hellip; on *all* GPL'd and LGPL'd components &hellip;
     - &hellip; judge is unlikely to grant us all that &hellip;
     - &hellip; so we work hard to settle on that request.

# Companies Want To Replace Copyleft

+ Companies scramble to replace BusyBox with Toybox.

+ Companies scramble to replace GCC with LLVM.

+ What community copyrighted GPL'd packages will remain essential?

# Linux's GPL Elephant

<img src="elephant-in-the-room_400x415.jpg" align="right"  />

+ Much debated: Are Linux modules combined works of Linux?
      + I have yet to see an example of one that didn't seem to be such.
      + Corporate lawyers are planning how they can stop us from proving that.

+ Through the accident of history (&amp; lots of great work by Linux
hackers):
      + Linux is the battle ground for copyleft.

# Why Linux?

+ Corporate lawyers have decided to stand their ground here:

+ Corporate lawyers advise their clients to create proprietary Linux modules, and fight us.

+ Linux proprietary module enforcement.

# Age of the Savvy Violator

+ The days of the innocent mistake violation are coming to an end.
    + Eternal September principle ensures there will always be some.
    + But we know how to solve those.

+ The truly dangerous violators now hire lawyers in advance to prepare
  arguments and plans to fight if anyone questions their right to keep Linux
  modules proprietary.

+ They are wily &amp; experienced opponents, whom, ironically, we are helping
  with our open communication, transparency and honesty.

# Zero-Sum Game

+ Meanwhile, copyleft enforcement is a zero sum game.

+ If we win, software that should be free is liberated.

+ If they win, software that should be free remains proprietary.

+ Our goals are diametrically opposed.

# Funding Enforcement

+ Enforcement done for profit is a path to corruption.

+ Violators always give us a choice: how much money does it take to buy
  permission to violate the GPL?

+ The moment you take the money without full compliance, you've just de-facto
  entered the proprietary relicensing business.

+ The amount offered goes down exponentially compared to the amount of time
  we insist on full compliance.

# Funding Enforcement

+ The only way to fund community enforcement is for the community to support
it.

+ We are fundraising from the public, because principled enforcement is never
  fully self-funding.

+ You can donate to help: [sfconservancy.org/supporter/](https://sfconservancy.org/supporter/)

# More Info / Talk License

<img align="right" src="cc-by-sa-4-0_88x31.png" />

+ URLs / Social Networking / Email:
     - Pls. support Conservancy: [sfconservancy.org/supporter/](https://sfconservancy.org/supporter/)
     - If you hold copyrights in Linux, Debian, Samba, or BusyBox, you can
       join our enforcement coalition.  [Contact us!](https://sfconservancy.org/linux-compliance/about.html)
     - [*The Guide*](https://copyleft.org/guide) is available &amp; [welcomes contributions at copyleft.org](https://copyleft.org).
     - Conservancy: [sfconservancy.org](https://sfconservancy.org/) &amp; <a href="https://twitter.com/conservancy/">@conservancy</a>.
     - Me: [faif.us](http://faif.us) &amp; [ebb.org/bkuhn](http://ebb.org/bkuhn)
     - Slides: [ebb.org/bkuhn/talks](http://ebb.org/bkuhn/talks/Oslo-2016/compliance.html).

<span class="fitonslide">
<p>Presentation and slides are: Copyright &copy; 2012, 2014, 2015, 2016 Bradley M. Kuhn, and are licensed under the <a rel="license" href="https://creativecommons.org/licenses/by-sa/4.0/legalcode">Creative Commons Attribution-Share Alike 4.0 International License</a>. </p>
<p>Some images included herein are &copy;'ed by others. I believe my use of those images is fair use under USA &copy; law.  However, I suggest you remove such images if you redistribute these slides under CC-By-SA 4.0.
</p>
</span>

# ZFS (Since You Asked)

+ [Conservancy's](https://sfconservancy.org/blog/2016/feb/25/zfs-and-linux/)
  and [FSF's](https://sfconservancy.org/blog/2016/apr/11/fsf-zfs/) statements
  really say it all.

+ Fundamentally, there is *little legal difference* between a
  GPL-incompatible license that gives source code and one that doesn't.

+ Tolerating CDDL-only modules in Linux is a backdoor to tolerating
  proprietary Linux modules.

+ The nasty GPL violators are seeking to exploit the people who bolster
  ZFSOnLinux as a method to justify their own GPL violations.

+ Thus, we must take the clear stand, that is supported by copyright law:
    + You need permission to distribute the binary combination of zfs.ko
      &mdash; Linux.
    + Neither CDDL nor GPL give you that permission, so it's copyright
      infringement when you do that distribution.
    + So, don't do it.  Sorry.  I wish the legal details worked out another
      way.  But they don't.
      
<!--  LocalWords:  ldquo rdquo RSA img src shuttleworth jpg SSL CACM href sa
 -->
<!--  LocalWords:  Paywalls codebases codebase FOSDEM Source'd ACM png
 -->
<!--  LocalWords:  blogosphere sfconservancy
 -->
