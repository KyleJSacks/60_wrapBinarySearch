# implement List.indexOf

`while`-style and recursive implementations at the top of
OrderedList_inArraySlots.java

[Java API on the `indexOf` method](https://docs.oracle.com/javase/10/docs/api/java/util/List.html#indexOf(java.lang.Object))

based on [solutionsHolmes/5D_genericTypes/OrderedList_inArraySlots_v2/](https://github.com/stuyvesant-cs/solutionsHolmes/tree/master/5D_genericTypes/OrderedList_inArraySlots_v2)
as of 2019-04-10 04:48

y = log2(x) represents the number,y, which 2 must be raised to the power of in order to become x.
The graph looks like a curved line which flattens out as x grows larger, and approaches -infinity as x approaches 0

Recursive Solution:
0. To find the index of a given name within a phonebook, by jumping between halves of the phonebook
1. When asked to find a name in a section of a list low to hi, this recursive abstraction can find the name in the section
(low + hi)/2, hi or the section low, (low + hi)/2
2. a. if itemOnPage = targetItem
   b. Base Case: if true, return index of targetItem
   c. Recursive case(s)
		find item between middle and low, or middle and hi
		no leftover/concatenation