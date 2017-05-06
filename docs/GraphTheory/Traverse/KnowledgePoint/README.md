<script type="text/javascript" async src="//cdn.bootcss.com/mathjax/2.7.0/MathJax.js?config=TeX-AMS-MML_HTMLorMML"></script>
<script type="text/javascript" async src="https://cdnjs.cloudflare.com/ajax/libs/mathjax/2.7.1/MathJax.js?config=TeX-MML-AM_CHTML"></script>


--------
[Upper Folder - 上一级目录](../)


--------

<div>
<h1 align="center">Knowledge Point</h1>
<h1 align="center">知识要点</h1>
<br>
图： <br>
&emsp;&emsp;图\(G = \lt V,E \gt \)是由节点集合\(V\)和边集合\(E\)组成的数据结构，每条边\(e\)的两端是\(2\)个节点，每个节点\(v\)至少连接\(2\)条边。 <br>
<br>
无向边： <br>
&emsp;&emsp;若无向边\(e\)的两端点是\(u\)和\(v\)，则可以从\(u\)出发到达\(v\)，也可以从\(v\)出发到达\(u\)。 <br>
<br>
有向边： <br>
&emsp;&emsp;若有向边\(e\)从\(u\)指向\(v\)，则只能从\(u\)出发到达\(v\)，而不能反向。无向边也可以看作相同两个端点之间的两条反向有向边的叠加。 <br>
<br>
出度： <br>
&emsp;&emsp;节点\(u\)的出度是从节点\(u\)出发的边的数量，也称为出度度数，从节点\(u\)出发的边也称为出弧边。对于无向边和无向图来说，节点\(u\)的所有边都可以看作出弧边，即边数等于出度。 <br>
<br>
入度： <br>
&emsp;&emsp;节点\(u\)的入度是到达节点\(u\)的边的数量，也称为入度度数，到达节点\(u\)的边也称为入弧边。对于无向边和无向图来说，节点\(u\)的所有边也都可以看作入弧边，即边数等于入度。无向图中每个节点的出度和入度相等。 <br>
<p align="center"><img src="../res/KnowledgePoint1.png" /></p>
&emsp;&emsp;上面两个图中，图\(A\)为有向图，节点\(0 - 6\)的出度分别为\(2, 2, 1, 1, 2, 1\)，入度分别为\(1, 1, 2, 2, 0, 2\)。图\(B\)为无向图，节点\(0 - 6\)的出度分别为\(3, 4, 3, 3, 2, 3\)，入度与出度一样。 <br>
&emsp;&emsp;经常用\(n \times n\)的矩阵\(g\)来表示一个拥有\(n\)个节点的图，节点下标范围为\([1,n]\)。\(g[i,j]\)表示从节点\(i\)到\(j\)的距离（\(i,j \in [1,n]\)），也可以是其他信息，比如节点\(i\)是否可以直接到达节点\(j\)。无向图中相连的两个节点，可以看作有向图中两个节点之间有权值相等，方向相反的两条边。图\(A\)和\(B\)可以表示为：
\[
A =
\begin{bmatrix}
0 & 1 & 0 & 0 & 0 & 1 \\
0 & 0 & 1 & 1 & 0 & 0 \\
0 & 0 & 0 & 0 & 0 & 1 \\
0 & 0 & 1 & 0 & 0 & 0 \\
1 & 0 & 0 & 1 & 0 & 0 \\
0 & 1 & 0 & 0 & 0 & 0
\end{bmatrix}
\quad
B =
\begin{bmatrix}
0 & 1 & 0 & 0 & 1 & 1 \\
1 & 0 & 1 & 1 & 0 & 0 \\
0 & 1 & 0 & 1 & 0 & 1 \\
0 & 1 & 1 & 0 & 1 & 0 \\
1 & 0 & 0 & 1 & 0 & 0 \\
1 & 1 & 1 & 0 & 0 & 0
\end{bmatrix}
\]
</div>


--------
--------