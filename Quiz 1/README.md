# CECS 528 Quiz 1, Spring 2019
<br>

### C. Suppose <i>f(n) = o(g(n))</i>. Circle each of the following that must also be true.<br> 
a. f(n) = ω(g(n))<br>
b. g(n) = ω(f(n))<br>
c. f(n) = O(g(n))<br>
d. g(n) = O(f(n))<br>
e. f(n) = Ω(g(n))<br>
f. g(n) = Ω(f(n))<br>
g. f(n) = Θ(g(n))<br>
h. g(n) = Θ(f(n))<br><br>
What we know:<br>
The definition of little o state: 
<p align="center">
lim<sub>n->∞</sub> = <i>f(n)</i> / <i>g(n)</i> = 0, so <i>g(n)</i> must be way bigger then f(n)<br>or<br>
lim<sub>n->∞</sub> = <i>g(n)</i> / <i>f(n)</i> = ∞, so <i>f(n)</i> must be way smaller then g(n)<br>
</p>
Knowing that means we can start circling which statements are true.<br>
<strike>a. f(n) = ω(g(n))</strike>, because lim<sub>n->∞</sub> = <i>f(n)</i> / <i>g(n)</i> is going towards 0 not ∞<br>
b. g(n) = ω(f(n)), because lim<sub>n->∞</sub> = <i>g(n)</i> / <i>f(n)</i> is going towards ∞  means this statement is true<br>
c. f(n) = O(g(n)), because <i>f(n)</i> &#8804; C(<i>g(n)</i>)<br>
d. <strike>g(n) = O(f(n))</strike>, because <i>f(n)</i> is big O of g(n)<br>
e. <strike>f(n) = Ω(g(n))</strike>, because <i>f(n)</i> &#8805; C(<i>g(n)</i>) , <i>f(n)</i> is not bigger<br>
f. g(n) = Ω(f(n)), because <i>g(n)</i> &#8805; C(<i>f(n)</i>) , <i>g(n)</i> is bigger<br>
g. <strike>f(n) = Θ(g(n))</strike>
h. <strike>g(n) = Θ(f(n))</strike>

### B. Use the definitions of big-O, big-Ω, big-Θ to prove that logn = Θ(ln(n)).<br>
ln(x) = log<sub>e</sub>x<br>
Change of base rule:
<p align="center">
  <img src="https://user-images.githubusercontent.com/13907836/52514823-19ef1d80-2bca-11e9-81b9-020ccddb8434.png">
</p><br>
<b>Big O</b><br>
log(n) &#8804; c(ln(n)) , where c > 0, n<sub>0</sub> &#8805; 0 and n &#8805; n<sub>0</sub><br>
log(n) &#8804; c(log(n)/log(e)) , where c > 0, n<sub>0</sub> &#8805; 0 and n &#8805; n<sub>0</sub><br><br>
lets make c = log(e)<br><br>
log(n) &#8804; log(e)(log(n)/log(e)) , where c > log(e), n<sub>0</sub> &#8805; 0 and n &#8805; n<sub>0</sub><br>
log(n) &#8804; log(n) , where c > log(e), n<sub>0</sub> &#8805; 0 and n &#8805; n<sub>0</sub><br><br>
lets make n<sub>0</sub> = 1<br><br>
log(2) &#8804; log(2) , where c > log(e), n<sub>0</sub> &#8805; 2 and n &#8805; n<sub>0</sub> &#8756; &#9989;<br>
