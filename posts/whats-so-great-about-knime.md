<!--
.. title: What's so great about Knime?
.. slug: whats-so-great-about-knime
.. date: 2018-09-16 00:00:42 UTC-05:00
.. tags: workflow,knime,python
.. category: Tools
.. link: 
.. description: 
.. type: text
-->

This year, (for the fifth time, according to
[Forest Grove Technology](https://www.forestgt.com.au/latest-news/2018/3/2/knime-2018-gartner-magic-quadrant-market-leader>),
the Knime Analytics platform was named a Gartner Magic Quadrant
leader. This year's other leaders are [Alteryx](https://www.alteryx.com/),
[SAS](https://www.sas.com/), [RapidMinder](https://rapidminer.com/),
and [H2Oai](https://www.h2o.ai/).
What surprised me in the announcement is that the platform is open source,
and free for individual users: I can afford to look at it!

Knime (silent "k"; rhymes with "dime") actually looks a lot like
Alteryx at first glance.
And both seem like Pentaho/Informatica but for machine learning,
meaning they provide a way to chain together steps in a data science
workflow by drawing lines between them in a graphical editor.
It also means the workflow is preserved,
along with links to the original code, in an executable pipeline.
Months later, if someone revisits the project, it will be understandable
at a glance, and still runnable.

Knime can connect to raw files, databases, AWS S3 and Azure, and
can interface with Python, R, Java, H2O.ai, and a ton more.
Plus, it can run with industry-standard [PMML](https://sourceforge.net/projects/pmml/)
models, meaning it's enterprise-deployable.
Even better, junior people can onboard quickly into a data science
team with workflows that have existing data preparation written by people
already familiar with the <span class="vocabulary" title="A ton of mistakes happen when different people aggregate data in different ways. Even something as simple as quarterly service calls—when does a quarter end? On the Friday of the business week? Or the literal last day of the month? At close of business? Midnight? Midnight GMT?">company's data</span>
and target metrics.

This is easy because Knime's built-in modularity forces users to
think in a modular way. Seriously,
[download it](https://www.knime.com/downloads) and follow along
with a Python workflow.

<!-- TEASER_END -->

## 



.. 
    ## Lots of  setup  ## TANYA SAVE FOR FUTURE
    
    This is overkill for a blog post but it's what I'd do in real life to use this week over week. Rather than running the entire script over and over again, the goal is to set up a database and just process the data as they come, incrementally updating the model. You can toggle the code below to see the setup.
    
    ### SQLite database
    
    <a href="https://www.sqlite.org/index.html">SQLite</a>, written in C, is massively underrated. They say themselves they're not an enterprise database, but from their <a href="https://sqlite.org/whentouse.html">'when to use' page</a>, <quote>"Generally speaking, any site that gets fewer than 100K hits/day should work fine with SQLite."</quote> Plus, since the <a href="https://docs.python.org/library/sqlite3.html">sqlite3</a> database api is in Python's standard library, it's perfect for personal projects. And for a cherry on top: it looks like windowing functions, intended to behave as described in the PostgreSQL documentation, are <a href="https://www.sqlite.org/draft/windowfunctions.html">in the works</a> for the next release. Rah SQLite!

