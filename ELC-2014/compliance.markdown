% Collaborative GPL Enforcement Through Non-Profit Entities
% Bradley M. Kuhn
% Thursday 1 May 2014

# My History

+ Worked my first GPL enforcement case in 1999 (as FSF volunteer).

+ Started working for FSF in 2000 (was there until 2005).

+ Now: President &amp; Distinguished Technologist of Software Freedom Conservancy &amp; on Board of Directors of the FSF.

+ Both FSF and Conservancy have extensive GPL enforcement programs:
     + so, the plurality of my time since 1999 has been spent on GPL enforcement.

# How GPL Works (Theoretically)

+ Copyright: the internationalized standard for authors' controls over works.

+ Use copyright license to grant permission.

+ Make permission conditional on giving your downstream the four freedoms.

+ This is the copyright law hack of copyleft.

+ Copyright rules require compliance with the license.

# How GPL Works (In Reality)

<img src="copyleft-irl.jpg" align="right"  />

+ What do you do when someone violates?
     + (and social pressure for compliance fails)?

+ Violation of the license means lost rights for distribution.
     + See GPLv2&sect;4 &amp; GPLv3&sect;8
     + Further distribution thereafter (even in compliance) is copyright infringement.

+ Copyright holders must use copyright enforcement:
     + &hellip; but for a *good* cause: the four freedoms.

# Complexity of Modern Enforcement

+ Not all GPL enforcement is software-freedom-motivated.

+ Oracle, after all, holds MySQL's copyrights now &amp; enforces.
     + I call this the corrupt version of what I do.

+ Compliance must be paramount &hellip;
     + &hellip; over all other interests.
     + Some call this &ldquo;community enforcement&rdquo;.
     + What's that mean?

# Who Reports Violations to Community Enforcers?

+ Who reports violations?: Individual users.

+ The user buys buy embedded products &hellip;
     + &hellip; (such as a TV, DVD Player, wireless router, mobile phone) &hellip;
     + &hellip; user tries to get the GPL'd sources and build them &hellip;
     + &hellip; and it doesn't work.

+ Conservancy gets a new report like this weekly.

# Community Enforcement

+ All community enforcement follows this rote procedure:
     + Receive a violation report from an end-user.
     + Verify it's really a violation.
     + Send a letter to the violator.
     + CCS-Ask: Ask the violator to submit CCS candidates
     + Review and provide feedback on CCS.
     + If we know why CCS doesn't work, give patches to violator.
     + If CCS still has issues, goto CCS-Ask.
     + Ask violator to inform past customers.
     + Ask violator to cover reasonable hourly cost of this work.
     + Restore copyright permissions.

+ Let's talk about the money issue first.

# Money

+ No community enforcer is getting rich.
     - 501(c)(3) non-profit charity enforcement == accountability.
     - On a Form 990, you can look up: &hellip;
     - &hellip; how much Conservancy  spends on / receives from enforcement.
     - &hellip; my annual salary &amp; compensation.
     - <a href="https://sfconservancy.org/about/filings/">https://sfconservancy.org/about/filings/</a>

+ Anyway, who should pay for enforcement:
     - Those who *comply* or those who *violate*?
     - Individual donors to non-profits?

+ There must be a deterrent.

+ Confidentiality is something violators ask for.

# What Conservancy Strives to Avoid

