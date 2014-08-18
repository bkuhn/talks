% Fork and Ignore: Fighting a GPL Violation By Coding Instead
% Bradley M. Kuhn
% Friday 22 August 2014

# GPL Violations Differ

+ Most of my talks historically have focused on embedded Linux-based GPL violations.
      + These are the most prevalent &amp; insidious.

+ However, GPL violations come in all shapes and sizes.

+ This is the story of a different sort of violation &hellip;
      + &hellip;  which allowed for a different sort of resolution.

# What's a GPL Violation?

+ This point may be too remedial for some of you.
     + If so, take a 2 minute email break.

+ GPL (both v2 and v3) require:
     + The whole work licensed under GPL.
     + Complete, Corresponding Source (CCS) of that work provided, under GPL.

+ I could give a whole talk on any of these topics:
     + What constitutes the &ldquo;whole work&rdquo;.
     + CCS requirements of GPL.

+ If you're new to GPL enforcement, just assume for this talk:
     + There are requirements on the forms of source-code disclosures. 
     + Everyone has an opinion on the &ldquo;whole/combined work&rdquo;
       question &hellip;
     + &hellip; but there is limited statutory guidance or Court precedent on the topic.


# Fundamental Assumptions

+ Generally speaking, everyone assumes:
     + proprietary software is more lucrative than Free Software.

+ The veracity of this claim is immaterial.
     + only the perception that it's true matters.

+ Companies therefore try to keep as much proprietary as they can.

# Fundamental Assumptions

+ Most developers, left to their own devices, share their code.

+ They tend to share their code if it's convenient.
     + &amp; even sometimes when it's not so convenient.

+ That's not to say most developers are software freedom zealots like me.

+ Rather, they err on the side of code-sharing.
     + In current times, that means developers  by default release code early
       and often under a Free Software license.

+ Thus, under these assumptions, so begins our story &hellip;


# A Developer Releases a Codebase

+ The story starts like most Free Software stories:
     + In 2010-10, a developer saw some useful proprietary software &hellip;
     + &hellip; didn't like the existing Free Software alternatives &hellip;
     + &hellip; and started writing one.

+ Specifically:
     + GitHub was a proprietary solution &amp; only supports Git.
     + Phabricator existed, but was written in PHP &amp; was
       Facebook-controlled.
     + GitLab didn't exist yet (doesn't  support       Mercurial.

+ Thus, [hg-app is announced](http://markmail.org/message/dx2pwuvt2l7u4tpn) on
  2010-06-03 under an [MIT-permissive license](https://kallithea-scm.org/repos/kallithea/files/bad9ccac26b7f84d8b7c65098ccfd6cd1903d4fe/LICENSE) on Mercurial's mailing list.

# There's Always Flaming.

+ A debate erupts about GPL compatible licensing.

+ hg-app incorporates code from Mercurial:
      + Thus, in the view of most people, hg-app is based on Mercurial (in
        the copyright &amp; GPL sense).

+ Some point out that [MIT-permissive license is GPL-compatible](http://www.gnu.org/licenses/license-list.html#X11License).

+ The developer decides to avoid confusion and [relicense hg-app under GPL](http://markmail.org/message/bds5x3ebnryzypkc).

