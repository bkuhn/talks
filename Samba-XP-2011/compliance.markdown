% Samba, GPL Enforcement, and the GPLv3
% Bradley M. Kuhn
% Tuesday 10 May 2011

# My History

+ Worked my first GPL enforcement case in 1999 (as FSF volunteer).

+ Started working for FSF in 2000 (until 2005).

+ Worked at SFLC from 2005-2010.

+ Now Executive Director of Software Freedom Conservancy.
    + &hellip; which is the non-profit home to Samba.
    + Conservancy does GPL enforcement on as part of our services.

+ Plurality of my time since 1999 has been spent on GPL enforcement.

# Nature of Free Software Community

+ Through the eyes of a GPL enforcer &hellip;

+ The Free Software Community is separated into two equally important groups:
     + The permissively licensed, who use social pressure to liberate code.
     + The copyleft licensed, whose license requires liberation.

+ Mine are the stories of the latter.

# On Requirement By License

<img src="Constitution.jpg" align="right"  />

+ Social pressure *does* work &hellip;
     + &hellip; and should be used (and is), even for copylefted software.
     + &hellip; enforcement is a last resort.

+ GPL == Constitution of Software Freedom Land.
     + a &ldquo;written down&rdquo; embodiment of core principles.

+ GPL's a detailed implementation of the four freedoms:
     + freedom to run and study.
     + freedom to improve.
     + freedom to share.
     + freedom to share improvements.

# Who Is This Talk For?

+ This talk isn't for you.

+ Well, I wrote for you so, it's *for* you.

+ But, it's not *about* you.

+ Sophisticated users and developers generally comply with GPL.

# How GPL Works (Theoretically)

<img src="theory-vs-practice.jpg" align="right"  />

+ Copyright: the internationalized standard for authors' controls over works.

+ Use copyright license to grant permission.

+ Make permission conditional on giving your downstream the four freedoms.

+ This is the copyright law hack of copyleft.

+ Copyright rules require compliance with the license.

# How GPL Works (In Reality)

<img src="copyleft-e-copyright.jpg" align="right"  />

+ What do you do when someone violates?
     + (and social pressure for compliance fails)?

+ Copyright enforcement
     + &hellip; (yes, similar stuff to what the MPAA does: EEP!)
     + &hellip; but for a *good* cause: the four freedoms.
     + &ldquo;using the tools of the oppressor against the oppressor&rdquo;

# Brief History of GPL Enforcement

<img src="emacs.png" align="right" />

+ GNU Emacs: was the first GPL'd program.

+ AFAIK Emacs' copyleft never been violated.

# Brief History of GPL Enforcement

<img src="gcc_sm.png" align="right"  />

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
Date: 19 Sep 89 15:36:16 GMT<br/>nnn
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

+ As you know, they've ditched Samba
     + Don't take it personally: 
     + Jobs hated your license since before Samba existed.

+ Apple to this day works hard to ditch GCC.
     + LLVM funding.

+ Spreads FUD about GPLv3.

# Practicing Avoidance

+ GPL is now well-known in the software industry.

+ The saavy make a conscious choice:
    + Adopt GPL technology, and comply.
    + Or, avoid it entirely.

+ That's why this talk isn't about you.
    + e.g.: Chris DiBona's &ldquo;Google will clear up any GPL violation in 24 hours&rdquo;

+ Everyone makes mistakes; I just want to see them set right in a timely fashion.

+ So, who the heck am I talking about?

# Onslaught of Embedded Violation

+ Conservancy has had > 100 GPL violations queued for action since 2007.
     - Conservancy's list is now > 300

+ Nearly all of them are:
     + embedded products.
     + made cheaply with a poorly-thrown-together software build.
     + add no significant *new* code (a few minor patches at most).
     + the key &ldquo;innovation&rdquo; is the build/install system.

+ Conclusion: it's the unsophisticated company that's most likely to violate GPL.

# So, why do we care?

<img src="helpless.jpg" align="right"  />

+ These companies undercut those that comply.

+ The end-users buy these devices.

+ The software build is often poorly put together.

+ The community wants make it better.

+ They can't; even if there were minimal feature changes. 

+ Users are left helpless.


# Freedom In Practice, Not Theory

+ GPL isn't just there to prevent proprietary improvements.

+ It's there to defend *all* the software freedoms:
     + copy, share, **modify** and redistribute.

+ What does it mean to **modify** software for an embedded device?

# Embedded Device Software Freedom

+ Sure, I've got the sources.

+ But, can I build it in the same way the company did?

+ If I get it built, can I install it?

+ By the time I get all that working, will the device be discontinued?

+ Will they get away with it if they do, only to violate in the next product line?

+ In the age of the embedded device, copyleft seeks to answer these questions correctly.

# GPL Predicted this Problem 

+ Even in 1991, RMS made sure GPLv2 handled this.

# GPLv2: More than Just Source

<p>For an executable work, complete source
code means all the source code for all modules it contains, plus any
associated interface definition files, plus <strong>the scripts used to
control compilation and installation of the executable</strong>.</p>

<p>(empahsis mine)</p>

# GPLv2: More than Just Source

