% A Beautiful Build: Releasing Linux Source Correctly
% Bradley M. Kuhn
% Monday 5 October 2015

# What Does Conservancy Do?

+ Software Freedom Conservancy is a charity based in the USA.
     + That means we're legally required to operate in the public good.
     + Contrast: a trade association, like LF, whose charge is to operate in
       a manner that advances common business interests of an industry.

+ Conservancy provides essential non-software-development work that Open
  Source and Free Software projects needs.

+ This includes helping projects ensure their software licenses continue to
  benefit the public.
     + which in concrete terms means acting to verify projects' FLOSS
       licenses meet goals their policy.
  
# Background

+ My first few slides point may be too remedial for some of you.
     + If so, take a 2 minute email break.


# The Copyleft

+ Linux and much Open Source and Free Software  use **copyleft** licenses.
    + The GNU General Public License (GPL) is the most common one.

+ Copyleft, simply, seeks to give downstream users the means and capacity to
  generate and utilize binaries in the same manner that upstream did.
    + Even after modifying sources.

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

+ Nevertheless, enforcement pursues the  second goal indirectly.

+ GPL compliance is usually *not* about what to do upstream.

+ GPL is a license made for the users, not the developers.

+ The main policy goal:
     + Ensure the user can exercise the freedom to modify the software &hellip;
     + &hellip; in a manner that's allows real world, not theoretical 

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

# A Pristine Example

+ Enforcement must often use a &ldquo;know it when I see it&rdquo; standard.
    + i.e., can we take your CCS build it, and install it?

+ We've reached compliant CCS with hundreds of companies:
    + but that didn't mean the CCS was pretty.

+ Thanks to ThinkPenguin, we finally have an example of beautiful embedded
  product compliance. 

# Lessons Learned from Pristine Example

