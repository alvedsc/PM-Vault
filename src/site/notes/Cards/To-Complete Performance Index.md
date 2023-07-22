---
{"dg-publish":true,"permalink":"/cards/to-complete-performance-index/"}
---

up:: [[Cards/Earned Value Management\|Earned Value Management]] 
x:: 
d:: c

*It is the cost performance index (CPI) needed for the remaining part of the project to finish within the budget*. 

In this equation, the subscript "r" means **remaining for the rest of the project.**
$$CPI_r = \dfrac{EV_r}{AC_{r}}\space\space\space(1)$$
We defined the $TCPI$ as the $CPI$ for the remaining work, which means 
$$TCPI = CPI_c$$
$EV_r$ is the remaining value to be delivered, which is the difference between the total value of the project ($BAC$) and the value already delivered ($EV$)
$$EV_{r}= BAC-EV \space\space\space(2)$$
$AC_r$ are the remaining expenses, which are the difference between the projected final expense ($EAC$) and the current expenses ($AC$). 
$$AC_r=EAC-AC$$
However, what we want is to finish the project within budget, which means the projected expenses ($EAC$) should be equal to the initial budget ($BAC$), which means
$$EAC = BAC$$
So,
$$AC_{r}= BAC-AC \space\space\space(3)$$
Substituting equations (3) and (2) into (1), we end up with
$$TCPI = \dfrac{BAC - EV}{BAC-AC}$$
Which is *the ratio of the remaining work to be delivered ($BAC - EV$) and the actual remaining expenses to finish within budget ($BAC - AC$)*. 

For more information on the power of the [[Cards/To-Complete Performance Index\|To-Complete Performance Index]], check:
- [Scott, W. J. (2012). TCPI: the tower of power. Paper presented at PMI® Global Congress 2012—North America, Vancouver, British Columbia, Canada. Newtown Square, PA: Project Management Institute.](https://www.pmi.org/learning/library/to-complete-performance-index-tcpi-6009)
