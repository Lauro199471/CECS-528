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
Now we must find an initial n (n<sub>0</sub>) to make this statement true. In this cause 1/2 is a good number becuase log<sub>2</sub>(1/2) = -1<br><br>
</p>

<b>Step 4</b>: Choose a <i>n<sub>0</sub></i>, in this case I am choosing 1/2 because of eariler statement<br>
<p align="center">
0 &#8805; (1/2) + (1/2)log(1/2) ; where C = 1 , n &#8805; n<sub>0</sub> , and n<sub>0</sub> &#8805; 1/2<br><br>
0 &#8805; 1/2 - 1/2 ; where C = 1 , n &#8805; n<sub>0</sub> , and n<sub>0</sub> &#8805; 1/2<br><br>
0 &#8804; 0 ; where C = 1 , n &#8805; n<sub>0</sub> , and n<sub>0</sub> &#8805; 1/2<br>That statement is true is therefore f(n) = &#937;(g(n))<br><br>

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
0 &#8804; 1 ; where C = 1 , n &#8805; n<sub>0</sub> , and n<sub>0</sub> &#8805; 1<br>That statement is true is therefore f(n) = O(g(n))<br><br>
</p>
<b>Visual</b>
<p align="center">
  <img src="https://user-images.githubusercontent.com/13907836/52298656-50ae0500-2938-11e9-9b77-c1d3fb663b4e.png">
  <img src="https://user-images.githubusercontent.com/13907836/52298712-7e934980-2938-11e9-8a71-4692dbd38e3f.png">
  <img src="https://user-images.githubusercontent.com/13907836/52298790-a8e50700-2938-11e9-8d9d-14f214dda186.png">
  <img src="https://user-images.githubusercontent.com/13907836/52298941-1729c980-2939-11e9-9ffc-bd579185ec97.png">
</p>

<br>
Let <i>G</i> be the graph we are observing. Since we have 2 odd degrees in the graph, the equation for <i>G</i> = <i>G<sup>i</sup></i>*<i>G<sup>ii</sup></i>.<br> Where <br>
<ul>
  <li><i>G<sup>i</sup></i>  = the even vertices of the graph( lets say n , where n > 0 (aka a postive amount of even vertices)</li>
  <li><i>G<sup>ii</sup></i> = the odd vertices of the graph ( in this case we have 2 odd vertices) </li>
</ul>
<br>
Now consider that the two odd vertices share an edge together like so, <br><br>
<p align="center">
  <img src="https://user-images.githubusercontent.com/13907836/52169282-70e88480-26ea-11e9-8ad5-fb39469ad8f8.png">
</p>
<br>If the Path(<i>P</i>) were to start at either of the odd vertices and the second node to move to is the other odd vertice then the shared edged will make the odd veritces even. Since the remaing of the graph is <b>Even</b> indicates that there is an <b>Euler Circuit</b> by applying <b>Theorem 1</b>. But! Our initial vertex was at vertex <b><i>a</i></b> and <i>G</i> got a circuit after the edge that was being shared by <b><i>a</i></b> and <b><i>b</i></b> is counted for already means we have a <i>P</i> only.
<br><br><br>

### 2. Prove that in any graph the number of vertices having odd degree is an even amount of vertices.<br>
<br>
The sum of the degrees is <b>twice</b> the number of edges.(The Handshake Theorem)<br><br>
<p align="center">
  <img src="https://user-images.githubusercontent.com/13907836/52169492-3254c900-26ee-11e9-8342-ee0fa32769d9.PNG">
</p>
Here is an example of the Handshake Theorem.<br>
<p align="center">
  <img src="https://user-images.githubusercontent.com/13907836/52169572-80b69780-26ef-11e9-91ba-93d0ff8aea26.png">
</p>
<br>

Let <i>e</i> be an edge on the graph( <i> e &#8712;</i> E(G)). Then <i>e</i> has 2 ends with 2 vertices(say <i>u</i> and <i>w</i>). When the sum of the degrees of <i>u</i> and <i>w</i>, edge <i>e</i> gets counted twice(one when we are counting the degrees of <i>u</i> and two for when we are counting the degrees of <i>w</i>). So since one edge takes on this property, means that <b>ALL</b> edges take on this property as well. So every edge gets counted <b>twice</b>. So this indicates that the Sum of degrees is even, which means there cannot be an odd number of odd degrees since adding an odd amount of odd numbers equals an odd but adding an even amount of odd degree is even. So therefore, there is an even amount of odd degree vertices.<br>
ex: Finding a graph with 2 vertices having 10 degrees and one vertex with one degree is IMPOSSIBLE<br>

### 3. Use the Pigeon-Hole Principle to prove that a simple graph with at least two vertices has at least two vertices having the same degree.
<br>
Since we are dealing with a simple graph(vertices do not repeat so no loops and no muliple edges to the same vertex) and its a connected finite graphwith <i>n</i> vertices. Then all vertices in <b>G</b> has a degree between 1 and <i>n</i>-1(the degree of a given vertex cannot be zero since <b>G</b> is connected). Since there are <i>n</i> vertices in <b>G</b> with degree between 1 and <i>n</i>-1, the pigeon-hole principle lets us concule that there is some integer <i>k</i> betweeen 1 and <i>n</i>-1 such that two or more verices have degree <i>k</i>.
<p align="center">
  <img src="https://user-images.githubusercontent.com/13907836/52174192-66a7a400-2745-11e9-8cd9-95358bbdf62f.png">
</p>
<br>

### 4. Prove that if G is a connected graph for which each of its vertices has even degree, then G must have a cycle.

A connected graph means that if given any two vertices(<i>i</i> and <i>j</i>), there is a path from <b>P<sub>i</sub></b> to <b>P<sub>j</sub></b>. Giving that the vertices are of even degree implies that there is a path from two vertices from using Theorem 1 where all even degree vertices have an Euler Circuit. Lets say vertices <i>i</i> and <i>j</i> were the first and last vertices respectively and the only way <i>j</i> can have a path with <i>i</i> is by having an edge to connect them thus creating a cycle. But lets say <i>i</i> and <i>j</i> were not the fist and last vertices, then the cycle can be within the path which means that Euler Circuit does not apply here since either of the vertices are revisting each other or another vertex in the math but also means they created a cylce which means any case if all vertices of even degree must have a cycle in a graph.

### 5. State a theorem analogous to Theorem 1 that holds true for strongly connected directed graphs

Let G = (V, E) be a directed graph, and deg<sup>−</sup>(v) means edges leaving the vertex and deg<sup>+</sup>(v) means edges entering the vertex. Then a strongly-connected simple graph ( no loops , no cycles , no repeats on edges, every vertex has a path to and from any vertex) has an Euler Circuit if all vertex in the graph has the same amount deg<sup>−</sup>(v) and deg<sup>+</sup>(v).

### 10. Prove that if G = (V, E) is connected, and a<sub>1</sub>, b<sub>1</sub>, . . . , a<sub>k</sub>, b<sub>k</sub> ∈ V are the odd-degree vertices of G, k ≥ 1, then the edges of G can be partitioned into k paths P<sub>1</sub>, . . . , P<sub>k</sub>, where P<sub>i</sub> is a path from one odd-degree vertex to another, and each odd-degree vertex serves as an endpoint to exactly one path.





