In the book Common Lisp A Gentle Introduction to Symbolic Computation by David S. Touretzky published in 2013 there is an Appendix which has the SDRAW tool.

This tool allows to print CONS cell diagrams in the REPL.

Process to get CONS cell diagrams.

Step 1: Save the sdraw.generic file into the same directory as where the usual files for emacs is saved

Step 2: Type this S-expression  (load "sdraw.generic")

Step 3: To draw the CONS cell diagram for say (fruits (apples mangoes)) (vegetables (okra brinjal)) eggs) enter the following S-expression (sdraw '((fruits (apples mangoes)) (vegetables (okra brinjal)) eggs))

It will generate the following output



         <img width="571" alt="Screenshot 2024-11-11 at 5 59 05 PM" src="https://github.com/user-attachments/assets/d96df5cf-5b71-46e5-9118-4fe500ffcc0a">



Thanks to Professor Touretzky for this tool for studying Common Lisp!
