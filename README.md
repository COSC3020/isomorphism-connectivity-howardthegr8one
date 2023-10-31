[![Open in Visual Studio Code](https://classroom.github.com/assets/open-in-vscode-718a45dd9cf7e7f842a935f5ebbe5719a5e09af4491e668f4dbf3b35d5cca122.svg)](https://classroom.github.com/online_ide?assignment_repo_id=12662416&assignment_repo_type=AssignmentRepo)
# Isomorphism

Prove that if two graphs $A$ and $B$ are isomorphic they do *not* have to
be completely connected. I have started with the formal definition of
isomorphism below. Add your answer to this markdown file. [This
page](https://docs.github.com/en/get-started/writing-on-github/working-with-advanced-formatting/writing-mathematical-expressions)
might help with the notation for mathematical expressions.

$G_1=(V_1 , E_1)$ is isomorphic to $G_2 = (V_2, E_2)$ if there exists a
one-to-one and onto function (bijection) $f: V_1 \rightarrow V_2$ such that $(u,v)
\in E_1$ iff $(f(u),f(v)) \in E_2$.


## My Proof: 

Let's rewrite our given statements as:  
p = If two graphs A and B are isomorphic  
then  
q = they do *not* have to be completely connected.  
So we have an implication statement, $p => q$, using a proof by contradiction we'll negate our statement
giving us $p \wedge \neg q$ or in English: if two graphs A and B are isomorphic they *must* be completely connected.
A completely connected graph being a graph where every vertex has a unique edge connecting it to every other vertex in the graph.

Let A be the graph represented by the following adjacency list:  
{  
  1: {2, 3},  
  2: {1, 4},  
  3: {1, 4},  
  4: {2, 3}  
}  
Let B be the graph represented by the following adjacency list:  
{  
  A: {B, D},  
  B: {A, C},  
  C: {B, D},  
  D: {A, C}  
}  
Since we can map all of the vertices and edges from A to B:  
1 => A  
2 => B or C  
3 => C or B  
4 => D  
Then A and B are isomorphic. However neither of these graphs are completely connected which contradicts our assumption that if
two graphs are isomorphic they must be completely connected, therefore by contradiction proving that if two graphs are isomorphic
they do *not* have to be completely connected. 

