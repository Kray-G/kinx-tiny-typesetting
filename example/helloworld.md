% Hello Kinx Tiny Typesetting
% Your name
% September 26, 2021

# Greeting
hello, world

# Unicode & Arrows

## Unicode Examples

`\\unicode{code}` is available.

|   Code   |     Character     |   Code   |     Character     |   Code   |     Character     |   Code   |     Character     |
| :------: | :---------------: | :------: | :---------------: | :------: | :---------------: | :------: | :---------------: |
| `0x2600` | \\unicode{0x2600} | `0x2608` |                   | `0x2660` | \\unicode{0x2660} | `0x2668` | \\unicode{0x2668} |
| `0x2601` | \\unicode{0x2601} | `0x2609` | \\unicode{0x2609} | `0x2661` | \\unicode{0x2661} | `0x2669` | \\unicode{0x2669} |
| `0x2602` | \\unicode{0x2602} | `0x260A` |                   | `0x2662` | \\unicode{0x2662} | `0x266A` | \\unicode{0x266A} |
| `0x2603` | \\unicode{0x2603} | `0x260B` |                   | `0x2663` | \\unicode{0x2663} | `0x266B` | \\unicode{0x266B} |
| `0x2604` |                   | `0x260C` |                   | `0x2664` | \\unicode{0x2664} | `0x266C` | \\unicode{0x266C} |
| `0x2605` | \\unicode{0x2605} | `0x260D` |                   | `0x2665` | \\unicode{0x2665} | `0x266D` | \\unicode{0x266D} |
| `0x2606` | \\unicode{0x2606} | `0x260E` | \\unicode{0x260E} | `0x2666` | \\unicode{0x2666} | `0x266E` | \\unicode{0x266E} |
| `0x2607` |                   | `0x260F` | \\unicode{0x260F} | `0x2667` | \\unicode{0x2667} | `0x266F` | \\unicode{0x266F} |

|   Code   |     Character     |   Code   |     Character     |   Code   |     Character     |   Code   |     Character     |
| :------: | :---------------: | :------: | :---------------: | :------: | :---------------: | :------: | :---------------: |
| `0x2500` | \\unicode{0x2500} | `0x2508` | \\unicode{0x2508} | `0x2510` | \\unicode{0x2510} | `0x2518` | \\unicode{0x2518} |
| `0x2501` | \\unicode{0x2501} | `0x2509` | \\unicode{0x2509} | `0x2511` | \\unicode{0x2511} | `0x2519` | \\unicode{0x2519} |
| `0x2502` | \\unicode{0x2502} | `0x250A` | \\unicode{0x250A} | `0x2512` | \\unicode{0x2512} | `0x251A` | \\unicode{0x251A} |
| `0x2503` | \\unicode{0x2503} | `0x250B` | \\unicode{0x250B} | `0x2513` | \\unicode{0x2513} | `0x251B` | \\unicode{0x251B} |
| `0x2504` | \\unicode{0x2504} | `0x250C` | \\unicode{0x250C} | `0x2514` | \\unicode{0x2514} | `0x251C` | \\unicode{0x251C} |
| `0x2505` | \\unicode{0x2505} | `0x250D` | \\unicode{0x250D} | `0x2515` | \\unicode{0x2515} | `0x251D` | \\unicode{0x251D} |
| `0x2506` | \\unicode{0x2506} | `0x250E` | \\unicode{0x250E} | `0x2516` | \\unicode{0x2516} | `0x251E` | \\unicode{0x251E} |
| `0x2507` | \\unicode{0x2507} | `0x250F` | \\unicode{0x250F} | `0x2517` | \\unicode{0x2517} | `0x251F` | \\unicode{0x251F} |

## Arrows

`\\arrow{direction}` is also avalilable.

|  Direction   |      Character      |      Direction       |          Character          |
| :----------: | :-----------------: | :------------------: | :-------------------------: |
|    `left`    |    \\arrow{left}    |   `left-and-right`   |   \\arrow{left-and-right}   |
|     `up`     |     \\arrow{up}     |   `right-and-left`   |   \\arrow{right-and-left}   |
|   `right`    |   \\arrow{right}    |    `up-and-down`     |    \\arrow{up-and-down}     |
|    `down`    |    \\arrow{down}    | `left-right-harpoon` | \\arrow{left-right-harpoon} |
| `left-right` | \\arrow{left-right} | `right-left-harpoon` | \\arrow{right-left-harpoon} |
|  `up-down`   |  \\arrow{up-down}   |       `left-x`       |       \\arrow{left-x}       |
|  `left-up`   |  \\arrow{left-up}   |      `right-x`       |      \\arrow{right-x}       |
|  `right-up`  |  \\arrow{right-up}  |    `left-right-x`    |    \\arrow{left-right-x}    |
| `right-down` | \\arrow{right-down} |                      |                             |
| `left-down`  | \\arrow{left-down}  |                      |                             |
# Table

<context label="Table:TableExample"/>
<context caption="Example of Table"/>
<context vline-left="single"/>
<context vline-right="single"/>
<context vline-inside="single"/>
<context hline-header="double"/>
<context hline-inside="single"/>
<context cell-valign="middle"/>
<context cell-2-1="This is very very very very very very very very very very very very very very very very very long text."/>
<context cell-0-2="l. This is very very very very very very very very very very very very very very very very very very very very very very very long text aligned to the left."/>

|                 Left                 |          Center           |  \<.  |                    Right                     |
| :----------------------------------- | :-----------------------: | :---: | -------------------------------------------: |
| A1                                   | w. Aligned to the center. |   -   | b. Aligned to the right<br />and the bottom. |
| r.t. A2 - Cell (1,0) with top right. |            \<.            |  ^.   |                                           ^. |
| A3                                   |             -             |  \<.  |                                           ^. |
