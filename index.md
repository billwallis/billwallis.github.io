<head>
  <title>Personal Projects</title>
  <link rel="shortcut icon" type="image/x-icon" href="favicon.ico?">
</head>

<span style="font-weight:bold">🚀 Personal Projects</span>

**What's on this page?**

* TOC
{:toc}

---

## [⏱️ Database Query Profiler](https://github.com/Bilbottom/db-query-profiler)

<span style="color:grey" size=1>[https://github.com/Bilbottom/db-query-profiler](https://github.com/Bilbottom/db-query-profiler)</span>

One of the awesome things about SQL is that there are so many different ways to get the same output. One of the hardest things about SQL is knowing which way is the most performant way 😝

Enter: the **Database Query Profiler**.

This is a Python package that will run a set of queries against your database a number of times and return the average execution times. It's intended to be used during development to help you understand the actual performance of your queries.

> **_This is NOT a replacement for analysing the [query plan](https://en.wikipedia.org/wiki/Query_plan). This should just support the analysis done with it._**

**✨ Features**

- Database agnostic, just provide a class that can execute a query against your database
- Minimal setup required, drop your queries into a directory and run!
- Provides real-time feedback on the progress of the profiling (thanks to [`tqdm`](https://github.com/tqdm/tqdm))

A typical output will look something like this:

```
Start time: 2023-05-07 12:38:06.879738
----------------------------------------
100%|██████████| 5/5 [00:01<00:00,  3.29it/s]
query-1.sql: 0.10063192s (33.4%)
query-2.sql: 0.20044784s (66.6%)
----------------------------------------
End time: 2023-05-07 12:38:08.757555
```

---

## [📝 Timesheet automation with pop-up boxes](https://github.com/Bilbottom/daily-tracker)

<span style="color:grey" size=1>[https://github.com/Bilbottom/daily-tracker](https://github.com/Bilbottom/daily-tracker)</span>

Not sure where all your time goes? I wasn't either, so this application generates a pop-up box every 15 minutes (configurable) for me to enter what I'm working on.

<div style="text-align: center;">

<img alt="pop-up-box" src="https://raw.githubusercontent.com/Bilbottom/daily-tracker/main/tracker-form-tkinter.png"/>

</div>
<br>

**✨ Features**

- Drop-down box to select from recent projects
- Autopopulates the detail text box with the project's last entry
- Integrates with [Outlook <img alt="Microsoft Outlook" height="14px" src="https://outlook.live.com/favicon.ico"/>](https://outlook.live.com/owa/)
  - Reads the calendar and autofills with meeting information
- Integrates with [Jira <img alt="Jira Software" height="12px" src="https://example.atlassian.net/favicon.ico">](https://www.atlassian.com/software/jira)
  - Reads tickets in the current sprint and adds them to the project drop-down
  - Adds a worklog to the ticket when the form is submitted
- Integrates with [Slack <img alt="Slack" height="12px" src="https://slack.com/favicon.ico"/>](https://slack.com/)
  - Posts a message to channel when the form is submitted

**⚠️ Warnings**

- This is still very early in development and is undergoing a significant restructure
- The code coverage is extremely limited
- The code requires manual tweaks the first time it's cloned
- There are a number of outstanding issues, see the repo's Issues page:
  - [https://github.com/Bilbottom/daily-tracker/issues](https://github.com/Bilbottom/daily-tracker/issues)

---

## [<img alt="dbt-labs" height="16px" src="https://www.getdbt.com/favicon.ico"> Life Admin using dbt](https://github.com/Bilbottom/billiam-database)

<span style="color:grey" size=1>[https://github.com/Bilbottom/billiam-database](https://github.com/Bilbottom/billiam-database)</span>

In addition to my 'automated' timesheet (the project above), I also keep track of every transaction I make at an item level (since 2018-01-18).

This project is both a [dbt](https://www.getdbt.com/) proof-of-concept, plus a means for me to analyse my spending and work.

Current lineage diagram:

<img alt="lineage-diagrams" src="https://raw.githubusercontent.com/Bilbottom/billiam-database/main/src/assets/dbt-dag.png"/>

The dbt documentation is hosted at:

- [https://bilbottom.github.io/billiam-database](https://bilbottom.github.io/billiam-database)

---

## [<img alt="PyCharm" height="16px" src="https://upload.wikimedia.org/wikipedia/commons/1/1d/PyCharm_Icon.svg"> Custom PyCharm Database Extensions](https://github.com/Bilbottom/pycharm-extensions)

<span style="color:grey" size=1>[https://github.com/Bilbottom/pycharm-extensions](https://github.com/Bilbottom/pycharm-extensions)</span>

PyCharm is awesome, and it's even more awesome when you write your own database extensions 😉

The repo adds four aggregator extensions and three extractor extensions:

- **Aggregators**
  - [COUNT_CHARS.groovy](https://github.com/Bilbottom/pycharm-extensions/blob/main/pycharm-extensions/data/aggregators/COUNT_CHARS.groovy)
  - [COUNT_DISTINCT.groovy](https://github.com/Bilbottom/pycharm-extensions/blob/main/pycharm-extensions/data/aggregators/COUNT_DISTINCT.groovy)
  - [COUNT_NULLS.groovy](https://github.com/Bilbottom/pycharm-extensions/blob/main/pycharm-extensions/data/aggregators/COUNT_NULLS.groovy)
  - [HAS_BAD_CHARS.groovy](https://github.com/Bilbottom/pycharm-extensions/blob/main/pycharm-extensions/data/aggregators/HAS_BAD_CHARS.groovy)
- **Extractors**
  - [Jira-Server.md.groovy](https://github.com/Bilbottom/pycharm-extensions/blob/main/pycharm-extensions/data/extractors/Jira-Server.md.groovy)
  - [One-Row.sql.groovy](https://github.com/Bilbottom/pycharm-extensions/blob/main/pycharm-extensions/data/extractors/One-Row.sql.groovy)
  - [SQL-Where.sql.groovy](https://github.com/Bilbottom/pycharm-extensions/blob/main/pycharm-extensions/data/extractors/SQL-Where.sql.groovy)

---

## [<img alt="Microsoft Excel" height="16px" src="https://www.microsoft.com/favicon.ico"> Custom Excel Add-In](https://github.com/Bilbottom/vba-projects/tree/main/personal-toolkit)

<span style="color:grey" size=1>[https://github.com/Bilbottom/vba-projects/tree/main/personal-toolkit](https://github.com/Bilbottom/vba-projects/tree/main/personal-toolkit)</span>

Excel will never go away... So let's enrich it with some quality-of-life features wrapped up into a handy custom ribbon tab (in addition to the millions of features that Excel already has).

[//]: # "Uncomment once the repo is no longer private"
[//]: # '<div style="text-align: center;">'
[//]: #
[//]: # '<img alt="personal-toolkit-ribbon" src="https://raw.githubusercontent.com/Bilbottom/vba-projects/main/personal-toolkit/personal-toolkit-ribbon.png"/>'
[//]: #
[//]: # "</div>"

The features are built using VBA, and the custom ribbon tab is added using the **Office RibbonX Editor** available at:

- [https://github.com/fernandreu/office-ribbonx-editor](https://github.com/fernandreu/office-ribbonx-editor)

---

## [📘 VBA Guide](https://github.com/Bilbottom/vba-guide)

<span style="color:grey" size=1>[https://github.com/Bilbottom/vba-guide](https://github.com/Bilbottom/vba-guide)</span>

> This will probably not be updated any more

Can you tell that I like VBA? Well, I want you to like it too: this is a reference material for getting started with VBA. The guide is written in LaTeX, but you can find the latest compiled version at:

- [https://github.com/Bilbottom/vba-guide/blob/main/compiled/vba-guide.pdf](https://github.com/Bilbottom/vba-guide/blob/main/compiled/vba-guide.pdf)

It was originally written for some former colleagues and has been slightly adapted for a more general audience, but probably not enough. If you want to see some VBA videos, I strongly recommend [the WiseOwl YouTube](https://www.youtube.com/@WiseOwlTutorials) tutorials:

- [https://youtube.com/playlist?list=PLNIs-AWhQzckr8Dgmgb3akx_gFMnpxTN5](https://youtube.com/playlist?list=PLNIs-AWhQzckr8Dgmgb3akx_gFMnpxTN5)
- [https://youtube.com/playlist?list=PLNIs-AWhQzckV9rAM3yv8ym4pioIMA0UR](https://youtube.com/playlist?list=PLNIs-AWhQzckV9rAM3yv8ym4pioIMA0UR)

---

## [🌍 SQL Schema Models](https://github.com/Bilbottom/sql-schema-models)

<span style="color:grey" size=1>[https://github.com/Bilbottom/sql-schema-models](https://github.com/Bilbottom/sql-schema-models)</span>

Since I work with data all day every day, this is a start at some generalised data models.

For example, most databases (at least, analytical ones) benefit from having some calendar tables, also sometimes referred to as a "date dimension" from when they were built into the Kimball star schema architecture.

This is also a chance for me to just practise data modelling and data generation, so don't take these models too seriously.

---

## [💰 Loan Calculations](https://github.com/Bilbottom/loan-calcs)

<span style="color:grey" size=1>[https://github.com/Bilbottom/loan-calcs](https://github.com/Bilbottom/loan-calcs)</span>

I worked in Finance for 4 years and spent a lot of time working with loans. There are loads of helpful calculations to go with them, so this is a place to both document them and to also expose them through Python classes.

Mainly another opportunity for me to play around with OOP (mainly inheritance in this case) and to have fun with some maths.

---

## [🃏 Blackjack Emulator](https://github.com/Bilbottom/blackjack)

<span style="color:grey" size=1>[https://github.com/Bilbottom/blackjack](https://github.com/Bilbottom/blackjack)</span>

Blackjack can be a fun casino game to play, especially when you win. This is an attempt to build Blackjack with Python just to get familiar with OOP concepts.

---

## [🔁 Mathematics Textbook on Algebraic Permutations](https://github.com/Bilbottom/permutations)

<span style="color:grey" size=1>[https://github.com/Bilbottom/permutations](https://github.com/Bilbottom/permutations)</span>

> Not really in development any more (and not even finished)

There's a branch of Maths called Linear Algebra, and one of the concepts that you can study is _permutations_:

- [https://en.wikipedia.org/wiki/Permutation](https://en.wikipedia.org/wiki/Permutation)

They're a pretty simple concept, but learning about them becomes a pain because there's a lot of different --- and in some places, contradictory --- notation used to describe them and what they can do.

The purpose of this project was to show all the different notations, where they differ, and how to solve problems using each of them.

---

## [🧑‍🎓 Master's Dissertation Graphs](https://github.com/Bilbottom/ma5p1-dissertation-code)

<span style="color:grey" size=1>[https://github.com/Bilbottom/ma5p1-dissertation-code](https://github.com/Bilbottom/ma5p1-dissertation-code)</span>

> Originally an R project, this has been reduced and reworked as a Python project

As part of my dissertation, I was exploring ["point-line duality"](<https://en.wikipedia.org/wiki/Duality_(projective_geometry)>) -- and it was easiest to do this by drawing up the points and the lines using a computer.

One of the images has also been used as the thumbnail for the song **Perdidos en la Multitud** by the Argentinian musician **Aroldo De Souza**:

- [https://www.instagram.com/aroldo_de_souza/](https://www.instagram.com/aroldo_de_souza/)
- [https://open.spotify.com/track/5XXUJO0EzWpjkRpvrkZkt1?si=2ebc3c24556b44ff](https://open.spotify.com/track/5XXUJO0EzWpjkRpvrkZkt1?si=2ebc3c24556b44ff)

The description to go with this image is:

> In Mathematics, there is a concept of point-line duality: that is, for a point on a graph there is a corresponding line called its _dual_. The dual of the point `(a, b)` is the set of points `{(x, y)}` such that `ax + by = 0`, and we call the set of points a _line_.
>
> An interesting consequence of this duality is that if a collection of points all line on a straight line, then their dual lines will all intersect in the same place. The image is the duals of some points on the cubic curve `y = x^3`. The points on the cubic curve have been selected so that there are many sets of 3 points that all lie on the same line (such as `(-1, -1)`, `(0, 0)`, and `(1, 1)`) which means that their duals (the lines) have many intersections of exactly three lines.

If you look carefully, you'll also see that the image has been set as the tab icon for this page 😉

<br>
<div style="text-align: center;">

<img alt="cubic-graph-61" src="favicon.ico"/>

</div>
