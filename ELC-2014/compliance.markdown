% Collaborative GPL Enforcement Through Non-Profit Entities
% Bradley M. Kuhn
% Thursday 1 May 2014

# My History

+ Worked my first GPL enforcement case in 1999 (as FSF volunteer).

+ Started working for FSF in 2000 (was there until 2005).

+ Now: President &amp; Distinguished Technologist of Software Freedom Conservancy &amp; on Board of Directors of the FSF.

+ Plurality of my time since 1999 has been spent on GPL enforcement.
     + I'm probably the person most &ldquo;responsible&rdquo; for every major USA GPL enforcement action.

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

+ Copyright holders must use copyright enforcement:n
     + &hellip; but for a *good* cause: the four freedoms.
     + &ldquo;using the tools of the oppressor against the oppressor&rdquo;

# Complexity of Modern Enforcement

+ Not all GPL enforcers are created equal anymore.

+ Oracle, after all, holds MySQL's copyrights now &amp; enforces.
     + I'd call this the corrupt version of what I do.

+ Compliance must be paramount &hellip;
     + &hellip; over all other interests.
     + This has been called &ldquo;community enforcement&rdquo;.
     + What's that mean?

# Community Enforcement

+ All community enforcement follows this rote procedure:
     + Receive a violation report from an end-user.
     + Verify it's really is a violation.
     + Send a letter to the violator.
     + CCS-Ask: Ask the violator to submit CCS candidates
     + Review and provide feedback on CCS.
     + If CCS has issues, goto CCS-Ask.
     + Ask violator to inform past customers.
     + Ask violator to cover reasonably hourly cost of this work.
     + Restore copyright permissions.

+ Let's talk about the money issue first.

# Money

+ No community enforcer is getting rich from this.

+ 501(c)(3) non-profit charity enforcement == accountability.
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
     + &hellip; but only after a year or more of ongoing violation.
     + &hellip; and only after many warnings about compliance progress stymied.

+ Companies switching away from GPL'd software.
     + We *all* want them to use: just in compliance

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

+ After years of complex negotiation, and many CCS &ldquo;rounds&rdquo;

+ All CCS works (only two proprietary Linux modules held back).

+ The first check-in of the OpenWRT is this CCS release.

+ OpenWRT project leaders to this day credit this as their start.
      + Source: <a href="http://twit.tv/show/floss-weekly/265">Gregers Petersen on FLOSS Weekly Episode 265</a>
        
+ OpenWRT blossomed into *the* key replacement firmware for most wireless routers.

# GPL-violations.org

<img align=right src="harald-welte.jpg"/>

+ FSF was initially shy about lawsuits.

+ Harald participated with FSF in WRT54G matter.
     + But Harald disagreed with FSF's early 2000s &ldquo;no litigation&rdquo; strategy.
     + (in hindsight, Harald was right).

+ launches multiple lawsuits in Germany (about 8 between 2005-2008).

+ Quite successful.

# Embedded Violations Prevalent

+ Erik Andersen becomes exasperated by mid-2006.
     - post-WRT54G: router &amp; NAS market is a violation haven.

+ Erik asks for help.

+ Conservancy becomes his enforcement agent (&amp; receive some others' &copy; assignment)

+ Conservancy has had > 100 GPL violations queued for action since 2007.
     - Conservancy's list is now > 300

# Why Do Violations Happen?

+ Compliance actually isn't difficult.
     - &amp; compliance problems are easily remedied.

+ So, why are there so many violations?

# The Upstream Problem

<img align=left src="michael-scott.jpg"/>

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

+ Make sure the suppliers' base system builds/installs from sources.
     + Consider using Yocto (automated tools to help w/ compliance)
     + it's better engineering to have reproducible builds anyway.
     + Convince your bosses the build/install process isn't their value add.

+ Just put that CCS online &amp; put URL in the manual.
     + No, GPLv2 doesn't require this!
     + But, I don't want to test your offers for source.
     + Your fulfillment department *will* screw this up.

+ If possible, help select the supplier.
     + Ask the supplier up front about CCS.
     + Demand legal indemnity from your upstream!

+ Join Conservancy's Coalition.
     + Now, the coalition's history:

# Historical BusyBox Enforcement

+ Erik Andersen rewrote BusyBox from scratch (starting 2001).

+ BusyBox slowly but surely became standard userspace for embedded systems.

+ Linux plus BusyBox:
     + Standard for embedded systems.
     + Usually out of compliance.

# Just Look Busy!

+ The <a href="https://lwn.net/Articles/478308/">Tempest in a Toybox</a>.

+ BusyBox enforcement was de-facto Linux enforcement.
     + BusyBox copyright holders (Conservancy and Andersen) asked for comprehensive GPL compliance.
     + Some Linux developers felt this was unfair&hellip;
     + &hellip;but Linux developers appeared to be supportive.
<hr/>

> Busybox is arguably the most litigated piece of GPL software in the world.  &hellip; Litigants have sometimes requested remedies outside the scope of busybox itself&hellip;

<span class="fitonslide">
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

# Matthew Garrett, Linux's Freedom Fighter

+ For years, Matthew had asked me to help him enforce the GPL on Linux.

+ I'd told him that as it stood, it was easier to just work based on BusyBox.

+ After so much had change, it made sense to simply engage directly on behalf
  of Linux developers.

+ <a href="http://sfconservancy.org/news/2012/may/29/compliance/">On
  2012-05-29, GPL Compliance Project for Linux Developers</a> gives structure
  to Linux compliance activity.

# Why Special Case Linux?

+ Linux violations are rampant.

+ Denys asked us to engage.

+ Also, various Linux developers &hellip;
     - &hellip; like Matthew Garrett &hellip;
     - &hellip; had bugged Conservancy for years to help with enforcement.

+ GPL Compliance Project for Linux Developers gives structure to Linux compliance activity.

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
