% Demystifying GPL Enforcement: Using the Law To Uphold Copyleft
% Bradley M. Kuhn
% Saturday 20 February 2010

# Who I Am?

+ Currently: President of Software Freedom Conservancy, which is:
     - ... non-profit home of BusyBox project.
     - ... Erik Andersen's & BusyBox's designated GPL enforcement agent.

+ Currently: on Board of Directors of the FSF

+ Previously: employee of SFLC
     - SFLC are the lawyers for Andersen and Conservancy.

+ Previously: Executive Director of FSF
     - Started and ran the GPL Compliance Labs, 2001-2005.

+ Before That: Volunteer / Part Time for FSF
     - Did GPL Compliance Engineering work, 1999-2001

# GPL Compliance

+ Not a new topic.

+ FUD machine makes it seem mysterious.

+ Let's clear up misconceptions.

# The Clueful: Constant Vigilance!

<img src="moody.jpg" align="right"  />

+ Made plan when incorporating FLOSS.

+ Changed the software development practices.

# What the Clueful Do

+ Planned best practices to avoid violation.

+ Realize GPL software is here to stay.

+ Design development, integration and acquisition to pre-handle it.

# Compliance-Friendly Development

+ Use revision control ...
    - ... to pull in vendor branch.
    - ... to tag releases.

+ Avoid "Build Guru" ...
    - ... by documenting build process.
    - ... and versioning it, too.

+ Use Fossology!
    - http://fossology.org/

# Why Is Compliance Necessary?

+ Binaries are modified versions of source.

+ Modification controlled by copyright, thus by GPL.

+ This separation is where nearly all violations occur.

***

> After all, what is binary distribution of software but a rudimentary form of DRM?

<p align=right>
--  Richard Fontana, during the GPLv3 process
</p>

# GPL Binary Requirements

(v2 &sect; 3, v3 &sect; 6)

+ Four options:
    - Source alongside binary (v2/v3).
    - Offer for source (v2/v3).
    - Internet side-by-side distribution (v3).
    - Torrent distribution (v3).

# Source Alongside Binary

+ Simplest option

+ **Obligations end at distribution time.**

+ Physical media required.

# Offer For Source

+ Useful if not shipping CD already.

+ Lasts three years.

+ Mail fulfillment required (not in v3).

# Side-By-Side Distribution

+ Not in GPLv2, pedantically speaking.

+ Always been considered compliant for v2.

+ v3 clarifies this.

# Peer-to-Peer Distribution 

+ v2 obviously couldn't consider this.

+ v3 allows distribution of equally seeded source and binary.

# Preparing Corresponding Source

(v2 &sect; 3, v3 &sect; 1)

+ Make sure all sources are present.
     - revision system helps a lot here.

+ Build scripts
     - rule of thumb:
     - make sure someone skilled in art can build it.

# Termination

<img width="450" height="250" src="daleks.jpg" align="right"  />


(v2 &sect; 4, v3 &sect; 8)

+ v2 is automatic and permanent.

+ v3 has auto-reinstatement.
    - 60 day self-correction timeout.
    - 30 day penalty-less after notice.

+ Usually, you need copyright holder to reinstate.

#  What Enforcers Do First

+ Send a Letter, carefully finding right person.

+ Communication is key.

+ Ask for the Standard Requests.

# Standard Requests to Expect

+ Compliance on all FLOSS copyrights.

+ Notification to past recipients.

+ Appoint GPL Compliance Officer.

+ Periodic compliance reports.

+ Yes, we do ask for some money.

# Money

+ No one in non-profits is getting rich from this.

+ Who should pay for enforcement: 
     - Compilers or Violators?
     - Individual donors.

+ There must be some deterrent.

+ Non-profit enforcement == accountability.

+ Confidentiality is something violators ask for.

# Lawsuits

+ Only bring lawsuits against people who don't communicate or take process seriously.

+ It's always the last resort.

+ Lawsuits are not the "scary" things people make them out to be.
 
# GPL Enforcement Clarifies Community

+ Avoid two sets of rules: participators vs. the ignorant.

+ Either coplyeft matters, or we should all switch to Apache-2.0.

+ Every GPL violator is a new potential contributor.

+ Shows that the rules are meaningful.

# The Upstream Problem

<img align=left src="michael-scott.jpg"/>

When I said that I was king of forwards, you got to understand that I
don't come up with this stuff. I just forward it along. You wouldn't
arrest a guy who was just passing drugs from one guy to another.

<p align=right>
 -- Michael Scott, *The Office* 
</p>

# Don't be Michael Scott

<img height=250 width=250 align=right src="michael-scott.jpg"/>

+ A repackager is a distributor, just like supplier is.

+ Repakager shares the same obligations.

+ Should ask due diligence questions *before* buying.

+ Suppliers should be asked to teach downstream to comply.

+ Repackagers should be indemnified!

# Derivative Works Discussion?

+ Truth is, it rarely comes up in GPL enforcement.

+ Never has a violator in our experience disputed our interpretation.

+ Uses are primarily mundane; lines are clear.

+ Anyway, in complicated cases ...
    - ... a seasoned software copyright lawyer should study the facts.
    - ... such modifiers are already extremely sophisticated, anyway.

# Follow / License 

+ Conservancy Website: http://sfconservancy.org/

+ My blog: ebb.org/bkuhn/blog

+ Personal Identica: @bkuhn

This talk and the slides are

Copyright &copy; 2008, 2009, 2010, 2011 Bradley M. Kuhn.

<img src="cc-by-sa-3-0_88x31.png"/>
<a href="http://creativecommons.org/licenses/by-sa/3.0/us/">This presentation and these slides are licensed under a <a href="http://creativecommons.org/licenses/by-sa/3.0/us/">Creative Commons Attribution-Share Alike 3.0 United States License</a>.
            
