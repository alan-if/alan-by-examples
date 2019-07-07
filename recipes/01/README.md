# 1. How to Use The Recipe Book

Some guidelines on how to use the Alan recipes, the ultimate goal of this project, and how to contribute your own examples.


-----

**Table of Contents**

<!-- MarkdownTOC autolink="true" bracket="round" autoanchor="false" lowercase="only_ascii" uri_encoding="true" levels="1,2,3" -->

- [Introduction](#introduction)
- [Project Status](#project-status)
- [Contents Organization](#contents-organization)
- [The Recipes](#the-recipes)
- [Contributing](#contributing)

<!-- /MarkdownTOC -->

-----

# Introduction

_The Alan Recipe Book_ is heavily inspired by _[The Inform Recipe Book]_ that ships with [Inform 7] — it's structured the same way.
Although the two languages are quite different in nature, the _[The Inform Recipe Book]_ is a valuable resource for it approaches the common problems of IF authoring in a well organized manner, and has been developed in the course of many years and around users' feedback.

The goal of _The Alan Recipe Book_ is to present Alan-specific solutions to the same general problems presented in _[The Inform Recipe Book]_, for the challenges faced by IF authors are the same, regardless of the authoring tool and language.
Obviously, the actual Alan examples will differ from their [Inform 7] counterparts, and the goal is not to recreate the same exact manual, but only to keep the same structural organization — which has the added benefit of providing familiarity for those coming to Alan from [Inform 7].

# Project Status

_The Alan Recipe Book_ is still in its very early stages, but we hope that through users' contributions it will eventually grow in time and ultimately become a full-fledged book — when this happens, we'll actually publish it as a readable eBook with examples sources and transcripts.

# Contents Organization

Examples (aka _recipes_) are organized by topic, according to the book structure illustrated in the [Table of Contents].

The book is structured into a directory tree where folders are named like the chapter number they represent, and sections are subfolders therein, also named according to their section number.
Every chapter and section has a README file introducing the covered topics and providing links to the examples:

- `01/` — 1. How to Use The Recipe Book
    + `README.md`
- `02/` — 2. Adaptive Prose
    + `README.md`
    + `01/` — 2.1. Varying What Is Written
        * `README.md`
        * examples sources and transcripts...
    + `02/` — 2.2. Varying What Is Read
        * `README.md`
        * examples sources and transcripts...
    + etc.
- etc.

Some examples might fit multiple categories/sections, in which case the example will be hosted in the most pertinent section, and a link will be provided in all the other sections.

# The Recipes

Every recipe is an example showing how to achieve a given task in pure Alan (i.e. without external dependencies like modules or libraries).

Ideally, a recipe should be a minimum viable example on how to achieve any given task — i.e. its code should be as simple as possible, so that the reader can easily study it without distractions.
A recipe doesn't have to be a full fledged example, a proof of concept is more than enough for learning purposes.

More advanced recipes are also welcome, alongside with their minimum viable examples, to provide a richer example and demonstrate how to handle more complex scenarios.
As a general rule, advanced recipes should only be provided after a minimum viable example, so that the reader can study a topic in order of complexity.

Every recipe comes with a sample transcript and, optionally, it might have an introductory document too, where its author shares some considerations on the code and techniques used.
All recipes file are same named, differing only in their extension:

- `<filename>.alan` — recipe source code.
- `<filename>.a3sol` — recipe commands script (aka _solution_).
- `<filename>.a3log` — recipe transcript (generated from the `.a3sol` file).
- `<filename>.md` — recipe documentation (optional).

# Contributing

Feel free to contribute your own recipes to _The Alan Recipe Book_. 

Contributing should be rather intuitive by looking at the existing examples.
For more info, see the _[Contributors' Guidelines]_ and feel free to ask any questions by [opening an issue] or posting to the [ALAN Yahoo Group].

<!-----------------------------------------------------------------------------
                               REFERENCE LINKS
------------------------------------------------------------------------------>

[Inform 7]: http://inform7.com "Visit Inform 7 website"
[The Inform Recipe Book]: http://inform7.com/book/RB_1_1.html "View 'The Inform Recipe Book' online"

[ALAN Yahoo Group]: https://groups.yahoo.com/neo/groups/alan-if/info "Visit the Alan-IF group on Yahoo"

<!-- repo xrefs -->

[opening an issue]: https://github.com/tajmone/alan-by-examples/issues/new "Click to open an issue"

[Table of Contents]: ../README.md#table-of-contents
[Contributors' Guidelines]: ../../CONTRIBUTING.md

<!-- EOF -->