+ The full paper for this talk is available online:
    + [compliance.guide/pristine-example](http://compliance.guide/pristine-example)


+ It's part of a larger tutorial called [*Copyleft and the GNU General
  Public License: A Comprehensive Tutorial and Guide*](https://copyleft.org/guide/)
  at copyleft.org.

+ The Guide, as we call it, contains over 150 pages of tutorials materials
  about how copyleft works and why copyleft licenses are written the way they
  are.

+ For the remainder of this talk, I'll give you the highlights of good
  compliance lessons the pristine example shows.

# Avoid the offer for source.

+ Lawyers love the offer for source.
    + I don't think they are good lawyers if they do.

+ The offer creates ongoing obligations.

<hr/>

> Accompany [executable form] with a written offer, valid for at least three
> ears, to give any third party, for a charge no more than your cost of
> physically performing source distribution, a complete machine-readable copy
> of the corresponding source code &hellip; on a medium customarily used for software
> interchange

<p align=right>
&mdash; GPLv2&sect;3
</p>
</span>

# Avoid the offer for source.

+ Often, an offer for sources telegraphs that compliance wasn't done.

+ If you must use the offer, assume it'll be requested on product launch day.

<hr/>

> Accompany [executable form] with a written offer, valid for at least three
> ears, to give any third party, for a charge no more than your cost of
> physically performing source distribution, a complete machine-readable copy
> of the corresponding source code &hellip; on a medium customarily used for software
> interchange

<p align=right>
&mdash; GPLv2&sect;3
</p>
</span>

# Give a roadmap in a README

+ Scripts doesn't only mean shell scripts and Makefiles.

+ Think of the script of a play or movie. 

+ If your build process includes human intervention &hellip;

+ &hellip; then the script are a written explanation of what the human must
do.

<hr>
> **the scripts** used to control compilation and installation of the executable.

<p align=right>
&mdash; GPLv2&sect;3
</p>
</span>

# ThinkPengiun's README

A file called “README” at the top-level directory said:

    In order to build firmware images for your router, the following needs to be installed:

    gcc, binutils, bzip2, flex, python, perl, make, find, grep, diff, unzip,
    gawk, getopt, libz-dev and libc headers.

    Please use “make menuconfig” to configure your appreciated configuration
    for the toolchain and firmware. Please note that the default configuration
    is what was used to build the firmware image for your router. It is advised
    that you use this configuration.

    Simply running “make” will build your firmware. The build system will
    download all sources, build the cross-compile toolchain, the kernel and all
    chosen applications.

     To build your own firmware you need to have access to a GNU/Linux system
     (case-sensitive filesystem required).

# Make Sure It Builds

+ Can your CCS pass this test?
    + Give you source release to another developer from another department.
    + Ask them to follow the instructions you wrote.
    + They should get the equivalent binaries you get in building.

+ Very few organizations bother to do this.

+ It's probably the most useful step to verify compliance, yet *no*
  compliance process recommendations I've ever seen include this.

<hr>
> the scripts used to **control compilation** and installation of the executable.

<p align=right>
&mdash; GPLv2&sect;3
</p>
</span>


# Toolchain?

+ The toolchain is rarely considered mandatory as part of &ldquo;the
  scripts&rdquo;.

+ Admittedly, it doesn't *control* compilation, it *is* complication.

+ The script here is explaining precisely what type of toolchain is needed.

+ Something like: &ldquo;GCC vX built with the following ./configure
  line&rdquo; is usually adequate.

+ But including the toolchain is a nice step to make it easy for your users.

<hr>
> the scripts used to **control compilation** and installation of the executable.

<p align=right>
&mdash; GPLv2&sect;3
</p>
</span>

# It's not &ldquo;make install&rdquo;

+ Server system software can offer a &ldquo;make install&rdquo; that
  reasonable works to meet installation requirements.

+ Embedded products are admittedly difficult to install.

+ To comply here, you'll usually just have write out the instructions.

+ It is required; don't skip this part.

<hr>
> the scripts used to **control** compilation and **installation** of the executable.
<p align=right>
&mdash; GPLv2&sect;3
</p>
</span>

# Missing hardware components

+ Inclusion of specialized installation hardware is not a
  &ldquo;script&rdquo;.

+ In our ThinkPenguin example, we had to go buy a USB serial adapter to
  install the modified firmware.

+ Just tell the user what they have to go buy for the install to work.

# Summary

+ The GPL requires that the users can replace the copylefted binaries in your
  embedded product with binaries they build.

+ The host system matters; just tell everyone what host system you use.
  (&amp; don't be ashamed at how old it is.)

+ Explain details of the toolchain used.  Including it would be nice, but
  ensure its compliance too.

+ Have a colleague not working on the project test the build and
  installation.

# More Info / Talk License

<img align="right" src="cc-by-sa-4-0_88x31.png" />

+ URLs / Social Networking / Email:
     - Pls. support Conservancy: [sfconservancy.org/supporter/](https://sfconservancy.org/supporter/)
     - If you hold copyrights in Linux, Debian, Samba, or BusyBox, you can
       join our enforcement coalition.  [Contact us!](https://sfconservancy.org/linux-compliance/about.html)
     - [*The Guide*](https://copyleft.org/guide) is available &amp; [welcomes contributions at copyleft.org](https://copyleft.org).
     - Conservancy: [sfconservancy.org](https://sfconservancy.org/) &amp; [@conservancy](https://twitter.com/conservancy/).
     - Me: [faif.us](http://faif.us) &amp; [ebb.org/bkuhn](http://ebb.org/bkuhn)
     - Slides: [ebb.org/bkuhn/talks](http://ebb.org/bkuhn/talks/ELC-2015/pristine-example.html).

<span class="fitonslide">
<p>Presentation and slides are: Copyright &copy; 2015 Bradley M. Kuhn, and are licensed under the <a rel="license" href="https://creativecommons.org/licenses/by-sa/4.0/legalcode">Creative Commons Attribution-Share Alike 4.0 International License</a>. </p>
</span>


<!--  LocalWords:  CCS ldquo rdquo img src jpg Codebase Bitbucket GitHub hg
 -->
<!--  LocalWords:  Phabricator GitLab Mercurial's relicenses RhodeCode vader
 -->
<!--  LocalWords:  RhodeCode's GmbH codebase GPL'd un relicense fitonslide
 -->
<!--  LocalWords:  mdash GPLv USL BSDi br CSS Rebrand Kiilerich Shadura fc
 -->
<!--  LocalWords:  Kallithea changeset cd bb Marcin Kuzminski Sep cwd af eab
 -->
<!--  LocalWords:  rhodecode init py config lsquo rsquo sed perl rst ci mani
 -->
<!--  LocalWords:  paster xargs kallithea websetup ga captcha stylify url js
 -->
<!--  LocalWords:  metatags gravatar uri tmpl Javascript ffd codemirror ef
 -->
<!--  LocalWords:  loadmode qgraph mergerly pyroutes CodeMirror sha fd cbf
 -->
<!--  LocalWords:  ee css whitespace md Marijn Haverbeke txt Codemirror's ln
 -->
<!--  LocalWords:  minified bytecode YUI yui hudson JumpToPageDropDown tmp
 -->
<!--  LocalWords:  dom dragdrop datasource autocomplete json datatable html
 -->
<!--  LocalWords:  paginator deploybuild Kallithea's
 -->
