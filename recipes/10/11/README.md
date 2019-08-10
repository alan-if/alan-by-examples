# 10.11. Mathematics

Inspired by same-named section of _[The Inform Recipe Book]_.


-----

**Table of Contents**

<!-- MarkdownTOC autolink="true" bracket="round" autoanchor="false" lowercase="only_ascii" uri_encoding="true" levels="1,2,3" -->

- [Introduction](#introduction)
- [Available Examples](#available-examples)
    - [Maths Rigorosum](#maths-rigorosum)
- [Implementation Overview](#implementation-overview)
    - [Maths Limitations in Alan](#maths-limitations-in-alan)

<!-- /MarkdownTOC -->

-----

# Introduction

Generally speaking, most interactive fiction works don't involve complex mathematical calculations, but there are exceptions.

Whether you'll need to rely on maths for internal calculations of the adventure (e.g. to implement some simulation algorithm for the sake of realism), or to provide the player with some verbs to carry out calculations (e.g. for maths-oriented puzzles), in either case you'll have to resort to some custom hacks to circumvent some [limitations of the Alan language] regarding numerical types and mathematical operators.

[limitations of the Alan language]: #maths-limitations-in-alan "Jump to document section"

# Available Examples

## Maths Rigorosum

- [`maths-rigorosum.alan`](./maths-rigorosum.alan)
- [`maths-rigorosum.a3log`](./maths-rigorosum.a3log)

This example illustrates how to use the `integer` literal class to implement verbs to carry out the four elementary arithmetic operations, and how to emulate the modulo operator in Alan.

# Implementation Overview

Let's go through the technical aspects of working with maths in Alan adventures. 

## Maths Limitations in Alan

When dealing with math, you have to consider the following limitations in Alan:

- __integers only__ — Any decimal fractions resulting from divisions will be dropped (e.g. 3/2 &rarr; 1).
- __limited operators__ — Only the elementary operators for addition (`+`), subtraction (`-`), multiplication (`*`) and division (`/`) are available — there are no modulo (`%`) or power (`^`) operators.
- __input limitations__ — The player can't use operator characters in his commands, for the parser will reject them. 

You must bare in mind that all of the above limitations are in line with Alan philosophy of authoring simplicity and its emphasis on prose, and that the language is flexible enough to allow circumventing those limitations via some smart hacks.

As demonstrated in the examples in this section, the lack of a modulo operator can easily be worked around using `Event`s as functions to calculate the remainder of divisions; and decimal fractions can also be implemented through code.

As for the player input limitations, you only need to translate arithmetic formulas into prose — i.e. instead of expecting the player to type:

    > calculcate 4 * 2

reformulate the verb/command into plain prose:

    > calculcate 4 times 2

<!-----------------------------------------------------------------------------
                               REFERENCE LINKS
------------------------------------------------------------------------------>

[The Inform Recipe Book]: http://inform7.com/book/RB_10_11.html "View section '10.11. Mathematics' of 'The Inform Recipe Book' online"


<!-- EOF -->
