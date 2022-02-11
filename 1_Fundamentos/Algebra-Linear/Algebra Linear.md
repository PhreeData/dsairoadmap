<center> <h1>Matrizes & Algebra Linear</h1></center>
<center>Valdeci S. B. S.</center>
<center>31/12/2021</center>
<center>19:40</center>

___

<center> <h2>Introdução</h2></center>
<br> 

> As vectors, matrices are data structures allowing you to organize numbers. They are square or rectangular arrays containing values organized in two dimensions: as rows and columns. You can think of them as a spreadsheet. Learn more here. 
> - Hadrien Jean, Machine Learning Scientist.

<br>

**Álgebra linear** é um ramo da [matemática](https://www.wikiwand.com/pt/Matem%C3%A1tica) que surgiu do estudo detalhado de sistemas de [equações lineares](https://www.wikiwand.com/pt/Equa%C3%A7%C3%A3o_linear), sejam elas [algébricas](https://www.wikiwand.com/pt/Equa%C3%A7%C3%A3o_alg%C3%A9brica "Equação algébrica") ou [diferenciais](https://www.wikiwand.com/pt/Equa%C3%A7%C3%A3o_diferencial "Equação diferencial"). A álgebra linear utiliza alguns conceitos e estruturas fundamentais da matemática como [vetores](https://www.wikiwand.com/pt/Vector_(espacial) "Vector (espacial)"), [espaços vetoriais](https://www.wikiwand.com/pt/Espa%C3%A7o_vetorial), [transformações lineares](https://www.wikiwand.com/pt/Transforma%C3%A7%C3%A3o_linear "Transformação linear"), [sistemas de equações lineares](https://www.wikiwand.com/pt/Sistema_de_equa%C3%A7%C3%B5es_lineares) e [matrizes](https://www.wikiwand.com/pt/Matriz_(matem%C3%A1tica)).

Vetores e matrizes desempenham um papel central na ciencia de dados, tendo provavelmente o meio mais comum de se representar dados a serem analizados e manipulados por quaisquer algoritimos de machine learning ou analytics. São dois os principais usos das matrizes em ciencia de dados:

1. Matrizes são o meio óbvio para se guardar dados tabulares de forma eficiente.

2. Matrizes são a fundação da algebra linear ou seja, são a linguagem da maioria dos modelos de machine learning e analytics.

 <br>
<center> <h2>Representação</h2></center>
<br> 



Vetores são arrays unidimensionais. Para representarmos usamos a notação

\begin{gathered}
\vec{a}^{m\! +\! 1} = \text{tansig} \left( \vec{W}^{m\! +\! 1}\! p + \vec{b}^{m\! +\! 1} \right) \quad \text{for}\; m = 0, 1, 2, ..., L-1\\
\vec{a} = \vec{a}^{L}\\
\vec{e} = t - a
\end{gathered}

 $\Large x\in \mathbb{R}^n$ para representar que $\Large x$ é um vetor com $\Large n$ entradas, tambem podemos representar de forma explicita da seguinte forma:

```math
\Large
x= \begin{bmatrix}

x_{1} \\
x_{2}\\
\vdots\\
x_{3}
\end{bmatrix}

```

Onde $\Large x_n$ representa o enésimo elemento do vetor. 

Matrizes são arrays 2D e usamos a notação $\Large A \in \mathbb{R}^{m\times n}$ para representar uma matriz de $\Large m$ linhas e $\Large n$ colunas, tambem podemos representar a matriz de forma explicita da seguinte forma:

$$\Large A = 
\begin{bmatrix}
    x_{11} & x_{12} & x_{13} & \dots  & x_{1n} \\
    x_{21} & x_{22} & x_{23} & \dots  & x_{2n} \\
    \vdots & \vdots & \vdots & \ddots & \vdots \\
    x_{m1} & x_{m2} & x_{m3} & \dots  & x_{mn}
\end{bmatrix}
$$


 <br>

Uma matriz tambem pode representar dados tabulares, usaremos aqui a representação de dados relacionais:


	
| Person ID | WH1 Grade | HW2 Grade |
|:---------:|:---------:|:---------:|
|     5     |    85     |    95     |
|     6     |    80     |    60     |
|    100    |    100    |    100    |



A representação da tabela acima se dá da seguinte forma:


$$\Large A \in \mathbb{R^{3\times 2}} = 
\begin{bmatrix}
    85 & 95\\
    80 & 60\\
    100 & 100
\end{bmatrix}
$$

<br>
<center> <h2>Bases da Algebra Linear</h2></center>
<br> 

> Linear algebra is foundational in data science and machine learning. Beginners starting out along their learning journey in data science--as well as established practitioners--must develop a strong familiarity with the essential concepts in linear algebra. 
> - Benjamin Obi Tayo, Ph.D., DataScienceHub


Considere as seguintes equações lineares com duas variáveis $\Large x_1$ e $\Large x_2$.

$$\Large 4x_1 -5x_2 = -13$$
$$\Large -2x_1 +3x_2 = 9$$

Eles podem ser escritas de forma compacta como na equação $\Large Ax=b$, onde:

<br>

$$\large A \in \mathbb{R^{2\times 2}} = 
\begin{bmatrix}
    4 & -5\\
    -2 & 3
\end{bmatrix}, 
b \in \mathbb{R^{2}} = 
\begin{bmatrix}
    -13 \\
    9 
\end{bmatrix}, 
x \in \mathbb{R^{2}} =
\begin{bmatrix}
    x_1 \\
    x_2
\end{bmatrix}.
$$

<br>

As operações/funções básicas e matrizes especiais são:

- **Adição e Subtração**
- **Transposição**
- **Multiplicação de matriz**
- **Matriz Identidade**
- **Matriz Inversa**
- **Resolução de equações lineares**
- **Transposição do produto de uma Matriz**
- **Produto interno**
- **Norma**

<br>
Complexidade das operações: 

- **Produto interno** $\Large x^ty: O(n)$
- **Produto Matriz-Vetor** $\Large Ax: O(n^2)$
- **Produto Matriz-Matriz** $\Large AB: O(n^3)$
- **Matriz inversa** $\Large A^{-1} ou\ A^{-1}y: O(n^3)$

[Aqui](https://x.com) pode-se consultar códigos em C, R e Python das principais funções.