+ Junking products (that's bad for the environment).

+ Injunctions:
     + We've gotten them &hellip;
     + &hellip; but only after a year or more of ongoing violation &hellip;
     + &hellip; &amp; only after (a) many warnings to the violator, &amp;
     + &hellip; (b) explicitly warning the violator that's our plan.

+ Companies switching away from GPL'd software.
     + We *all* want them to use: just in compliance

+ Lawsuits of any kind:
     + suing someone is always a last resort &hellip;
     + &hellip; usually after years &amp; hundreds of hours of begging them to comply. 

# What's CCS?

+ The point of GPL is not merely to examine the source.

+ GPLv2 requires what it calls &ldquo;complete, corresponding source&rdquo;: CCS

+ The freedom to modify requires, as GPLv2 says:
    + &ldquo;the scripts used to control compilation and installation of the executable&rdquo;

+ CCS check: verify these scripts actually do compile and install the executable.

+ For embedded systems, this is not always easy.

+ But, why is it important?

# Coalition of the Willing

<img align=right src="wrt54g.png"/>

+ Spring 2003: dozens of reports on WRT54G.

+ Discussions begin with Cisco (who'd bought Linksys just weeks before)

+ Story hits slashdot on 2003-06-08

+ FSF puts together group to do enforcement.
     - key members: Erik Andersen (BusyBox) &amp; Harald Welte (Linux)

# WRT54G Begat OpenWRT

<img align=right src="wrt54g.png"/>

+ After years of complex negotiation, and many CCS &ldquo;rounds&rdquo;:
      + All CCS works (only two proprietary Linux modules held back).
      + First check-in of OpenWRT is that CCS release.

+ OpenWRT project leaders to this day credit this as their start.
      + Source: <a href="http://twit.tv/show/floss-weekly/265">Gregers Petersen on FLOSS Weekly Episode 265</a>
        
+ OpenWRT blossomed into *the* key replacement firmware for most wireless routers.

# GPL-violations.org

<img align=right src="harald-welte.jpg"/>

+ FSF was initially shy about lawsuits.

+ Harald participated with FSF in WRT54G matter.
     + But Harald disagreed with FSF's early 2000s &ldquo;no litigation&rdquo; strategy.
     + (in hindsight, Harald was right).

+ Launches multiple lawsuits in Germany (about 8 between 2005-2008).

+ Quite successful, but gpl-violations.org is now mostly defunct.
     + except for running the mailing lists.

# Embedded Violations Prevalent

+ Erik Andersen becomes exasperated by mid-2006.
     - post-WRT54G: router &amp; NAS market is a violation haven.

+ Erik asks for help.

+ Conservancy becomes his enforcement agent (&amp; receives some others' &copy; assignment)

+ Conservancy has had > 100 GPL violations queued for action since 2007.
     - Conservancy's list is now > 300

+ Conservancy's work in BusyBox enforcement *has* made a real difference.
     - both to BusyBox and Linux compliance.

# Samsung: A Success Story

+ Samsung has violated the GPL before.
     + Conservancy even had to sue them over TV products.

+ Conservancy settled &amp; the final CCS was really good!
     + That CCS launched <a href="http://www.samygo.tv/">SamyGo project</a>.

+ More recently, <a href="http://sfconservancy.org/news/2013/aug/16/exfat-samsung/">Conservancy helped Samsung fix</a> their <a href="https://gitorious.org/binbang/exfat-linux">exFAT module</a> violation.

# Why Do Violations Happen?

+ As Samsung now knows:

+ Compliance actually isn't difficult.
     - &amp; compliance problems are easily remedied.

+ So, why are there so many violations?

# The Upstream Problem

<img align="right" src="michael-scott.jpg"/>

When I said that I was king of forwards, you got to understand that I
don't come up with this stuff. I just forward it along. You wouldn't
arrest a guy who was just passing drugs from one guy to another.

<p align="right">
 &mdash; Michael Scott, *The Office* (USA Version)
</p>

# Suppliers Bully OEMs, AFAICT

+ I'd be the worst police officer in the world.

+ No one ever turns &ldquo;states' evidence&rdquo;
     - &hellip; at least they don't for _me_, anyway.

+ Me: &ldquo;Please, just tell me on the record your supplier violated when distributing to you.&rdquo;

+ Them: &ldquo;We'll work with our upstream to get into compliance.&rdquo;

# What Can You Do About This?

<img align="center" src="Smoky_The_Nanobot.jpg"/>

# What Can You Do About This? (0)

+ Make sure the suppliers' base system builds/installs from sources.
     + Consider using Yocto (automated tools to help w/ compliance)
     + It's better engineering to have reproducible builds anyway.
     + Convince your bosses the build/install process isn't their value add.

# What Can You Do About This? (1)

+ Just put that CCS online &amp; put URL in the manual.
     + No, GPLv2 doesn't require this!
     + But, I don't want to test your offers for source.
     + Your fulfillment department *will* screw this up.

# What Can You Do About This? (2)

+ If possible, help select the supplier.
     + Ask the supplier up front about CCS.
     + Demand legal indemnity from your upstream!

# What Can You Do About This? (3)

+ But, most importantly:

+ Please join Conservancy's Coalition.

+ For context, a bit of the coalition's history:

# Historical BusyBox Enforcement

+ Erik Andersen rewrote BusyBox from scratch (starting 2001).

+ BusyBox slowly but surely became standard userspace for embedded systems.

+ Linux plus BusyBox:
     + Standard for embedded systems.
     + Usually out of compliance.

# Just Look Busy!

+ BusyBox enforcement was de-facto for Linux.
     + The <a href="https://lwn.net/Articles/478308/">Tempest in a Toybox</a>.
     + BusyBox copyright holders request comprehensive GPL compliance.
     + Some Linux developers felt this was unfair&hellip;
     + &hellip;but other Linux developers supported it.
     + (i.e., community was already split on this question.)
<hr/>

<span class="fitonslide">
> Busybox is arguably the most litigated piece of GPL software in the world.  &hellip; Litigants have sometimes requested remedies outside the scope of busybox itself&hellip;

<p align=right>
 &mdash; <a href="http://www.elinux.org/Busybox_replacement_project">Tim Bird
 of Sony Corporation</a>, <a href="http://www.elinux.org/index.php?title=Busybox_replacement_project&action=history">in
 January 2012</a>.
</p>
</span>
 
# Denys, The Voice of Reason

<img src="denys-vlasenko-scaled.jpg" align="right"  />

+ Current BusyBox maintainer has that special skill of Free Software developers &hellip;
      + &hellip; to find the sane arguments hidden among troll-ish attacks.

+ I walk through Brussels on the phone with Denys &hellip;
      + &hellip; the day before FOSDEM 2012 &hellip;
      + &hellip; and he convinces me:

+ To continue with enforcement, Linux developers must be involved.

# Garrett, Linux's Freedom Fighter

+ For years, Matthew Garrett had asked me to help him enforce the GPL on Linux.

+ I'd told him that as it stood, it was easier to just work based on BusyBox.

+ After so much had changed, it made sense to simply engage directly on behalf
  of Linux developers.
      + &amp; there were many others who felt the same as Matthew did.

+ GPL Compliance Project for Linux Developers gives structure to Linux
  compliance activity.

# Expanding the Coalition

+ <a href="http://sfconservancy.org/news/2012/may/29/compliance/">On
  2012-05-29, Conservancy announced expanded GPL enforcement efforts</a>.

+ Conservancy now actively enforces GPL for:
     + BusyBox, Linux, Samba, Mercurial

+ Linux is not a full Conservancy member project:
     + Conservancy enforces for a coalition of about a dozen prominent copyright holders.
     + Matthew Garrett &amp; David Woodhouse are the most public.
     + We expect to offer this service to more projects.

# The Great Queue

+ We're aware of hundreds of embedded Linux GPL violations.
     + Each one takes 40-100 hours of work to resolve.
     + Over a period of usually 3-6 months.

+ The CCS issue is the most difficult:
     + CCS candidates just don't build.

+ But, we're facing a worse problem everywhere.

# Linux's GPL Elephant

<img src="elephant-in-the-room_400x415.jpg" align="right"  />

+ I used to avoid the elephant, but now it's *the* central issue of compliance.

# Linux's GPL Elephant

<img src="elephant-in-the-room_400x415.jpg" align="right"  />

+ Much debated: Are Linux modules derivative works of Linux?
      + I &amp; our lawyers believe they almost always are.
      + Many corporate lawyers disagree.

+ Case law is limited:
      + Both sides believe they're correct.
      + No general rule: the actual facts of a specific situation always matter.
      + This is the exact type of issue that becomes a big court case.

+ My political opponents call this: &ldquo;the ground war of GPL&rdquo;
      + Maybe it's time for that ground war.

# Biggest Way You Can Help

<img align="right" src="smokey-says-only-you-can-prevent-forest-fires.jpg"/>

+ You're all embedded Linux developers.
     + That means it's likely your copyrighted work that violators infringe.
     + Only *you* can help your users.

+ OTOH, maybe you don't care about the GPL or the freedoms it protects.
     + &amp; I don't blame you if you don't care &hellip;
     + &hellip; you aren't required to agree with strong copyleft to be a Linux contributor.

+ But, if you *do* care, you can join our coalition:
     + If you want to join the GPL Compliance Project for Linux Developers &hellip;
     + &hellip; see me after the talk; I have blank forms with me. :)

# More Info / Talk License

+ URLs / Social Networking / Email:
     - Sign Up Today as part of the <a href="https://sfconservancy.org/linux-compliance/">*GPL Compliance Project for Linux Developers*</a>.
     - A Book I helped write: <a
        href="http://ebb.org/bkuhn/writings/comprehensive-gpl-guide.pdf">*Copyleft and
        the GNU General Public License: A Comprehensive Tutorial*</a> is available.
     - Conservancy: sfconservancy.org &amp; @conservancy
     - Me: faif.us &amp; ebb.org/bkuhn
     - Slides: ebb.org/bkuhn/talks &amp; gitorious.org/bkuhn/talks (source)
     - DONATE: https://sfconservancy.org/donate/

<span class="fitonslide">
<p>Presentation and slides are: Copyright &copy; 2014 Bradley M. Kuhn, and are licensed under the <a href="http://creativecommons.org/licenses/by-sa/3.0/usa/">Creative Commons Attribution-Share Alike (CC-By-SA) 3.0 United States License</a>. <img src="cc-by-sa-3-0_88x31.png"/></p>
<p>Some images included herein are &copy;'ed by others. I believe my use of those images is fair use under USA &copy; law.  However, I suggest you remove such images if you redistribute these slides under CC-By-SA-USA 3.0.
</p>
</span>

<!--  LocalWords:  GPLv MySQL's ldquo rdquo CCS goto href GPL'd img src wrt
 -->
<!--  LocalWords:  png Linksys slashdot BusyBox Harald Welte OpenWRT Gregers
 -->
<!--  LocalWords:  harald welte jpg NAS michael scott mdash OEMs AFAICT de
 -->
<!--  LocalWords:  Yocto userspace facto Toybox Busybox busybox fitonslide
 -->
<!--  LocalWords:  Denys denys vlasenko ish FOSDEM Linux's Woodhouse faif sa
 -->
<!--  LocalWords:  sfconservancy
 -->
