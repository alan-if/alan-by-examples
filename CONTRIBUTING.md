# Contributors' Guidelines

A few guidelines for submitting contents to the __ALAN by Examples__ projects.

> __WIP NOTE__ — These guidelines are still work in progress.
> [Suggestions are welcome].

-----

**Table of Contents**

<!-- MarkdownTOC autolink="true" bracket="round" autoanchor="false" lowercase="only_ascii" uri_encoding="true" levels="1,2,3" -->

- [Introduction](#introduction)
    - [Important License Notice](#important-license-notice)
    - [Getting Help and Support](#getting-help-and-support)
    - [About the Guidelines](#about-the-guidelines)
- [Conventions](#conventions)
    - [File and Folders Names](#file-and-folders-names)
    - [README Files](#readme-files)
    - [Submitting Examples](#submitting-examples)
        - [Examples Documentation](#examples-documentation)
    - [Testing Before Submitting](#testing-before-submitting)

<!-- /MarkdownTOC -->

-----

# Introduction

Anyone can contribute examples to the project, either via:

- __eMail__ — i.e. sending your example to <tajmone@gmail.com>.
- __Git and GitHub__ — i.e. by creating a pull request on the repository.

The latter contribution method is the preferred one, but sending the source files via email might be the simplest solution for many Alan users.

If you decide to contribute via [Git], then you'll need to stick to the following guidelines, whereas eMail contributors only have to focus on creating the example adventure, and the project maintainers will deal with the rest (you should still read the guidelines though, to get a general idea of how contributions are expected to be).

## Important License Notice

By contributing your examples to this project, you are donating your code to the Alan community under the [MIT License] (although it will still be attributed to you, and you'll retain its paternity).

## Getting Help and Support

This being a community project, feel free to ask for help if you need support setting up Git, or with any technical problems you might be facing.

For questions and discussions, you can either:

- [open an issue] — for all matters directly concerning this repository.
- post on the [ALAN Yahoo Group] — for all discussion involving the ALAN community.


## About the Guidelines

The goal of these guidelines is to preserve consistency across the project, in order to simplify its maintenance.

Some guidelines concerning technical issues might be stricter than others, for they take into consideration cross-platform portability of the examples; other guidelines are just arbitrary conventions which are open to discussion and revision.

# Conventions

## File and Folders Names

As a general rule, try to keep all file names in lower case, unless there is a good reasons for not doing so.

For cross-platform portability, avoid using spaces in file and folder names, as well as any characters unsupported by any OS for which Alan is available.
As a replacement for the space character, use an hyphen (`-`), or an underscore (`_`) — the former is preferable, for consistency reasons.

## README Files

For consistency sake, all README files must be in GFM ([GitHub Flavored Markdown]) with the `.md` extension.
GFM is one of the most popular markdown flavours, and the _de facto_ standard on GitHub.

## Submitting Examples

We'd love to see your examples contributed to the project.
Here are a few (hopefully simple) guidelines on how to submit your examples.

Every Alan example _must_:

- have the `.alan` extension.
- be fully standalone (i.e. don't depend on external libraries).
- must be submitted together with:
    + a sample command script (extension `.a3sol`).
    + the resulting transcript (extension `.a3log`).
- can optionally come with a documentation file, which must formatted in:
    + [GitHub Flavored Markdown]  (extension `.md`).
    + or one of the alternative syntaxes mentioned below.
- all examples file must be same named, differing only in their extension:
    + `<filename>.alan` — example source code.
    + `<filename>.a3sol` — example commands script (aka _solution_).
    + `<filename>.a3log` — example transcript (generated from the `.a3sol` file).
    + `<filename>.md` — example documentation (optional).
- all `.alan`, `.a3sol` and `.a3log` files must be encoded in ISO-8859-1.


The `.a3sol` and `.a3log` file extensions for commands scripts and transcripts are arbitrarily choices, resembling the Alan 3 file naming convention.

The above file naming conventions are important for the automation tool chain that needs to verify integrity of all project files and update their contents whenever a new Alan release is available — i.e. they are _not_ negotiable.


### Examples Documentation

As mentioned above, an example might come with an explanatory document.
The preferred choice for documentation formatting is GFM ([GitHub Flavored Markdown]), which is the _de facto_ standard on GitHub.

If you are more familiar with other markup syntaxes, you may use anyone of the syntaxes listed in the table below, using the indicated file extension:

|       markup       |     flavour      |  extension  |
|--------------------|------------------|-------------|
| [AsciiDoc]         | Asciidoctor Ruby | `.asciidoc` |
| [Markdown]         | GFM              | `.md`       |
| [ReStructuredText] |                  | `.rst `     |
| [Textile]          |                  | `.textile`  |

Although the above table doesn't contain all of the [lightweight markup syntaxes supported by GitHub], we've restricted the choice to the most commonly used syntaxes in order to avoid having to deal with a confusion of languages of Babylonian proportions.

The proposed file extensions are important for both consistency as well as for the automation toolchain — again, _not_ negotiable.

__Free-form plaintext documentation can't be accepted in the project!__

Project maintainers need to be able to convert all documentation to and from the various markup formats at any stage, without having to manually format documents that don't adhere to well established standards.
Piling up plaintext documentation would eventually cause a bottleneck in the project, which will ultimately require a huge amount of work to fix.
Since it has become standard practice on any [Git] related project to adopt a lightweight markup syntax for its documentation, we ask you to stick to one of the above markup syntaxes (they are all easy to learn, and there are hundreds of editors extensions to support them). 

## Testing Before Submitting

- `ABuilder.exe` — Build-test binary tool for Windows.

The repository includes some Windows executables to test locally that all examples and their commands scripts actually work and meet some basic standards.

Before submitting an example adventure, first check that it passes all the build tests locally by executing the `ABuilder.exe` tool found in the project root.

> __NOTE__ — Currently the project only ships with binaries to test under Windows OS.
> Binaries for other OSs shall be made available on request, if needed.


<!-----------------------------------------------------------------------------
                               REFERENCE LINKS
------------------------------------------------------------------------------>
<!-- ALAN -->

[ALAN Yahoo Group]: https://groups.yahoo.com/neo/groups/alan-if/info "Visit the Alan-IF group on Yahoo"

<!-- repo xrefs -->

[open an issue]: https://github.com/tajmone/alan-by-examples/issues/new "Click to open an issue"
[Suggestions are welcome]: https://github.com/tajmone/alan-by-examples/issues/new "Click to open an issue"
[MIT License]: ./LICENSE "View the MIT License file"

<!-- external references -->

[GitHub Flavored Markdown]: https://guides.github.com/features/mastering-markdown/ "Learn more about GFM"
[lightweight markup syntaxes supported by GitHub]: https://github.com/github/markup#markups "See the full list of markups supported by GitHub"

<!-- markup syntaxes -->

[AsciiDoc]: http://asciidoctor.org/ "Learn more about Asciidoctor"
[Markdown]: https://guides.github.com/features/mastering-markdown/ "Learn more about GitHub Flavored Markdown"
[ReStructuredText]: http://docutils.sourceforge.net/rst.html "Learn more about ReStructuredText"
[Textile]: https://www.promptworks.com/textile "Learn more about Textile"

<!-- 3rd party tools -->

[Git]: https://git-scm.com "Visit Git website"

<!-- EOF -->