# costparser

A Clojure library designed to parse file that contains information about spending money.

## Usage

Create file that contains some costs with date. For example:

"--- 03.10.2013
-170 : cinema
-300 : fastfood
--- 06.10.2013
-2000 : party
--- 11.10.2013
-400 : book"

Then change "costsFile" constant and evaluate core.clj.
Now you can check how much you spend for fastfood, like that
"(amount (costsFor :fastfood))"

"amount" can take "after" date or "after" and "before" dates, like that
"(amount (costsFor :fastfood) "02.10.2013" "04.10.2013")"

There will be Incanter graphs in future.