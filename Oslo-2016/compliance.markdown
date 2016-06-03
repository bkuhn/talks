% Tales from 20 Years of Copyleft Enforcement
% Bradley M. Kuhn
% Friday 3 June 2016

# The Guiding Moral Theory

<hr/>

> Fighting for software freedom means trying to build a world where every
> user has the unencumbered, inalienable right to copy, share, modify,
> redistribute, upgrade and improve all the software on which they rely.

# The Final Goal

<hr/>

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
[copyleft.org](https://copyleft.org/) </p> </span>

# What is GPL Enforcement?

+ Broadly, GPL enforcement is the process of ensuring that redistributors
  grant the rights that copyleft assures.

+ The primary goals are:
     + ensure that the users of a product containing copylefted works can
       participate upstream by testing, building, and enhancing the work on
       the actual device.
     + help distributor themselves join and contribute back to the upstream
       project.

+ *The Principles of Community-Oriented GPL Enforcement* [at sfconservancy.org/linux-compliance/principles.html](https://sfconservancy.org/linux-compliance/principles.html).

# But It's Not *Really* About Upstream.

+ Nevertheless, enforcement pursues that second goal only indirectly.

+ GPL compliance is usually *not* about what to do upstream.

+ GPL is a license made for the users, not the developers.
     + Who, of course, may be future developers.

+ The main policy goal:
     + Ensure the user can exercise the freedom to modify the software &hellip;
     + &hellip; in a manner that's real and concrete, not theoretical.

# What's a GPL Violation?

+ GPL (both v2 and v3) require:
     + The whole work licensed under GPL.
     + (which means all copyrighted material added must be under
       GPL-compatible licenses.)
     + Complete, Corresponding Source (CCS) of that work provided, under GPL.

+ The licenses terminate upon violation &hellip;
     + &hellip; thus failure to comply means lost distribution rights.
     + &hellip; enforcement uses this rights termination as leverage to
       restore compliance.

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

# My First CCS Check

+ In mid-2000, RMS sent me a proposed source release to verify for compliance
  on a GNU tar violation.

+ They'd modified GNU tar to support various other filesystems.

+ There was also some odd &ldquo;cryptography support&rdquo;.
     + I suspected they'd been resisting compliance because it was
       security-though-obscurity.
       + The passphrase appeared to be written to tape.

# Enforcement is Technical

+ Copyleft's policy goals related to technical acts.
     + modifying, building, and installing software is a technical process.

+ In embedded systems, this process is rarely straightforward.
     + Yet GPL requires that such be possible.

+ In enforcement, we talk about &ldquo;the CCS adequately meeting GPL's requirements&rdquo;

# How GPLv3 says CCS.

<hr/>

> The "Corresponding Source" for a work in object code form means all the source code needed to generate, install, and (for an executable work) run the object code and to modify the work, including scripts to control those activities.
<span class="fitonslide">
<p align=right>
&mdash; GPLv3&sect;1
</p>
</span>

# How GPLv2 says CCS.

<hr/>

> You may copy and distribute the Program (or a work based on it, under
> &sect; 2) in object code or executable form under the terms of &sect; 1
> &amp; 2 above provided that you &hellip; [a]ccompany it with the complete
> corresponding machine-readable source code &hellip; The source code for a
> work means the preferred form of the work for making modifications to it.
> For an executable work, complete source code means all the source code for
> all modules it contains, plus any associated interface definition files,
> plus the scripts used to control compilation and installation of the
> executable.

<p align=right>
&mdash; GPLv2&sect;3
</p>
</span>

# The 11 Words That Consumed My Life

+ GPLv2 enforcement, for embedded products, is all about the these eleven
  words.

+ I could give an entire talk on any one of these 11 words.
    + Yes, I can even give 20-30 minute treatises on each use of &ldquo;the&rdquo;. 

+ Yet, when enforcement processes are at their best, they're about the spirit
  behind these words, not the words themselves.

<hr>
> the scripts used to control compilation and installation of the executable.

<p align=right>
&mdash; GPLv2&sect;3
</p>
</span>

# The 11 Words That Consumed My Life

+  Basic reference rule:
     + Can a developer reasonably skilled in the art of embedded software
       build your sources, take the (copylefted) executables and install
       them?

+ Enforcement spends its most attention on testing CSS
  &ldquo;candidates&rdquo; to verify that.

<hr>
> the scripts used to control compilation and installation of the executable.

<p align=right>
&mdash; GPLv2&sect;3
</p>
</span>

# Tar Wars Continue

+ There were a number of these backup solutions on the market.

+ All of them had modified tar, it seemed.

+ All but one came into compliance.

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

# Success in Court

+ The &ldquo;Big One&rdquo;:
[Software Freedom Conservancy, et al vs. Best Buy et al.](https://ia600207.us.archive.org/21/items/gov.uscourts.nysd.355978/gov.uscourts.nysd.355978.docket.html)

+ Settle with most of the defendants for actual compliance *on BusyBox*.
      + Linux compliance is sometimes elusive (more on that later).

+ Received a [default judgment against Westinghouse](http://www.archive.org/download/gov.uscourts.nysd.355978/gov.uscourts.nysd.355978.131.0.pdf).

# The Default Judgment

<img width="274" height="383" align=right src="shira-scheindlin.jpg"/>

+ &ldquo;[Westinghouse is] still producing these BusyBoxes&rdquo;.

+ Judge Scheindlin honors our request to have all their TVs donated to
  charity, and an injunction on further selling.

+ The lawyers for Westinghouse quit, saying they aren't getting paid and
  their client is broke.

# Violators Are Often Corrupt

+ Westinghouse used a bizarre bankruptcy rule in California.
     + You go out of business on a Friday.
     + Transfer all assets to another company on a Saturday.
     + Go back into business under a similar name on Monday morning.
     + The brother of the previous CEO is the new CEO.

+ The new defendant is added, with a new lawyer.
     + The previous lawyer sits in the back of the Court and shouts
       directions to the new lawyer!

# Age of the Savvy Violator

+ The days of the innocent mistake violation are coming to an end.
    + Eternal September principle ensures there will always be some.
    + But we know how to solve those.

+ The truly dangerous violators now hire lawyers in advance to prepare
  arguments and plans to fight if anyone questions their right to keep Linux
  modules proprietary.

+ They are wily &amp; experienced opponents, whom, ironically, we are helping
  with our open communication, transparency and honesty.

# The Tempest in the Toybox

+ Conservancy had sought Linux compliance via BusyBox enforcement.
    + My view was that this consolidated claims.
    + Violators realize this is a politically weak spot &hellip;
    + &hellip; &amp; seek to drive a political wedge in community.
    + Industry consortia send their proxies to
      [attack BusyBox enforcement](https://lwn.net/Articles/478674/)
      [with specious in the press](https://lwn.net/Articles/478702/).

+ Our methods were of course legally sound, but becoming politically unviable.

# Fighting anti-enforcement industry consortia

+ Companies that adopt Linux have always wanted GPL enforcement to end.

+ They redouble their efforts during BusyBox suits.

+ Company-controlled Linux community representatives insist BusyBox copyright
  holders never ask for Linux compliance.

+ Many community developers (Matthew Garrett, Ben Hutchings, David Woodhouse,
  and many others) come forward &amp; ask Conservancy to directly enforce on
  their behalf.

+ [The GPL Compliance Project For Linux Developers](https://sfconservancy.org/copyleft-compliance/) Is Born.

# Why Linux?

+ Corporate lawyers have decided to stand their ground here:

+ Corporate lawyers advise their clients to create proprietary Linux modules, and fight us.

+ Linux proprietary module enforcement.

# Linux's GPL Elephant

<img src="elephant-in-the-room_400x415.jpg" align="right"  />

+ Much debated: Are Linux modules combined works of Linux?
      + I have yet to see an example of one that didn't seem to be such.
      + Corporate lawyers are planning how they can stop us from proving that.

+ Through the accident of history (&amp; lots of great work by Linux
hackers):
      + Linux is the battle ground for copyleft.

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
