# Excercises
<br>

### 1. Use the deﬁnition of big-Ω to prove that nlogn = Ω(n + nlog(n<sup>2</sup>)). 
<b>Step 1</b>: Write the definition<br>
<p align="center">
f(n) = Ω(g(n))<br><br>
nlog(n) &#8805; C((n + nlog(n<sup>2</sup>))) ; where C &#62; 0 , n &#8805; n<sub>0</sub> , and n<sub>0</sub> &#8805; 0
</p>

<b>Step 2</b>: Simplify the equation<br>
<p align="center">
nlog(n) &#8805; C((n + 2nlog(n))) ; where C &#62; 0 , n &#8805; n<sub>0</sub> , and n<sub>0</sub> &#8805; 0<br><br>
</p>

<b>Step 3</b>: Choose a <i>C</i>, in this case I am choosing 1 because its easier to work with<br>
<p align="center">
nlog(n) &#8805; 1((n + 2nlog(n))) ; where C = 1 , n &#8805; n<sub>0</sub> , and n<sub>0</sub> &#8805; 0<br><br>
0 &#8804; n + nlog(n) ; where C = 1 , n &#8805; n<sub>0</sub> , and n<sub>0</sub> &#8805; 0<br>
Now we must find an initial n (n<sub>0</sub>) to make this statement true. In this cause 1/2 is a good number because log<sub>2</sub>(1/2) = -1<br><br>
</p>

<b>Step 4</b>: Choose a <i>n<sub>0</sub></i>, in this case I am choosing 1/2 because of eariler statement<br>
<p align="center">
0 &#8805; (1/2) + (1/2)log(1/2) ; where C = 1 , n &#8805; n<sub>0</sub> , and n<sub>0</sub> &#8805; 1/2<br><br>
0 &#8805; 1/2 - 1/2 ; where C = 1 , n &#8805; n<sub>0</sub> , and n<sub>0</sub> &#8805; 1/2<br><br>
0 &#8805; 0 ; where C = 1 , n &#8805; n<sub>0</sub> , and n<sub>0</sub> &#8805; 1/2<br>That statement is true because we have proven we f(n) = &#937;(g(n))<br><br>

<b>Visual</b>
<p align="center">
  <img src="https://user-images.githubusercontent.com/13907836/52300498-d6cc4a80-293c-11e9-99b5-1d48405c5e54.png">
  <img src="https://user-images.githubusercontent.com/13907836/52300523-e481d000-293c-11e9-8210-6a8cf4c2fbec.png">
  <img src="https://user-images.githubusercontent.com/13907836/52300538-f499af80-293c-11e9-9750-26fabd0ee1d9.png">
  <img src="https://user-images.githubusercontent.com/13907836/52300563-02e7cb80-293d-11e9-850a-4b39491c6ab9.png">
</p>

### 2. Provide the big-O relationship between  f(n) = nlogn and g(n) = (n + nlog(n<sup>2</sup>))
<b>Step 1</b>: Write the definition<br>
<p align="center">
f(n) = O(g(n))<br><br>
nlog(n) &#8804; C((n + nlog(n<sup>2</sup>))) ; where C &#62; 0 , n &#8805; n<sub>0</sub> , and n<sub>0</sub> &#8805; 0
</p>

<b>Step 2</b>: Simplify the equation<br>
<p align="center">
nlog(n) &#8804; C((n + 2nlog(n))) ; where C &#62; 0 , n &#8805; n<sub>0</sub> , and n<sub>0</sub> &#8805; 0<br><br>
</p>

<b>Step 3</b>: Choose a <i>C</i>, in this case I am choosing 1 because its easier to work with<br>
<p align="center">
nlog(n) &#8804; 1((n + 2nlog(n))) ; where C = 1 , n &#8805; n<sub>0</sub> , and n<sub>0</sub> &#8805; 0<br><br>
0 &#8804; n + nlog(n) ; where C = 1 , n &#8805; n<sub>0</sub> , and n<sub>0</sub> &#8805; 0<br><br>
Now we must find an initial n (n<sub>0</sub>) to make this statement true. In this cause 1 is a good number becuase 1+(anthing , where anything is positive) is greater then 0<br><br>
</p>

<b>Step 4</b>: Choose a <i>n<sub>0</sub></i>, in this case I am choosing 1 because of eariler statement<br>
<p align="center">
0 &#8804; (1) + (1)log(1) ; where C = 1 , n &#8805; n<sub>0</sub> , and n<sub>0</sub> &#8805; 1<br><br>
0 &#8804; 1 + 0 ; where C = 1 , n &#8805; n<sub>0</sub> , and n<sub>0</sub> &#8805; 1<br><br>
0 &#8804; 1 ; where C = 1 , n &#8805; n<sub>0</sub> , and n<sub>0</sub> &#8805; 1<br>That statement is true therefore f(n) &#8804; O(g(n))<br><br>
</p>
<b>Visual</b>
<p align="center">
  <img src="https://user-images.githubusercontent.com/13907836/52298656-50ae0500-2938-11e9-9b77-c1d3fb663b4e.png">
  <img src="https://user-images.githubusercontent.com/13907836/52298712-7e934980-2938-11e9-8a71-4692dbd38e3f.png">
  <img src="https://user-images.githubusercontent.com/13907836/52298790-a8e50700-2938-11e9-8d9d-14f214dda186.png">
  <img src="https://user-images.githubusercontent.com/13907836/52298941-1729c980-2939-11e9-9ffc-bd579185ec97.png">
</p>

<br>

### 3. Prove that f(n) = O(g(n)) if and only if g(n) = Ω(f(n)).<br>
<p align="center">
g(n) &#8805; c<sub>1</sub>(f(n))<br>
=> (1/c<sub>1</sub>)g(n) &#8805; f(n)<br>
<br>
Letting c<sub>2</sub> = (1/c) we can rewrite this inequality as <br>
f(n) &#8804; c<sub>2</sub>(g(n)) , where c<sub>2</sub> = 1/c<sub>1</sub>
</p>