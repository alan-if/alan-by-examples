# ALAN by Examples

- https://github.com/alan-if/alan-by-examples

A collection of examples to learn [ALAN IF] v3 — the Alan Interactive Fiction Language. Provided as a public service by the [Alan Interactive Fiction Development team].

Created by [Tristano Ajmone] in June 2, 2019.

-----

**Table of Contents**

<!-- MarkdownTOC autolink="true" bracket="round" autoanchor="false" lowercase="only_ascii" uri_encoding="true" levels="1,2,3" -->

- [About ALAN](#about-alan)
- [About This Project](#about-this-project)
- [Project Organization](#project-organization)
- [Contributing](#contributing)
- [License](#license)

<!-- /MarkdownTOC -->

-----

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

The project being in its early stages, we'd rather leave its structural organization open for now, and let it be shaped by the actual contributions. As examples start to flow in, we'll be able to organize them into categories by subfoldering them in a way to make consultation easier.

# Contributing

Anyone can contribute examples to the project, via Git and GitHub.
By contributing your examples to this project, you are donating your code to the Alan community under the MIT License (although it will still be attributed to you, and you'll retain its paternity).

For questions and discussions, you can either:

- [open an issue] — for all matters directly concerning this repository.
- post on the [ALAN Yahoo Group] — for all discussion involving the ALAN community.


# License

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


<!-----------------------------------------------------------------------------
                               REFERENCE LINKS
------------------------------------------------------------------------------>

[Benjamin "Ben" Parker's]: https://en.wikipedia.org/wiki/Uncle_Ben "Learn more about Uncle Ben on Wikipedia"
[words of advise to his nephew]: https://en.wikipedia.org/wiki/With_great_power_comes_great_responsibility "See Wikipedia page on the motto 'With great power comes great responsibility'"
[Spider-Man]: https://en.wikipedia.org/wiki/Spider-Man "See Wikipedia page on Spider-Man"


<!-- ALAN -->

[ALAN]: https://www.alanif.se/ "Visit the ALAN website"
[ALAN IF]: https://www.alanif.se/ "Visit the ALAN website"
[ALAN Yahoo Group]: https://groups.yahoo.com/neo/groups/alan-if/info "Visit the Alan-IF group on Yahoo"

<!-- Alan StdLib -->

[ALAN Standard Library]: https://github.com/AnssiR66/AlanStdLib/ "Visit the official repository of the ALAN Standard Library on GitHub"

[Artistic License 2.0]: https://opensource.org/licenses/Artistic-2.0

<!-- repo xrefs -->

[open an issue]: https://github.com/tajmone/alan-by-examples/issues/new "Click to open an issue"

<!-- people -->

[Alan Interactive Fiction Development team]: https://github.com/alan-if "Visit the Alan Interactive Fiction Development team organization on GitHub"

[Anssi Räisänen]: https://github.com/AnssiR66 "View Anssi Räisänen's GitHub profile"
[Tristano Ajmone]: https://github.com/tajmone "View Tristano Ajmone's GitHub profile"

<!-- EOF -->