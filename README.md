# ALAN by Examples

[![Build Status][Travis Badge]][Travis LInk]


- https://github.com/alan-if/alan-by-examples

A collection of examples to learn [ALAN IF] v3 — the Alan Interactive Fiction Language. Provided as a public service by the [Alan Interactive Fiction Development team].

Created by [Tristano Ajmone] in June 2, 2019.

    Alan SDK v3.0beta6

-----

**Table of Contents**

<!-- MarkdownTOC autolink="true" bracket="round" autoanchor="false" lowercase="only_ascii" uri_encoding="true" levels="1,2,3" -->

- [Project Contents](#project-contents)
- [About ALAN](#about-alan)
- [About This Project](#about-this-project)
- [Project Organization](#project-organization)
- [Contributing](#contributing)
- [Project License](#project-license)
- [Third Party Assets Licenses](#third-party-assets-licenses)
    - [Alan SDK License](#alan-sdk-license)
    - [Alan Project Builder](#alan-project-builder)
- [External Links](#external-links)
    - [Documentation and Tutorials](#documentation-and-tutorials)
    - [Code Examples](#code-examples)
    - [Libraries](#libraries)
    - [Editors](#editors)
    - [Miscellanea](#miscellanea)

<!-- /MarkdownTOC -->

-----

# Project Contents

- [`/_dev/`](./_dev/) — Project maintainers' assets:
    + [`/AlanSDK/`](./_dev/AlanSDK/) — Alan SDK binaries for Windows (for toolchain automation).
- [`/recipes/`](./recipes/) — _The Alan Recipe Book_.
- [`ABuilder.exe`](./ABuilder.exe) — tests and builds the project (locally and on GitHub via [Travis CI])
- [`ABuilderLICENSE`](./ABuilderLICENSE) — MIT License for `ABuilder.exe`.
- [`CONTRIBUTING.md`](CONTRIBUTING.md) — _Contributors' Guidelines_.
- [`LICENSE`](./LICENSE) — MIT License.

# About ALAN

The Alan Interactive Fiction Language is a powerful tool for developing text adventure games. What makes ALAN unique amongst the IF authoring tools is that it doesn't provide a standard library (although various libraries are available if you need one, like the **[ALAN Standard Library]** by [Anssi Räisänen]); instead, ALAN provides all the basic tools for building your own adventure from the ground up, thus allowing you the uttermost freedom in tailoring your own adventure world and model.

This also means that ALAN is a truly locale-agnostic tool (i.e. it doesn't enforce any particular spoken language) because although it natively supports English, Swedish and German default message responses, you are free to override these messages with your own. Sine ALAN doesn't provide any verbs definitions, you won't have to translate any verbs to your native language, instead you'll be free to write your own verbs according to needs.

With ALAN being such a flexible and powerful tool, we need to be mindful of [Benjamin "Ben" Parker's] wise [words of advise to his nephew]  (Peter Parker, aka [Spider-Man]):

> With great power there must also come great responsibility.

The above motto holds true for IF authors working with ALAN, for the basic tools offered by the ALAN language can be combined in infinite ways to create a unique text adventure according to needs. The lack of a strict paradigm is both a blessing and a challenge, for you'll need to know how to wisely combine all the available tools offered by the language to maximize results and avoid pitfalls.

# About This Project

Since most constructs of the ALAN language were thought as general purpose tools that can be flexibly adapted to fulfil most text adventures needs, without imposing any predefined paradigm, the best way to learn ALAN is by looking at practical examples by different authors.

This goal of this repository is to provide a wide collection of practical examples — ranging from the basics to more advanced and complex examples — and, most important, this project is community oriented — meaning that anyone can contribute their examples to the project.

Since there are many ways to implement solutions to common IF problems, different authors will have their own coding style and approaches to the various challenges of creating text adventures. The ALAN community is a small and friendly group that values diversity, freedom and group discussion — there are no "benevolent dictators" in the ALAN community, and everyone's voice is heard and taken into account whenever discussing new features, projects and change. Everyone's contribution is important to the ALAN community.

# Project Organization

The project being in its early stages, we'd rather leave its structural organization open for now, and let it be shaped by the actual contributions.
As examples start to flow in, we'll be able to organize them into categories by subfoldering them in a way to make consultation easier.

Currently, there's only the [`recipes/`](./recipes/) directory tree, hosting _[The Alan Recipe Book]_; but more directories will be added as the need arises.

# Contributing

- [`CONTRIBUTING.md`](CONTRIBUTING.md)

Anyone can contribute examples to the project, via Git and GitHub.
By contributing your examples to this project, you are donating your code to the Alan community under the MIT License (although it will still be attributed to you, and you'll retain its paternity).

More information on how to submit contents to the project can be found in the _[Contributors' Guidelines]_ document.

For questions and discussions, you can either:

- [open an issue] — for all matters directly concerning this repository.
- post on the [ALAN Yahoo Group] — for all discussion involving the ALAN community.


# Project License

- [`LICENSE`](./LICENSE)

The Alan by Example project is released under the MIT License.
All examples code in this project belong to the [Alan Interactive Fiction Development team] — i.e. are donated to the Alan community.

```
MIT License
-----------

Copyright (c) 2019 Alan Interactive Fiction Development team:
https://github.com/alan-if

Permission is hereby granted, free of charge, to any person
obtaining a copy of this software and associated documentation
files (the "Software"), to deal in the Software without
restriction, including without limitation the rights to use,
copy, modify, merge, publish, distribute, sublicense, and/or sell
copies of the Software, and to permit persons to whom the
Software is furnished to do so, subject to the following
conditions:

The above copyright notice and this permission notice shall be
included in all copies or substantial portions of the Software.

THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND,
EXPRESS OR IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES
OF MERCHANTABILITY, FITNESS FOR A PARTICULAR PURPOSE AND
NONINFRINGEMENT. IN NO EVENT SHALL THE AUTHORS OR COPYRIGHT
HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER LIABILITY,
WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING
FROM, OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR
OTHER DEALINGS IN THE SOFTWARE.
```

The above license doesn't apply to third party assets which might be included in this project, which are governed by their own license terms and copyright notice — as indicated by their license files, which shall be included along with those assets, as well as being mentioned in this section.

# Third Party Assets Licenses

The project includes the following assets created by third parties, each governed by its own license terms.

## Alan SDK License

- [`/_dev/AlanSDK/`](./_dev/AlanSDK/)

The above folder contains the Windows executables of the [Alan SDK], which are released under the terms of the Artistic License 2.0:

- [`/_dev/AlanSDK/COPYING`](./_dev/AlanSDK/COPYING)

## Alan Project Builder

- `ABuilder.exe`
- [`ABuilderLICENSE`](./ABuilderLICENSE) — MIT License.

The __[ALAN Builder]__ tool was created by Tristano Ajmone and donated to the [Alan Interactive Fiction Development team] under MIT License.

```
MIT License

Copyright (c) 2019 Tristano Ajmone and the Alan IF Development team
https://github.com/alan-if/Alan-Builder

Permission is hereby granted, free of charge, to any person obtaining a copy
of this software and associated documentation files (the "Software"), to deal
in the Software without restriction, including without limitation the rights
to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
copies of the Software, and to permit persons to whom the Software is
furnished to do so, subject to the following conditions:

The above copyright notice and this permission notice shall be included in all
copies or substantial portions of the Software.

THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR
IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,
FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
SOFTWARE.
```

Please, note that the [`ABuilderLICENSE`](./ABuilderLICENSE) file contains additional licenses for [third party components used by the PureBasic compiler], which _must_ be included with any distribution of the __Alan Builder__ application in compiled binary format (but not necessarily so if only the source code is being distributed).

The full source code (in [PureBasic]) can be found on the __ALAN Builder__ repository:

- https://github.com/alan-if/Alan-Builder


# External Links

- [www.AlanIF.se][ALAN] — the ALAN website.
- [ALAN Yahoo Group] — for community help, announcements and discussions.
- [ALAN sources][ALAN Bitbucket] — source code repository on Bitbucket.

## Documentation and Tutorials

- [Alan Docs] — GitHub repository for Alan documentation.
- _[The ALAN Manual]_ — online-readable version of the latest _ALAN Adventure Language Reference Manual_.
- _[Alan Cookbook v2]_ — by [Anssi Räisänen].
- _[The Alan Beginner's Guide]_ — by Michael Arnaud (2006). [Tutorial source files available](https://github.com/alan-if/alan-docs/tree/master/alanguide/alanguide-code).
- _[Alan IDE Reference Guide]_ — by Robert DeFord (2018).

## Code Examples

- [Samples & examples for alan v3] — on ALAN website.


## Libraries

- [ALAN Standard Library] — by [Anssi Räisänen], GitHub repository.
- [ALAN Library v0.6.2] — an earlier (but still working) library (2002–2007), mainly used to compile legacy adventures.
- [ALAN StdLibLab] — experimental playground for variations on the Alan StdLib.
- [Alan Italian] — Italian port of the Alan StdLib.

## Editors

- [AlanIDE] — a complete Alan Integrated Development Environment, built in Java/Eclipse by Alan developer [Thomas Nilefalk]. For more info, see:
    + [AlanIDE info page].
    + _[Alan IDE Reference Guide]_ — by Robert DeFord (2018), PDF document.
    + [AlanIDE sources] — JAVA source files, on GitHub.
- [Sublime Alan] — [Sublime Text 3] package for Alan 3 (working Alpha).


## Miscellanea

- [Alan Goodies] — A collection of assorted assets for Alan.

<!-----------------------------------------------------------------------------
                               REFERENCE LINKS
------------------------------------------------------------------------------>

[Benjamin "Ben" Parker's]: https://en.wikipedia.org/wiki/Uncle_Ben "Learn more about Uncle Ben on Wikipedia"
[words of advise to his nephew]: https://en.wikipedia.org/wiki/With_great_power_comes_great_responsibility "See Wikipedia page on the motto 'With great power comes great responsibility'"
[Spider-Man]: https://en.wikipedia.org/wiki/Spider-Man "See Wikipedia page on Spider-Man"

<!-- Travis CI -->

[Travis CI]: https://travis-ci.com/ "Visit Travis CI website"
[Travis Badge]: https://travis-ci.org/alan-if/alan-by-examples.svg
[Travis LInk]: https://travis-ci.org/alan-if/alan-by-examples

<!-- ALAN -->

[ALAN]: https://www.alanif.se/ "Visit the ALAN website"
[ALAN IF]: https://www.alanif.se/ "Visit the ALAN website"
[ALAN Yahoo Group]: https://groups.yahoo.com/neo/groups/alan-if/info "Visit the Alan-IF group on Yahoo"
[ALAN Bitbucket]: https://bitbucket.org/alanif/alan/ "Visit the ALAN source repository on Bitbucket"

[Alan SDK]: https://www.alanif.se/download-alan-v3/development-kits "Go to the Alan SDK section of the ALAN website"

<!-- AlanIDE -->

[AlanIDE]: https://www.alanif.se/download-alan-v3/alanide "Go to the AlanIDE download page on Alan website"
[AlanIDE info page]: https://www.alanif.se/information/alanide/alanide-intro "View the AlanIDE information page on Alan website"
[Alan IDE Reference Guide]: https://github.com/alan-if/alan-docs/blob/master/ideguide/ideguide.pdf "Get the 'Alan IDE Reference Guide' (PDF format)"
[AlanIDE sources]: https://github.com/thoni56/alanide "Visit the AlanIDE source repository on GitHub"

<!-- Alan StdLib -->

[ALAN Standard Library]: https://github.com/AnssiR66/AlanStdLib/ "Visit the official repository of the ALAN Standard Library on GitHub"

[Artistic License 2.0]: https://opensource.org/licenses/Artistic-2.0

<!-- Alan misc -->

[Alan Goodies]: https://github.com/tajmone/alan-goodies "Visit the Alan Goodies project on GitHub"
[ALAN Library v0.6.2]: https://github.com/tajmone/alan-goodies/tree/master/libs "View ALAN Lib v0.6.2 at the 'Alan Goodies' project"
[ALAN StdLibLab]: https://github.com/tajmone/Alan-StdLibLab "Visit the ALAN StdLibLab project on GitHub"
[Alan Italian]: https://github.com/tajmone/Alan3-Italian "Visit the Alan Italian project on GitHub"
[Sublime Alan]: https://github.com/tajmone/sublime-alan "Visit the Sublime Alan project on GitHub"
[ALAN Builder]: https://github.com/alan-if/Alan-Builder "Visit the ALAN Builder project on GitHub"

<!-- Alan docs & tutorials -->

[Alan Docs]: https://github.com/alan-if/alan-docs "Visit the Alan Docs project on GitHub"
[The ALAN Manual]: http://htmlpreview.github.io/?https://github.com/alan-if/alan-docs/blob/master/manual/manual.html "Live HTML preview of the ALAN Manual"
[Alan Cookbook v2]: https://www.alanif.se/download-alan-v3/all-downloads/documentation/alan-cookbook-v2 "Go to the 'Alan Cookbook' download page on Alan website"

[The Alan Beginner's Guide]: http://htmlpreview.github.io/?https://github.com/alan-if/alan-docs/blob/master/alanguide/alanguide.html "Live HTML preview of the Alan Beginner's Guide"

[Samples & examples for alan v3]: https://www.alanif.se/information/samples

<!-- PureBasic -->

[PureBasic]: https://www.purebasic.com "Visit PureBasic website."
[third party components used by the PureBasic compiler]:https://www.purebasic.com/documentation/reference/license_application.html "Read full details on PureBasic online documentation"

<!-- 3r party tools -->

[Sublime Text 3]: https://www.sublimetext.com/ "Visit Sublime Text website"

<!-- repo xrefs -->

[open an issue]: https://github.com/tajmone/alan-by-examples/issues/new "Click to open an issue"
[Contributors' Guidelines]: ./CONTRIBUTING.md
[The Alan Recipe Book]: ./recipes/README.md "Go to the The Alan Recipe Book"

<!-- people -->

[Alan Interactive Fiction Development team]: https://github.com/alan-if "Visit the Alan Interactive Fiction Development team organization on GitHub"

[Anssi Räisänen]: https://github.com/AnssiR66 "View Anssi Räisänen's GitHub profile"
[Tristano Ajmone]: https://github.com/tajmone "View Tristano Ajmone's GitHub profile"
[Thomas Nilefalk]: https://github.com/thoni56 "View Thomas Nilefalk's GitHub profile"


<!-- EOF -->