% Why GPL Enforcement Is Essential to OpenWrt's Past and Future 
% Bradley M. Kuhn
% Thursday 13 October 2016

# Slides Links

+ Some of the slides have links to various articles.

+ I don't mind at all if you would rather read those than listen to me
  further. :)

+ [ebb.org/bkuhn/talks/OpenWRT-2016/gpl.html](http://ebb.org/bkuhn/talks/OpenWRT-2016/gpl.html),
  or via url shortener at [ur1.ca/pvrdi](http://ur1.ca/pvrdi)

+ [Source code of slides is available](https://github.com/bkuhn/talks/tree/master/OpenWRT-2016).  I'm sure to have typos; please
  submit patches there rather than calling them. :)

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
<span class="fitonslide">

> Copyleft is a strategy of utilizing copyright law to pursue the policy goal
> of fostering &amp; encouraging the equal &amp; inalienable right to copy,
> share, modify &amp; improve creative works of authorship. Copyleft &hellip;
> describes any method that utilizes the copyright system to achieve the
> aforementioned goal. Copyleft as a concept is usually implemented in the
> details of a specific copyright license &hellip; Copyright holders of
> creative work can unilaterally implement these licenses for their own works
> to build communities that collaboratively share &amp; improve those
> copylefted creative works.

<p align=right> &mdash; Definition of copyleft from
[copyleft.org](https://copyleft.org/) </p> </span>

# It's Not Magic 

<img src="Pixie_Dust.png" width="50%" height="50%" align="right"  />

Copyleft is *not* magic pixie dust.


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

# How This Relates to OpenWrt

+ OpenWrt may be the most successful historical example of GPL enforcement.

+ The project began as the outcome of GPL enforcement action.

# Where It All Began

<img align=right src="wrt54g.png"/>

+ Spring 2003: dozens of reports on WRT54G.

+ Discussions begin with Cisco (who'd bought Linksys just weeks before)

+ Story hits slashdot on 2003-06-08

+ FSF (where I used to work) put together group to do enforcement.
     - key members: Erik Andersen (BusyBox) &amp; Harald Welte (Linux)

# First, the End of the Story

<img align=right src="openwrt-history-page.png"/>

+ WRT54G source is released (but wireless driver kept proprietary).

+ SVN check-in r1 of the OpenWrt project was the actual source code we
  reviewed in our GPL compliance efforts.

# How We Got There

+ Cisco had just purchased Linksys.
      + Cisco was actually surprised that any Free Software was in Linksys devices.
      + Linksys had no plan for GPL compliance.

+ After months of negotiation, Linksys admitted the build came from Broadcom.

+ Please note: Broadcom was a different company, and led by different people
  then.

# Dealing With Broadcom

+ On Monday 13 October 2003, Broadcom brought most of their executive team to
  meet with us.

+ Their primary request: don't push on the wireless driver issue, for fear
  of an FCC fight, and in return they will comply with GPL.

+ The coalition of copyright holders enforcing the GPL in this case made that deal.

# Was It the Right Deal?

<img align=right height="333" width="333" src="dr-who-timey.jpg"/>


+ I've often wondered if we made the right deal.

+ But I doubt I'd go back and change it, because the birth of OpenWrt was too
  important to mess with.

+ &hellip; &amp; besides, I am convinced time-travel into the past is
  impossible.

# Culture of Enforcement-Born Projects

+ More than any other project, I believe OpenWrt/LE DE culture has GPL
  enforcement as part any other project.

+ OpenWrt/LEDE developers have a healthy distrust of any proprietary component,
  particularly proprietary device drivers.

+ Developers are not afraid to confront companies who make proprietary
drivers &hellip;

+ &hellip; &amp; laud companies who change their behavior and get GPL
  compliance right:
     + (cf: ath9k &hellip; but ask me to tell you the ath5k story sometime :)

# What's Next

+ The GPL gives OpenWrt/LEDE a strong argument:
     + &ldquo;if you are out of compliance, we can't maintain your changes upstream&rdquo;.

+ OpenWrt/LEDE is the *key* project to influence wireless industry behavior:
     + proprietary Linux device drivers violate the license; the project
       takes on risk if it distributes them &hellip;
     + &hellip; so vendors must eliminate the risk by liberating the drivers
       &amp; gain upstream cooperation. 

+ The tool of GPL works for OpenWrt/LEDE to assure wireless device users'
software freedom.

# What about USA FCC &amp; Other Regulators?

+ So much but so little has changed in the 13 years since I sat across the
  table from those Broadcom executives.
      + We have a shared problem: misunderstanding by the FCC.

+ I thought we solved in this with
  [the Cognitive Radio Report and Order](http://hraunfoss.fcc.gov/edocs_public/attachmatch/FCC-07-66A1.pdf)
  back on 2007-04-25.
      + This is the ruling that allowed us to say: &ldquo;you have no FCC-related argument
         to fail to comply with the GPL&rdquo;
      + I'm quite sure ath9k would have been a non-starter without this ruling.

+ But thanks to Eric Schultz for being the very first to point out
  [FCC NPRM 15-170](transition.fcc.gov/Daily_Releases/Daily_Business/2015/db0722/FCC-15-92A1.pdf)
  was likely to trump the 2007 ruling.

# Reusing the Strategy

+ How can GPL help?
    + We had, from 2003-2007, and now may  again soon have a clear conflict
      between copyright requirements under GPL &amp; FCC regulations.

    + In the USA, we can bring this issue to the forefront: ultimately,
      two federal laws/regulations (i.e., copyright &amp; spectrum
      regulation) have a fundamental conflict.

+ So, why not ask the federal government to directly consider this conflict!
 
# Bringing Issue Forward

+ Ultimately, the NPRM dance with the FCC, while necessary, is only one
  approach to bring forward the issue.

+ Consider this other simple, parallel approach:

# Bringing Issue Forward

+ Bring a product before the FCC that needs to be GPL'd due to compliance,
  and ask for certification.

+ If/When it is not certified, we can directly ask the federal government to
  address the question head-on: &ldquo;Is the USA federal government really
  telling us to either violate GPL, or never incorporate GPL'd software into
  FCC-compliant wireless products?&rdquo;

+ Conservancy is investigating executing on this approach.

# More Info / Talk License

<img align="right" src="cc-by-sa-4-0_88x31.png" />

+ URLs / Social Networking / Email:
     - Pls. **support Conservancy**: [sfconservancy.org/supporter/](https://sfconservancy.org/supporter/)
     - [*The Guide*](https://copyleft.org/guide) is available &amp; [welcomes contributions at copyleft.org](https://copyleft.org).
     - Conservancy: [sfconservancy.org](https://sfconservancy.org/) &amp; <a href="https://twitter.com/conservancy/">@conservancy</a>.
     - Me: [faif.us](http://faif.us) &amp; [ebb.org/bkuhn](http://ebb.org/bkuhn)
     - Slides: [ebb.org/bkuhn/talks](http://ebb.org/bkuhn/talks/OpenSym-2016/politics.html).

<span class="fitonslide">
<p>Presentation and slides are: Copyright &copy; 2015, 2016 Bradley M. Kuhn, and are licensed under the <a rel="license" href="https://creativecommons.org/licenses/by-sa/4.0/legalcode">Creative Commons Attribution-Share Alike 4.0 International License</a>. </p>
</span>


<!--  LocalWords:  ldquo rdquo RSA img src shuttleworth jpg SSL CACM href sa
 -->
<!--  LocalWords:  Paywalls codebases codebase FOSDEM Source'd ACM png AAs
 -->
<!--  LocalWords:  blogosphere sfconservancy politikos Pls faif
 -->
