In the book Common Lisp A Gentle Introduction to Symbolic Computation by David S. Touretzky published in 2013 there is an Appendix which has the SDRAW tool.

This tool allows to print CONS cell diagrams in the REPL.

Process to get CONS cell diagrams.

Step 1: Save the sdraw.generic file into the same directory as where the usual files for emacs is saved

Step 2: Type this S-expression  (load "sdraw.generic")

Step 3: To draw the CONS cell diagram for say (fruits (apples mangoes)) (vegetables (okra brinjal)) eggs) enter the following S-expression (sdraw '((fruits (apples mangoes)) (vegetables (okra brinjal)) eggs))

It will generate the following output


[*|*]--------------------------->[*|*]---------------------->[*|*]--->NIL
 |                                |                           |
 v                                v                           v
[*|*]--->[*|*]--->NIL            [*|*]------->[*|*]--->NIL   EGGS
 |        |                       |            |
 v        v                       v            v
FRUITS   [*|*]--->[*|*]--->NIL   VEGETABLES   [*|*]--->[*|*]--->NIL
          |        |                           |        |
          v        v                           v        v
         APPLES   MANGOES                     OKRA     BRINJAL


Thanks to Professor Touretzky for this tool for studying Common Lisp!