+ &ldquo;the scripts to control&hellip;&rdquo; gets us close.

+ It handles most of the issues.

+ I even argued it includes authorized install information.
     + Unfortunately, RMS gave in on that one.

# GPLv3: Installation Information

<span class="fitonslide">
<p>"Installation Information" for a User Product means any methods,
procedures, authorization keys, or other information required to install
and execute modified versions of a covered work in that User Product from
a modified version of its Corresponding Source.  The information must
suffice to ensure that the continued functioning of the modified object
code is in no case prevented or interfered with solely because
modification has been made.</p>

<p>If you convey an object code work under this section in, or with, or
specifically for use in, a User Product, and the conveying occurs as
part of a transaction in which the right of possession and use of the
User Product is transferred to the recipient in perpetuity or for a
fixed term (regardless of how the transaction is characterized), the
Corresponding Source conveyed under this section must be accompanied
by the Installation Information.</p>
</span>

.

# GPLv3: Installation Information

+ In my view, just clarifies GPLv2's terse wording.

+ In any event, it makes it certain.

+ Users of device can modify and upgrade their devices &hellip;
     + &hellip; as it should be.

+ This is one of the reasons projects should upgrade to GPLv3.

# Samba Team: GPLv3 Trailblazers

+ Samba is the only program in the embedded stack under GPLv3.
     + unfortunately
     + (&hellip; but that's not your fault, Samba Team DTRT. :)

+ Assuring freedom to modify may fall to Samba copyright holders.
     + certainly in crypto-locked-down products.

+ Enforcement is about entire software stack builds, not just single programs.

+ Users deserve the right to upgrade when and how *they* want to.

# Challenges of Modern Compliance

+ Saavy violators meant intelligent discussion.
    + Jobs knew just what he was trying to get away with re: Objective C.

+ Clueless violators means difficult conversations:
     + Me: &ldquo;Your software violates GPL.&rdquo;
     + Them: &ldquo;We make hardware.&rdquo;
     + Me: &ldquo;I know, but it has software in it.  Our members' software. Under the GPL.&rdquo;
     + Them: &ldquo;No, it doesn't. We make hardware.&rdquo;
     + Me: &ldquo;But your firmware download&hellip;on *your* website&hellip;that's software.&rdquo;
     + Them: &ldquo;Oh, that's not ours.  We got that from someone.  Nothing to do with us.&rdquo;

+ Having the above conversation across four phone calls every two months is why I seem so insane most of the time.

# The Upstream Problem

<img align=left src="michael-scott.jpg"/>

When I said that I was king of forwards, you got to understand that I
don't come up with this stuff. I just forward it along. You wouldn't
arrest a guy who was just passing drugs from one guy to another.

<p align="right">
 -- Michael Scott, *The Office* 
</p>

# The Upstream Problem

+ (Mostly) small companies churn out the software builds for various OEM boards.

+ Companies (big and small) acquire both as a unit.

+ Aren't even sophisticated enough to realize they have software licensing obligations.

+ Enforcement is the moral equivalent of:
      + Me: &ldquo;Hey, Company Foo, meet your developers!  They're called the copyleft community&rdquo;.
      + &hellip; and convincing them they'd rather meet those developers than &ldquo;get away with it&rdquo;.

# Today's Enforcement Work

<img align="right" height="473" width="557" src="DQWindmill.gif"/>

+ I continue on GPL enforcement for BusyBox and uClibc.

+ New reports at least once a week.

+ Samba is quite often in the devices, too, though.

# The Era of GPL Litigation

+ Lawsuits have become undeniably necessary.

+ Only used as the *very* last resort.

+ Focus is to settle:
     - What we want more than anything else is full compliance &hellip;
     - &hellip; on *all* GPL'd and LGPL'd components &hellip;
     - &hellip; judge is unlikely to grant us all that &hellip;
     - &hellip; so we work hard to settle on that request &hellip;
     - &hellip; taking extra money &amp; injunctions only as a consolation prize.

# Constant Vigilance!

<img align="right" src="moody.jpg"/>

+ GPL Violations *are* *everywhere*.

+ My only recourse is &hellip;
     - Constant Vigilance!

+ BTW, I'll take an even money bet for (almost) any amount:
     - Give me an hour and an Internet connection &hellip;
     - &amp; I'll find you a GPL-violating embedded firmware I've never seen before.

# More Info / Talk License

+ Some URLs:
     - Conservancy Website: http://sfconservancy.org/
     - My blog: ebb.org/bkuhn/blog
     - Personal Microblog: @bkuhn (on identi.ca)
     - Conservancy Microblog: @conservancy
     - FSF Licensing/Compliance Site: http://www.fsf.org/licensing
     - Slides source at: https://gitorious.org/bkuhn-small-hacks/talks

This talk and the slides are:
Copyright &copy; 2008, 2009, 2010, 2011 Bradley M. Kuhn.

<img src="cc-by-sa-3-0_88x31.png"/>
<a href="http://creativecommons.org/licenses/by-sa/3.0/us/">This presentation and these slides are licensed under a <a href="http://creativecommons.org/licenses/by-sa/3.0/us/">Creative Commons Attribution-Share Alike 3.0 United States License</a>.
            
