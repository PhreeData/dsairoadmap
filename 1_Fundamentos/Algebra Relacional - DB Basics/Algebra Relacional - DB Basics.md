<center> <h1>Algebra Relacional - DB Basics</h1></center>
<center>Valdeci S. B. S.</center>

<center>12/02/2022</center>
<br>


<center>

Notas: <br>
Para a correta visualização de funções em latex instale a extensão [Xdoc](https://github.com/nschloe/xhub) no chrome. <br>
[Aqui](https://colab.research.google.com/drive/18MjjX75mHj3N3hj0AtJDvMDx47sSfxUR?usp=sharing) voce encontra os respectivos códigos em Python.

</center>

<br>

___


<center> <h2>Algebra Relacional</h2></center>


Em [ciências da computação](https://www.wikiwand.com/pt/Ci%C3%AAncia_da_computa%C3%A7%C3%A3o), **álgebra relacional** é uma derivação descendente da [lógica de primeira ordem](https://www.wikiwand.com/pt/L%C3%B3gica_de_primeira_ordem "Lógica de primeira ordem") e da [álgebra de conjuntos](https://www.wikiwand.com/pt/%C3%81lgebra_de_grupo) em relação das [operações](https://www.wikiwand.com/pt/Opera%C3%A7%C3%A3o_(matem%C3%A1tica)) sobre a [relação finítimo](https://www.wikiwand.com/pt/Rela%C3%A7%C3%A3o_(matem%C3%A1tica)), que auxilia o trabalho ao identificar os componentes de uma [tupla](https://www.wikiwand.com/pt/Tupla) por nome (chamado o atributo) ao invés de uma coluna de chaves numéricas, o qual é chamado a [relação](https://www.wikiwand.com/pt/Rela%C3%A7%C3%A3o_(matem%C3%A1tica) "Relação (matemática)") na terminologia de banco de dados.

A principal aplicação da álgebra relacional é sustentar a fundamentação teórica de [banco de dados relacional](https://www.wikiwand.com/pt/Banco_de_dados_relacional), particularmente [linguagem de consulta](https://www.wikiwand.com/pt/Linguagem_de_consulta "Linguagem de consulta") para tais bancos de dados, entre os maiores o [SQL](https://www.wikiwand.com/pt/SQL).

Álgebra Relacional é definida como o conjunto de métodos que são aplicados para recuperar os dados com base nos requisitos definidos.

Esses conjuntos de métodos são chamados de Operadores de Álgebra Relacional.

Esses operadores são divididos em dois tipos:

- Operadores Nativos
- Operadores teóricos de conjuntos

<br>

Antes de conhecer em detalhes sobre esses operadores, precisamos entender as quatro definições a seguir.

Grau d(R): 

O número total de atributos/colunas presentes em uma relação/tabela é chamado de grau da relação e é denotado por d(R).

Cardinalidade |R|: 

Total não se tuplas presentes em uma relação ou Linhas presentes em uma tabela, chama-se cardinalidade de uma relação e é denotada por |R|.

**Domínio**: O intervalo total de valores aceitos para um atributo da relação é chamado de domínio do atributo.

**Compatibilidade da União**: Duas relações R e S são definidas para serem compatíveis entre si se e somente se:

Eles têm o mesmo grau d(R).
Os domínios dos respectivos atributos também devem ser os mesmos.


Agora voltando aos Operadores:

Conjunto teórico

União (∪)

Interseção (∩)

Subtração (-)

Produto cartesiano (X)

Nativo

Seleção (σ)

Projeção (π)

Renomear (ρ)

Dividir (÷)

Join

Nota: Para aplicar os operadores União, Interseção e Subtração entre quaisquer duas relações dadas, o pré-requisito é que essas relações sejam sempre compatíveis com União entre si.

suponha que existam duas relações R e S, então as seguintes propriedades são verdadeiras:

d(R∪S) = d(R) = d(S) e max(|R|,|S|) ≤ |R∪S| ≤ |R| + |S|

d(R∩S) = d(R) = d(S) e 0 ≤ |R∩S| ≤ min(|R|,|S|)

d(R-S) = d(R) = d(S) e 0 ≤ |R-S| ≤ (|R|) ou 0 ≤ |S-R| ≤ (|S|)

<br>

___


<center> <h2>DB Basics</h2></center>


**Bancos de dados** ([português brasileiro](https://www.wikiwand.com/pt/Portugu%C3%AAs_brasileiro)) ou **bases de dados** ([português europeu](https://www.wikiwand.com/pt/Portugu%C3%AAs_europeu)) são conjuntos de arquivos relacionados entre si com registros sobre pessoas, lugares ou coisas. São coleções organizadas de dados que se relacionam de forma a criar algum sentido (informação) e dar mais eficiência durante uma pesquisa ou estudo científico. São de vital importância para empresas e, há mais de duas décadas, se tornaram a principal peça dos sistemas de informação e segurança. Normalmente existem por vários anos sem alterações em sua estrutura sistemática.

Manipular grandes quantidades de dados pode ser uma tarefa desafiadora para os cientistas de dados. Na maioria das vezes, os dados que precisamos processar e analisar são muito maiores do que a capacidade de nossos dispositivos (o tamanho da RAM). Armazenar as informações no disco rígido pode fazer com que nosso código fique muito mais lento.
Sem mencionar que, para dar sentido aos dados e processá-los com eficiência, precisamos ter esses dados ordenados de alguma forma. Aqui onde os bancos de dados vêm para jogar.
Um banco de dados é definido como um conjunto estruturado de dados mantidos na memória de um computador ou na nuvem que pode ser acessado de várias maneiras.

Como cientista de dados, você precisará projetar, criar e interagir com bancos de dados na maioria dos projetos em que trabalhará. Às vezes, você precisará criar tudo do zero, enquanto em outras, você só precisará saber como se comunicar com um banco de dados já existente.

<br>
<center> <h3>Bancos de dados relacionais</h3></center>

Em um banco de dados relacional, os dados são organizados e armazenados em tabelas que podem ser vinculadas entre si por meio de alguma relação. Por exemplo, uma companhia aérea pode ter uma tabela de passageiros para todos os voos e outra para os passageiros de um voo específico. Um código de voo pode conectar essas duas tabelas.
Essa capacidade de ter tabelas conectadas nos permite — como desenvolvedores e cientistas de dados — entender melhor a relação entre os diferentes elementos da tabela. Compreender a relação pode nos dar dicas e insights que tornarão o processo de análise e visualização dos dados uma tarefa mais fácil.
A maneira de se comunicar e interagir com bancos de dados relacionais é através do uso da linguagem SQL.

<br>

<center> <h3>Bancos de dados não relacionais</h3></center>

Bancos de dados não relacionais, também conhecidos como bancos de dados NoSQL. Esses bancos de dados são aqueles que conectam as informações neles armazenadas por categorias e não por relações.
A forma mais popular do banco de dados NoSQL são os pares de valores-chave, nos quais você pode pensar da mesma forma que faz um dicionário Python. As chaves têm que ser únicas, desde que sejam, um par chave-valor pode armazenar todas as relações em um documento.
Os bancos de dados relacionais usam tabelas como sua unidade principal de armazenamento. Uma tabela em um banco de dados consiste em uma coleção de linhas e colunas, e você pode conectar várias tabelas usando relações. No NoSQL, no entanto, os dados são armazenados em um armazenamento semelhante a um documento. Você ainda pode realizar todas as tarefas diárias, como adicionar, excluir, atualizar seus dados, desde que saiba como o documento está estruturado.


<br>
<center> <h3>Comparação de banco de dados SQL vs. NoSQL</h3></center>

Os armazenamentos de dados NoSQL não relacionais ganharam popularidade por dois motivos:

- O RDBMS não foi dimensionado horizontalmente para Big Data

- Nem todos os dados se encaixam no esquema RDBMS estrito

Os datastores NoSQL oferecem escala horizontal em várias compensações do CAP Theorem. De acordo com o teorema CAP, um armazenamento de dados distribuído pode fornecer no máximo 2 das 3 garantias a seguir:

- Consistência: Cada leitura recebe a gravação mais recente ou um erro.

- Disponibilidade: Cada solicitação obtém uma resposta (sem erro), independentemente dos estados individuais dos nós.

- Tolerância de partição: O cluster não falha apesar de um número arbitrário de mensagens serem descartadas (ou atrasadas) pela rede entre os nós.


As diferenças entre os bancos de dados RDBMS e NoSQL decorrem de suas escolhas para:

Modelo de Dados: Os bancos de dados RDBMS são usados para dados estruturados (tabulares) normalizados que aderem estritamente a um esquema relacional. Os datastores NoSQL são usados para dados não relacionais, por exemplo. valor-chave, árvore de documentos, grafo.
Garantias de Transação: Todos os bancos de dados RDBMS suportam transações ACID, mas a maioria dos datastores NoSQL oferece transações BASE.

<br>
<center> <h3>Desempenho SQL vs. NoSQL</h3></center>


Os RDBMS são projetados para transações rápidas que atualizam várias linhas em tabelas com restrições de integridade complexas. As consultas SQL são expressivas e declarativas. Você pode se concentrar no que uma transação deve realizar. O RDBMS descobrirá como fazê-lo. Ele otimizará sua consulta usando álgebra relacional e encontrará o melhor plano de execução.
Os datastores NoSQL são projetados para manipular de forma eficiente muito mais dados do que RDBMS. Não há restrições relacionais nos dados e não precisa ser tabular. O NoSQL oferece desempenho em uma escala mais alta, geralmente desistindo de uma consistência forte. O acesso aos dados é feito principalmente por meio de APIs REST. As linguagens de consulta NoSQL (como GraphQL) ainda não são tão maduras quanto o SQL em design e otimizações. Portanto, você precisa cuidar do que e como fazê-lo com eficiência.
O RDBMS escala verticalmente. Você precisa atualizar o hardware (CPU mais potente, maior capacidade de armazenamento) para lidar com a carga crescente.
Os datastores NoSQL são dimensionados horizontalmente. O NoSQL é melhor no tratamento de dados particionados, portanto, você pode dimensionar adicionando mais máquinas.


---

> Fontes:
> [SQL vs. NoSQL Database: When to Use, How to Choose](https://towardsdatascience.com/datastore-choices-sql-vs-nosql-database-ebec24d56106)
> [RELATIONAL ALGEBRA – DEGREE, CARDINALITY, DOMAIN, UNION COMPATIBILITY AND OPERATORS](https://ashutoshtripathi.com/gate/dbms/relational-model/relational-algebra-degree-cardinality-domain-union-compatibility-and-operators/)
