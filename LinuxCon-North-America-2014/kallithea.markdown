% Fork and Ignore: Fighting a GPL Violation By Coding Instead
% Bradley M. Kuhn
% Friday 22 August 2014

# GPL Violations Differ

+ Most of my talks historically have focused on embedded Linux-based GPL violations.
      + These are the most prevalent &amp; insidious.

+ However, GPL violations come in all shapes and sizes.

+ This is the story of a different sort of violation &hellip;
      + &hellip;  which inspired a different sort of resolution.

# What's a GPL Violation?

+ This point may be too remedial for some of you.
     + If so, take a 2 minute email break.

+ GPL (both v2 and v3) require:
     + The whole work licensed under GPL.
     + (which means all copyrighted material added must be under
       GPL-compatible licenses.)
     + Complete, Corresponding Source (CCS) of that work provided, under GPL.

# What's a GPL Violation?

+ I could give a whole talk on any of these topics:
     + What constitutes the &ldquo;whole work&rdquo;.
     + CCS requirements of GPL.

+ If you're new to GPL enforcement, just assume for this talk:
     + There are requirements on the forms of source-code disclosures. 
     + Everyone has an opinion on the &ldquo;whole/combined work&rdquo;
       question &hellip;
     + &hellip; but there is limited statutory guidance or Court precedent on the topic.

# Fundamental Assumptions

<img align="right" src="breaking-bad_how-much-is-enough_scaled.jpg" width="600" height="338"/>

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

+ Specifically, in June 2010:
     + Bitbucket was (still is) a proprietary solution.
     + GitHub was (still is) a proprietary solution &amp; only supports Git.
     + Phabricator wasn't released yet.
     + GitLab didn't exist yet (doesn't support Mercurial anyway).

