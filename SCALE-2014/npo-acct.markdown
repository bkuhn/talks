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


# NPO as YA Vertical Market

+ Fiscal sponsorship is specialized.

+ Conservancy's auditor call this the Z axis of accounting:
       + NPOs care where money came from (example next).
       + Fiscal sponsors have to earmark funds under temporary restrictions.

+ Even fiscal sponsors outside of software *have developers on staff* to do
  custom accounting.
       + e.g., Fractured Atlas.

+ So many reports no one but a non-profit needs.

# The Public Support Test

+ Take the last five years' income.

+ Compute 2% of it.

+ Figure out what donors in the last 5 years have given more than 2% of that.

+ Divide the excess donations by the total donations over the five year
  period.  You "pass" if that number is 33&#x2153;.%.

+ (And there other special cases not described above).

+ This report doesn't exist:
     + Many non-profits don't even have data-gathering sufficient to run it.


# Those Who Forget the Past &hellip;

+ What should we do to avoid this vertical market bias?

+ Remember what Luca taught us circa 1509:
       + double entry accounting is a *math library*.
       + How many times have you written sqrt(), cos()?
       + We need a library.

# Brogrammers Are Sometimes (Partly) Right
<span class="fitonslide">
*Up The Asset* is a reimagination of accounting software for the modern
age.  Based on the proven, centuries-old principle of double-entry
bookkeeping, yet using nothing but open web standards &amp; formats stored in
text files, it aims to bring to accounting the same breath of fresh air
which git brought to version control.
</span>

**Arrogant Much?**

    $ git clone https://github.com/zacharyvoase/uptheasset
    $ cd uptheasset; git log --pretty=oneline|wc -l
    52
    $ wc -l `find . -type f -print`|tail -1
    1324 total

# Enter Ledger-CLI

+ Ledger CLI is a hackers' way of doing accounting.

+ plain text files format

+ generate reports with the command line.

+ Only a command-line hacker who is *also* an accounting geek can love this.
       + there are probably only 100 people like this on the planet.

# Conservancy Already Runs on This

+ I keep the books of Conservancy myself &hellip;
       + &amp; I happen to be a CLI hacker who's also an accounting geek.

+ I'm documenting our system of tagging transactions to link up to reporting:
       + <a href="https://gitorious.org/ledger/npo-ledger-cli">https://gitorious.org/ledger/npo-ledger-cli</a>

# Reusing Ledger-CLI

+ Ledger-CLI ultimately *is* a double entry accounting math library.

+ but it has no real API.

+ Our first job: make an API.

# This Is Not Vaporware

+ Yes, if I have to title a slide &hellip;
      + that says this isn't vaporware &hellip
      + you have to worry if it's vaporware.

+ But, we've written a proof of concept of a JSON API to do double entry
  accounting.

# There's a There There.

    $ git clone https://git.gitorious.org/conservancy/accounting-api.git
    $ cd accounting-api; git log --pretty=oneline|wc -l
    64
    $ wc -l `find . -type f -print`|tail -1
    58395 total

Documentation available at: <a
href="http://npoacct.sfconservancy.org/accounting-api/">http://npoacct.sfconservancy.org/accounting-api/</a>.


# Basics of the REST API

Ledger-CLI Data: 
    2010/01/01 Kindly T. Donor
        ;Id: Ids can be anything
      Income:Foo:Donation   $-100.00
        ;Invoice: Projects/Foo/Invoices/Invoice20100101.pdf
      Assets:Checking       $100.00


# REST API: Transaction List

    GET /transaction HTTP/1.1
    Host: accounting.example
    Accept: application/json

    HTTP/1.1 200 OK
    Content-Type: application/json
    {
       "transactions": [
         {
            "__type__": "Transaction",
            "date": "2010-01-01",
            "id": "Ids can be anything",
            "metadata": {},
            "payee": "Kindly T. Donor",
            "postings": [
            {
               "__type__": "Posting",
               "account": "Income:Foo:Donation",
                   "amount": {
                       "__type__": "Amount",
                       "amount": "-100",
                       "symbol": "$"
                    },
             "metadata": {
                 "Invoice": "Projects/Foo/Invoices/Invoice20100101.pdf"
              }
      }]}


# REST API Functions

+ Get all, get specific, Add, delete, update

+ This is admittedly a proof-of-concept.

+ Next step: transition Conservancy reporting to use this API:
      + to improve and shake out the bugs.

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
