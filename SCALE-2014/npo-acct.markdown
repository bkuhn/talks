% A New Approach to Accounting Software for Non-Profit Organizations
% Bradley M. Kuhn
% Saturday 22 February 2014

# Thanks to SCALE

+ This is one of the best conferences in the Open Source and Free Software community.

+ Because it's community-run and organized by a non-profit.

+ For-profit corporate control is not an issue here.

+ That means a lot to me as a non-profit career administrator &amp; policy wonk.

# Governance / Licensing First

+ I always hate sitting through talks waiting to hear what the license is.

# Governance / Licensing First

+ Conservancy's NPO Accounting Project will:
     + Be multi-copyright held (NO CLA!) &hellip;
     + &hellip; even Conservancy is letting contractors keep copyright.
     + new code licensed under Affero GPL.
     + any upstreamable code: use license of upstream project &hellip;
     + &hellip; specifically Ledger-CLI is 3-Clause-BSD.

# Governance / Licensing First

+ All development done in public:
     + Max time btw. authorship &amp; publish is a day or two.
     + But an hour or two is ideal.
     + Public mailing list and IRC channel.

# A Brief History of Accounting Software

+ Accounting software systems have existed since 1960s.

+ Imagine how many times our society as reinvented this wheel.

+ People are *still* getting hired to write COBOL &hellip;
     + &hellip; mostly for accounting/financial systems.

# &amp; In Open Source and Free Software?

+ Phase 0 of our project: evaluate known FLOSS accounting software.

+ Results: http://npoacct.sfconservancy.org/ExistingProjects/
     + Nearly 20 projects.
     + Every single one of them *reinvents the double-entry wheel*.
     + And often not very well.
     + e.g.: ERPNext: we found two SQL injection attacks in 30 minutes.
     + None of them separate API boundary walls adequately.
 
# A Brief History of Double-Entry System


# A Brief History of Double-Entry System

+ Luca Pacioli: a late 1400s Venetian mathematician with a wealthy patron.

+ Luca is writing a math book.

+ His patron asks him to write up the Venetian System.

<hr/>
<span class="fitonslide">
<p align=right>
Source: <a href="http://www.npr.org/blogs/money/2013/10/18/237169497/episode-407-a-mathematician-the-last-supper-and-the-birth-of-accounting">NPR's *Planet Money*, Episode 407: *A Mathematician, The Last Supper And The Birth Of Accounting*</a>
</p>
</span>

# A Brief History of Double-Entry System

+ How do you keep track of what you have and what form it is in?

+ The Ventians were using this system of recording books in double-entry.

+ Luca adds it to his math encyclopedia

<hr/>
<span class="fitonslide">
<p align=right>
Source: <a href="http://www.npr.org/blogs/money/2013/10/18/237169497/episode-407-a-mathematician-the-last-supper-and-the-birth-of-accounting">NPR's *Planet Money*, Episode 407: *A Mathematician, The Last Supper And The Birth Of Accounting*</a>
</p>
</span>


#  An Example of Double Entry

    2014-02-10 Monthly Salary
       Assets:Checking           $1,000.00
       Income:Salary            $-1,000.00

# The Accrual Basis

    2014-01-31 Earned Monthly Salary
       Accrued                   $1,000.00
       Income:Salary            $-1,000.00

    2014-02-10 Monthly Salary
       Assets:Checking           $1,000.00
       Accrued                  $-1,000.00

# Pretty Simple, Right?

+ Sure, Double Entry bookkeeping is simple and easy to learn.

+ It's relatively easy to explain.

+ So, every developer looks at it and just implements it again.
     + But why?

# Why Is This Wheel Reinvented?: 1st

+ How'd did we get Y2K?
     + &ldquo;Who would still be using this code in 2000?&rdquo;x
     + Systems live longer than developers think.

+ Great developers plan ahead.
     + But great developers are rarely assigned accounting.

<hr/>

> He wasn't a good enough developer to work on GNU, so I assigned him to work on FSF's accounting system, figuring maybe he could do that.  I guess he couldn't.

<span class="fitonslide">
<p align=right>
 &mdash; Richard M. Stallman
</p>
</span>

# Why Is This Wheel Reinvented?: 2nd

+ Accounting is seen as purely vertical market software.

+ AFAICT, no one *has ever* tried to write a true horizontal marketing accounting software stack.

# Consider the NPO Problem

+ Blackbaud is the Oracle of non-profits.
    + No one ever got fired for chosing Blackbaud.
    + (although ask Josh Berkus for his story about this.)

+ Accountants generally don't understand software &hellip;
    + &hellip; so, they are used to what they know.
    + &hellip; but, Smarter accountants know something is wrong.

<hr/>
> I'd tell you to buy Blackbaud or Fund-EZ, but your books as a fiscal sponsor are complicated enough that they won't meet your needs anyway.

<span class="fitonslide">
<p align=right>
 &mdash; Gary Eisenkraft, Conservancy's auditor, after Conservancy's FY 2011 audit.
</p>
</span>

# Why-At ERP?

+ ERP: TLA for Enterprise Resource Planning

+ ERP people are obsessed with workflows.
     + Workflows *are* important.
     + But remember the vertical market bias.

+ ERP workflows always make assumptions about their preferred vertical
  market.


# ERP Workflow FAIL: Example

+ Most accountants will tell you: &ldquo;Accrue funds when you issue an
  invoice&rdquo;.

+ That's *usually* correct.

+ Except when it isn't.

+ NPO Fundraising trick: issue an invoice that you don't have a good faith
  basis to be paid.

+ Of course, accountants agree that this is &hellip;
      + fine under GAAP &hellip;
      + as long as you *don't* accrue.

# ERP Workflow FAIL: Example

+ Most ERP systems auto-accrue on invoice generation.

+ It's not a configurable part of workflow.

+ But this is no good for NPOs.

# More Info / Talk License

+ URLs / Social Networking / Email:
     - NPO Accounting project:
          + http://npoacct.sfconservancy.org/
          + https://gitorious.org/conservancy/accounting-api
     - Conservancy: sfconservancy.org &amp; @conservancy
     - Me: faif.us, ebb.org/bkuhn &amp; @bkuhn (identi.ca)
     - Slides: ebb.org/bkuhn/talks &amp; gitorious.org/bkuhn/talks (source)
     - DONATE: http://sfconservancy.org/donate/

<span class="fitonslide">
<p>Presentation and slides are: Copyright &copy; 2014 Bradley M. Kuhn, and are licensed under the <a href="http://creativecommons.org/licenses/by-sa/4.0/">Creative Commons Attribution-Share Alike (CC-By-SA) 4.0 International License</a>. <img src="cc-by-sa-3-0_88x31.png"/></p>

<p>Some images included herein are &copy;'ed by others. I believe my use of those images is fair use under USA &copy; law.  However, I suggest you remove such images if you redistribute these slides under CC-By-SA-USA 3.0.
</p>
</span>