+ Thus, [hg-app is announced](http://markmail.org/message/dx2pwuvt2l7u4tpn) on
  2010-06-03 under an [MIT-permissive license](https://kallithea-scm.org/repos/kallithea/files/bad9ccac26b7f84d8b7c65098ccfd6cd1903d4fe/LICENSE) on Mercurial's mailing list.

# There's Always A Flame War.

<img align="right" src="flame-war-exit.jpg" width="420" height="315"/>

+ A debate erupts about GPL compatible licensing.

+ hg-app is Based On (in the GPL sense) Mercurial:
      + Thus, in the view of most people, hg-app is based on Mercurial (in
        the copyright &amp; GPL sense).

+ Some point out that [MIT-permissive license is GPL-compatible](http://www.gnu.org/licenses/license-list.html#X11License).

+ The developer decides to avoid confusion and [relicenses hg-app under GPL](http://markmail.org/message/bds5x3ebnryzypkc).

# &hellip; &amp; the Community Goes On.

+ The project is renamed to [RhodeCode](http://markmail.org/message/qg545yaqqbbh3xxy).

+ Developers from Mercurial community begin contributing under GPL.

+ Independent contracts for software improvement are available for some.

+ All is well as a traditional Free Software community, until &hellip;

# Altering The Deal

<img align="right" src="vader-altered-the-deal.jpg" width="482" height="330"/>

+ RhodeCode's primary author forms a company, RhodeCode GmbH (The Company).

+ The Company announces a licensing scheme &ldquo;change&rdquo; for RhodeCode.
      + &amp; adds a &ldquo;20 user max&rdquo; code.

+ Community backlash, and threats from all sides.
      + Author of the patch that removes the 20 user max [is attacked](https://github.com/moparisthebest/unlimit-code).

# Conservancy as Mediator

+ Conservancy is contacted since Mercurial is a member project.
      + &amp; RhodeCode's codebase is based on GPL'd Mercurial code.

+ Some Mercurial developers and other community members seek aggressive enforcement action.

+ Conservancy seeks calm conversation with the Company.

+ The Company makes it clear that they believe it's 100% their copyright.

+ Situation quickly becomes a stand-off. 

# Of Course, GPL Is Irrevocable!

+ Of course, old code cannot be un-GPL'd.
      + AFAIK, no one has legitimately disputed that.

+ The question is with regard to future copyrights generated by the Company:
      + Can they relicense their *future* copyrighted works under non-GPL
        terms?

+ It's complicated:

<hr/>
>  All rights granted under this License are granted for the term of copyright on the Program, and are irrevocable provided the stated conditions are met.
<span class="fitonslide">
<p align=right>  &mdash;  GPLv3&sect;2&para;1

</p>
</span>

# &ldquo;Based on&rdquo; the earlier work

+ This codebase is, in Conservancy's view, GPL'd:
     + first, it's based Mercurial.
     + second, some third-party authors contributed patches under GPL.

+ The Company just doesn't agree.

+ Friendly negotiations to reach a fully GPL'd version going further failed.

+ So what are the options?

# How This Differs from Other Violations

+ Some GPL enforcement efforts reach the point of fundamental legal
  disagreement about the requirements of GPL.

+ In most cases, the stand-off is a true stand-off:
     + Free Software community doesn't have necessary CCS for the product.
     + A lawsuit eventually becomes only remaining way to compel CCS release.

+ But we don't have a mundane violation here.

# Early Friendliness Yields Better Options

+ Ultimately, the Company was, at one point, a good actor:
     + They shared kindly their software under the irrevocable GPL.

+ That code release remains GPL'd and useful.

+ In the worst case, forking at that point is an option.
     + &amp; avoids conflict.

# Avoiding Conflict

+ Conservancy has done GPL litigation before.

+ Lawsuits are the last resort; they take far too long.

+ When licensing of the primary codebase remains uncertain during the case:
     + you've effectively repeated USL v. BSDi, and tied your codebase up in
       court for years.

+ Conservancy had better options here, thanks to earlier GPL release &hellip;
     + &hellip; plus partial release of more recent code under GPL.
 
# A Complex License

+ The Company's final text of [their license](https://rhodecode.com/licenses)
  is clearly ambiguous (or worse):

+ GPLv3, in fact, contemplated this problem:

<hr/>
<span class="fitonslide">
<p>
RhodeCode system is split-licensed and comprised of two parts:<br/><br/>
(1) The Python code and integrated HTML are licensed under the GPLv3 license as is RhodeCode itself. &hellip;<br/><br/>
(2) All other parts of RhodeCode including, but not limited to, CSS code, images, and design are licensed according to the license purchased.
</p>
</span>
 
# Invalid Additional Term?

<br/>

>  All other non-permissive additional terms are considered "further restrictions" within the meaning of section 10.  If the Program as you received it, or any part of it, contains a notice stating that it is governed by this License along with a term that is a further restriction, you may remove that term.
<span class="fitonslide">
<p align=right>&mdash;  GPLv3&sect;7&para;4</p>
</span>

# Remember: No Conflict!

+ Obviously, the Company would fight Conservancy's GPLv3&sect;7&para;4 claim.

+ Instead, to make peace, Conservancy reads the license more conservatively
  than necessary.

<hr/>
<span class="fitonslide">
<p>
RhodeCode system is split-licensed and comprised of two parts:<br/><br/>
(1) The Python code and integrated HTML are licensed under the GPLv3 license as is RhodeCode itself. &hellip;<br/><br/>
(2) All other parts of RhodeCode including, but not limited to, CSS code, images, and design are licensed according to the license purchased.
</p>
</span>

# Making the Fork

+ Thus begins: the hard work of a four step process:
      + Find the last known version of the codebase without the new (invalid) text added.
      + Extract useful patches of only Python code and HTML files from
        post-license-change versions.
      + Rebrand to a new name.
      + Ensure &ldquo;beyond reproach&rdquo; compliance.


# Step 0: Last Known GPLv3'd version

+ First step was easier than it looked.

+ Beta branch got new license in early August 2013:

        changeset:   4466:66aad5f0a38e
        branch:      beta
        user:        Marcin Kuzminski <marcin@python-works.com>
        date:        Wed, 07 Aug 2013 04:33:56 -0500 (12 months ago)
        summary:     updated license header

        diff --git a/LICENSE b/LICENSE
        --- a/LICENSE
        +++ b/LICENSE
        @@ -1,3 +1,13 @@
        +RhodeCode system is comprised of two parts:
        +(1) The Python code and integrated HTML are licensed under the GPLv3 license as
        +is RhodeCode itself.
        +You will find a copy of the license text below.
        +
        +(2) All other parts of the RhodeCode including, but not limited to the CSS code,
        +images, and design are licensed according to the license purchased.
        +Read about licensing details here: https://rhodecode.com/licenses
        +
        +
                     GNU GENERAL PUBLIC LICENSE
                        Version 3, 29 June 2007

# Step 0: Last Known GPLv3'd version

+ Material in beta branch was thus considered for Step 1.

+ The v1.7.2 maintenance branch never received the license patch.

+ For Step 0, we took:

        changeset:   4107:fc64cd9bb856
        tag:         v1.7.2
        user:        Marcin Kuzminski <marcin@python-works.com>
        date:        Mon, 02 Sep 2013 09:49:53 -0500

# Step 1: Extract New Python &amp; HTML

+ Even with hyper-conservative reading, Python code &amp; HTML are clearly GPLv3'd.

+ Careful extraction was required to include only those changes.

+ We wrote a shell script to rerun Mercurial commands and verified resulting
  repositories included only new changes to Python &amp; HTML files.

# Step 1: Example Command

      hg --cwd $RHODECODE_REPOSITORY diff -r 21af6c4eab3d -r 6177597791c2 \
         -I rhodecode/__init__.py \
         -I rhodecode/websetup.py \
         -I rhodecode/bin/ \
         -I rhodecode/config/ \
         -I rhodecode/controllers/ \
         -I rhodecode/lib/ \
         -X rhodecode/lib/paster_commands/make_config.py \
         -X rhodecode/config/deployment.ini_tmpl \
         -X rhodecode/bin/template.ini.mako \
         -I rhodecode/model/ \
         -I rhodecode/tests/ \
         -I rhodecode/templates/ \
         -I setup.py \
        | hg --cwd $KALLITHEA_REPOSITORY import - --no-commit

# Step 1: Vetting

+ Output of each diff command (i.e., each patch):
      + Vetted by me to verify it was just Python/HTML changes.
      + Edge cases discussed carefully with legal counsel.

# Step 3: Rename

+ Won't use the (potentially trademarked) brand name, &ldquo;RhodeCode&rdquo;
     + &hellip; other than in those ways third parties are already permitted to do so.

+ Picking names is always hard.
     + We decided on: &ldquo;Kallithea&rdquo;

<hr/>

> Kallithea, or  &Kappa;&alpha;&lambda;&lambda;&iota;&theta;&epsilon;&alpha;, is the name of a locality on the island of Rhodes, in Greece, which itself means &lsquo;the best view&rsquo;. Our Kallithea project helps developers get the best views of their project and its contributions so they can better collaborate together.

# Step 3: Rename

+ Problem: rhodecode_ was commonly used throughout the code.

+ Hyper-conservative approach requires removal.
     + This is of course mostly functional use, so perhaps unnecessary.

+ Obvious sed/perl scripts require care:
     + You have to make sure your replacements generate working code!
     + Ultimately 300 lines of shell commands were needed.

# Step 3: Example Commmands

    sed -i 's,setup-rhodecode,setup-db,g' */tests/scripts/create_rc.sh docs/*.rst setup.py
    sed -i 's,setup_rhodecode,setup_db,g' setup.py
    hg ci -m 'Rename paster command setup-rhodecode to setup-db'

    hg mani | xargs sed -i 's/\<from rhodecode import /from kallithea import /g'
    sed -i 's,\<rhodecode \(=\|is\) None\>,kallithea \1 None,g' */config/*.py
    hg mani | xargs sed -i 's/\<import rhodecode$/import kallithea/g'
    hg mani | xargs sed -i 's/\<rhodecode\.\(bin\|config\|controllers\|lib\|model\|tests\|__init__\|__version__\|websetup\|CONFIG\|EXTENSIONS\|CELERY_ON\|CELERY_EAGER\)\>/kallithea.\1/g'
    hg mani | xargs sed -i 's,\<rhodecode/\(controllers\|lib\|model\|tests\|public\|i18n\|__init__\|templates\)\>,kallithea/\1,g'
    sed -i 's, rhodecode/, kallithea/,g' MANIFEST.in

     hg mani | xargs sed -i -e 's,settings\['"'rhodecode_' + ,settings[,g" -e 's,\<rhodecode_\(title\|realm\|ga_code\|captcha_public_key\|captcha_private_key\|show_public_icon\|show_private_icon\|stylify_metatags\|repository_fields\|lightweight_journal\|dashboard_items\|admin_grid_items\|show_version\|use_gravatar\|gravatar_url\|clone_uri_tmpl\|update_url\|extras\)\>,\1,g'
     hg ci -m 'Drop rhodecode_ prefix for known setting names that are stored in kallithea_settings without prefix'

#  Step 4: Beyond Reproach

+ Even if the Company violated the GPLv3:
      + it doesn't mean we have permission to do so.
      + as a large copyright holder, the Company could enforce against the fork.

+ Therefore, we must be beyond reproach in our compliance.
      + which means the CCS must be right is a complicated issue.

+ Why is getting the CCS right difficult in this case?

# GPL'd Javascript

+ Most people don't realize how similar Javascript programs are to mundane
  software distribution:
      + You publish a .js file on a URL.
      + Your users download it with an HTTP request.
      + You've *distributed* (in GPLv3 terms, *conveyed*) the software to
        them.

+ Every GPL requirement, including those relating to CCS provisioning *apply*
  fully for most Javascript in a GPL'd system!

# So, What Do I find?

So, there's Javascript in this thing?

      $ hg clone -q https://kallithea-scm.org/repos/kallithea/
      $ cd kallithea; hg update -C ffd45b185016
      $ ls -1 rhodecode/public/js/
      codemirror.js
      codemirror_loadmode.js
      excanvas.min.js
      qgraph.js
      jquery.1.10.1.min.js
      mergerly.js
      mode
      native.history.js
      pyroutes_map.js
      rhodecode.js
      yui.2.9.js
      yui.flot.js

# Verify Upstream licensed this code

     $
     $ hg -v log -r bb9ef0638069
     changeset:   4120:bb9ef0638069
     branch:      rhodecode-2.2.5-gpl
     user:        Bradley M. Kuhn <bkuhn@sfconservancy.org>
     date:        Fri May 16 15:54:24 2014 -0400
     description:
       Update CodeMirror CSS and Javascript files to version 3.15, under MIT-permissive license.

       These files are exactly as they appear the upstream release 3.15 of
       Codemirror, which was released under an MIT-permissive license.  To extract
       these files, I did the following:

       I downloaded the following file:
            http://codemirror.net/codemirror-3.15.zip
       with sha256sum of:
       $ sha256sum codemirror-3.15.zip
       8cf3a512899852fd4e3833423ea98d34918cbf7ee0e4e0b13f8b5e7b083f21b9  codemirror-3.15.zip

       And extracted from it the Javascript and CSS files herein committed, which
       are licensed under the MIT-permissive license, placing them into their
       locations in: rhodecode/public/{css,js}/

       Using the procedure above, the only difference found between these files in
       RhodeCode 2.2.5 release and herein were a few comments and whitespace.

       Note that the file .../public/js/mode/meta_ext.js does *not* appear to be
       part of CodeMirror and therefore is not included in this commit.

# Add Correct LICENSE notices

Update our LICENSE.md:

      Codemirror
      ----------

      Kallithea incorporates parts of the Javascript system called
      [Codemirror](http://codemirror.net/), which is primarily:

      Copyright &copy; 2013 by Marijn Haverbeke <marijnh@gmail.com>

      and licensed under the MIT-permissive license, which is
      [included in this distribution](MIT-Permissive-License.txt).

      Additional files from upstream Codemirror are copyrighted by various authors
      and licensed under other permissive licenses.  The sub-directories under
      [.../public/js/mode/](kallithea/public/js/mode) include the copyright and
      license notice and information as they appeared in Codemirror's upstream
      release.

# Most Javascript is Object Code

+ That was easy compared to minified Javascript.

+ Minified Javascript is Object Code.

+ Must find appropriate CCS, &amp; restart from scratch.

# Most Javascript is Object Code

<br/>

> "Object code" means any non-source form of a work.
<p align=right>  &mdash; GPLv3&sect;1&para;1
</p>
<hr/>
> Object code is not restricted to a narrow technical meaning and is understood broadly to include any form of the work other than the preferred form for making modifications to it.  **Object code** therefore **includes** any kind of transformed version of source code, such as bytecode or **minified Javascript**.
<p align=right>
&mdash; [FSF's GPLv3 First Rationale Document, 2006-01-16](http://gplv3.fsf.org/gpl-rationale-2006-01-16.tex/view) (emphasis mine)
</p>

# Why You?!? I (asked)!

+ YUI 2.9 is Yahoo's (deprecated) Javascript interface library.
+ Minified versions found on many websites &hellip;
     + &hellip; which isn't a violation &hellip;
     + &hellip; since YUI is 3-Clause BSD &hellip;
     + &hellip; but it's now part of a larger GPLv3'd work's CCS.

<hr/>

> The "Corresponding Source" for a work in object code form means all the source code needed to generate, install, and (for an executable work) run the object code and to modify the work, including scripts to control those activities.
<span class="fitonslide">
<p align=right>
&mdash; GPLv3&sect;1
</p>
</span>

# Handling Our Distribution

What about distributing minified Javascript in our repository?

<hr/>

> Convey the object code by offering access from a designated place (gratis or for a charge), and offer equivalent access to the Corresponding Source in the same way through the same place at no further charge.  You need not require recipients to copy the Corresponding Source along with the object code.
<span class="fitonslide">
<p align=right>
&mdash; GPLv3&sect;6(c)
</p>
</span>

# YUI Solution

From our LICENSE.md:

    Kallithea incorporates parts of the Javascript system called
    [YUI 2 — Yahoo! User Interface Library](http://yui.github.io/yui2/docs/yui_2.9.0_full/),
    which is made available under the [BSD License](http://yuilibrary.com/license/):

    Copyright &copy; 2013 Yahoo! Inc. All rights reserved.
    [Text of 3-Clause BSD]

    Kallithea includes a minified version of YUI 2.9. To build yui.2.9.js:
        git clone https://github.com/yui/builder
        git clone https://github.com/yui/yui2
        cd yui2/
        git checkout hudson-yui2-2800
        # work around inconsistent casing
        ln -sf JumpToPageDropDown.js src/paginator/js/JumpToPageDropdown.js
        rm -f tmp.js
        for m in yahoo event dom connection animation dragdrop \
                 element datasource autocomplete container event-delegate \
                 json datatable paginator; do
          rm -f build/\$m/\$m.js
          ( cd src/\$m && ant build deploybuild ) && \
            sed -e 's,@VERSION@,2.9.0,g' -e 's,@BUILD@,2800,g' build/\$m/\$m.js >> tmp.js
        done
        java -jar ../builder/componentbuild/lib/yuicompressor/yuicompressor-2.4.4.jar \
         tmp.js -o yui.2.9.js

    In compliance with GPLv3 the Corresponding Source for this Object Code is made
    available on [https://kallithea-scm.org/repos/mirror](https://kallithea-scm.org/repos/mirror).

# Lessons for New Communities

<img align="right" src="stan-learned-something.jpg" width="224" height="316"/>

+ For a web application, *don't* just copy Javascript (even Free Software
  stuff) into your repository.

+ When you start contributing to a project, *ask* who holds domain name
  &amp; trademark for the project.
       + If the answer is one person or I don't know, find a non-profit like
         Conservancy to help *right away*.

+ Keep your own copyrights &amp; make it clear you expect the license to be
  upheld.
       + &amp; will do so yourself if needed.

# More Info / Talk License

<img align="right" src="cc-by-sa-4-0_88x31.png" />

+ URLs / Social Networking / Email:
     - [Kallithea Project: https://kallithea-scm.org](https://kallithea-scm.org).
     - A Book I helped write: [*Copyleft and the GNU General Public License: A Comprehensive Tutorial*](http://ebb.org/bkuhn/writings/comprehensive-gpl-guide.pdf) is available.
     - Conservancy: [sfconservancy.org](https://sfconservancy.org/) &amp; [@conservancy](https://twitter.com/conservancy/)
     - Me: [faif.us](http://faif.us) &amp; [ebb.org/bkuhn](http://ebb.org/bkuhn)
     - Slides: [ebb.org/bkuhn/talks](http://ebb.org/bkuhn/talks/LinuxCon-North-America-2014/kallithea.html) &amp; [gitorious.org/bkuhn/talks](https://gitorious.org/bkuhn/talks/source/master:LinuxCon-North-America-2014) (source)
     - DONATE: [https://sfconservancy.org/donate/](https://sfconservancy.org/donate/)
     - Sign Up Today as part of the [*GPL Compliance Project for Linux Developers*](https://sfconservancy.org/linux-compliance/).

<span class="fitonslide">
<p>Presentation and slides are: Copyright &copy; 2014 Bradley M. Kuhn, and are licensed under the <a rel="license" href="https://creativecommons.org/licenses/by-sa/4.0/legalcode">Creative Commons Attribution-Share Alike 4.0 International License</a>. </p>
<p>Some images included herein are &copy;'ed by others. I believe my use of those images is fair use under USA &copy; law.  However, I suggest you remove such images if you redistribute these slides under CC-By-SA 4.0.
</p>
</span>
