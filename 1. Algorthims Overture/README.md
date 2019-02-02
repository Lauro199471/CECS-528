# Excercises
<br>

1. A Eulerian path from vertex <b><i>a</i></b> to vertex <b><i>b</b></i> is a path that begins at <b><i>a</b></i>, traverses each edge exactly once, and ends at <b><i>b</b></i>. Prove that if a connected graph has exactly <b>two odd-degree vertices</b>, <b><i>a</b></i> and <b><i>b</b></i>, then there is a Eulerian path from <b><i>a</b></i> to <b><i>b</b></i>.
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

2. Prove that in any graph the number of vertices having odd degree is an even amount of vertices.<br>
<br>
The sum of the degrees is <b>twice</b> the number of edges.(The Handshake Theorem)<br><br>
<p align="center">
  <img src="https://user-images.githubusercontent.com/13907836/52169492-3254c900-26ee-11e9-8342-ee0fa32769d9.PNG">
</p>
Here is an example of the Handshake Theorem.
<p align="center">
  <img src="https://user-images.githubusercontent.com/13907836/52169572-80b69780-26ef-11e9-91ba-93d0ff8aea26.png">
</p>
