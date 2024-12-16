![Logo do GitHub](https://github.com/Sarah-Freire/Trabalho-RNAG/raw/main/A2.png)

![LICENSE](https://img.shields.io/badge/LICENSE-GNU%20General%20Public%20License%20v3.0-red)

<h1 align="center"> Nutrella: O Algoritmo Genético que faz a sua dieta! </h1>

O Nutrella é um algoritmo genético baseado no problema da mochila com restrição. O nosso algoritmo utiliza uma base de dados brasileira de alimentos para montar uma dieta otimizada para o seu bem-estar. O algoritmo é de otimização visando maximizar a nutrição do consumidor, por entregar os alimentos mais nutritivos, sempre respeitando o limite calórico que ele deve consumir.

Não caia na rotina, use Nutrella.

Com Nutrella, toda vez que rodar o código você receberá uma nova dieta.

## Bem-vindo!

Este repositório de GitHub é dedicado para a disciplina de Redes Neurais e Algoritmos Genéticos do 3° semestre do Bacharelado em Ciência e Tecnologia da Ilum Escola de Ciência, faculdade parte do Centro Nacional de Pesquisa em Energia e Materiais (CNPEM), ministrada pelo Profº [Cassar. Daniel](https://github.com/drcassar). O projeto é um trabalho realizado para o atividade final da disciplina. Desse modo, abaixo temos uma explicação do trabalho e os responsaveis: 

 - [Barbara Perez](https://github.com/barbaraperez) - 220040
 - [Sarah Freire](https://github.com/Sarah-Freire) - 220043
 - [Vitor Barelli](https://github.com/Leprechas) - 220072

<details>
    
__<summary>O que é o Nutrella e o motivo da sua criação :orange:</summary>__
    
<p align="justify"> Nutrella é o nome dado a este código, o qual procura uma dieta razoável para o usuário. Desse modo, usando Algoritmos Genéticos para gerar a dieta e, para que seja possível, tem-se um dataframe contendo uma lista de vários alimentos comuns na alimentação brasileira. Pensando nisso, o diferencial em relação aos demais concorrentes é que aqui, toda vez que após interagir com o código uma dieta nova será retornada, de moto a evitar alimentações repetitivas, mantendo a qualidade nas escolhas, estas que são dadas pelos melhores indivíduos (alimentos) encontrados na busca usado pelo algoritmo.  

Além disso, sua criação se deu pelo objetivo de cientificamente poder proporcionar uma dieta com alimentos acessíveis para a população, dado o objetivo de cada usuário.
</p>
</details>

<details>

__<summary>Como foi feito 🥗</summary>__
    
<p align="justify">O código foi feito fazendo uma adaptação no algoritmo genético para o problema clássico da mochila. Portanto, o funcionamento do código é semelhante e baseia-se em encontrar a melhor resposta possível dadas as opções, que nesse caso é uma dieta que aproxima-se do numero de calorias "ideal" que foi retornado pelas perguntas anteriores.

Desse modo, como grande mudança temos a função obevtivo, já que além de buscar uma dieta com bons valores de calorias ela busca os melhores índices possíveis para o valor nutricional, dado as restrições. E para compreender melhor como é a estrutura de um algoritmo genético e o que cada termo usado durante as etapas do código temos o glossario abaixo:

- __*Indivíduos*:__ Em algoritmos genéticos, os indivíduos são soluções potenciais para um problema. Cada indivíduo é representado por um cromossomo, que contém genes que codificam características ou traços específicos.

- __*População*:__ Uma população é uma coleção de indivíduos que são avaliados e evoluídos ao longo do tempo. A população representa a geração atual de soluções potenciais.

- __*Gene*:__ Um gene é uma seção específica de um cromossomo que codifica um traço ou característica particular. Por exemplo, em um algoritmo genético para otimizar o design de uma asa de avião, um gene pode representar o ângulo no qual a asa está inclinada.

- __*Cromossomos*:__ Um cromossomo é uma sequência de genes que representa uma solução individual para o problema em questão. Em algoritmos genéticos codificados em binário, os cromossomos são geralmente representados como sequências de 0s e 1s.

- __*Geração*:__ Uma geração refere-se a uma iteração do algoritmo genético. Durante cada geração, a função de aptidão é aplicada para avaliar os indivíduos da população, e novos indivíduos são criados por meio de seleção, cruzamento e mutação.

- __*Função de objetivo*:__ A função de aptidão é usada para avaliar o quão bem cada indivíduo da população resolve o problema em questão. Ela atribui uma pontuação de aptidão a cada indivíduo com base em quão próximo sua solução está de ser ótima.

- __*Seleção*:__ A seleção é o processo pelo qual os indivíduos com pontuações de aptidão mais altas têm maior probabilidade de serem escolhidos para reprodução (ou seja, passar seus genes adiante) do que aqueles com pontuações de aptidão mais baixas.

- __*Cruzamento*:__ O cruzamento envolve a combinação de dois cromossomos parentais para criar um ou mais cromossomos filhos. Esse processo pode ajudar a criar novas combinações de genes que podem levar a melhores soluções.

- __*Mutação*:__ A mutação envolve a alteração aleatória de um ou mais genes no cromossomo de um indivíduo. Esse processo pode ajudar a introduzir novos traços na população que podem levar a melhores soluções.

</p>
</details>

## Principais arquivos

<p align="justify"> Guia para navegar no Git da Nutrella; </p>

Desse modo, as seguintes pastas compõem esse repositório:
- [Alimentos - Calorias.xlsx](https://github.com/Sarah-Freire/Trabalho-RNAG/blob/main/Alimentos%20-%20Calorias.xlsx): É uma tabela excel que possibilita encontrar os alimentos e seus dados de calorias e densidade nutricional
- [Alimentos.xlsx](https://github.com/Sarah-Freire/Trabalho-RNAG/blob/main/Alimentos.xlsx): É uma tabela excel, onde podemos encontrar os alimentos e seus dados de calorias, proteínas, lipídios, carboidratos e fibra alimentar
- [Tratando dados.ipynb](https://github.com/Sarah-Freire/Trabalho-RNAG/blob/main/Tratando%20dados.ipynb): Notebook o qual utiliza o arquivo excel "Alimentos.xlsx" e altera os seus dados para produzir os dados de densidade nutricional e gerar o arquivo excel "Alimentos - Calorias.xlsx".
- [LICENSE](https://github.com/Sarah-Freire/Trabalho-RNAG/blob/main/LICENSE): Apresenta a licença usada no repositório
- [README.md](https://github.com/YgorRuas/Redes_Neuro_Anais/blob/main/README.md): Guia para o repositório
- [funcoes.py](https://github.com/Sarah-Freire/Trabalho-RNAG/blob/main/funcoes.py): Arquivo python a qual armazenam todas as funções utilizadas no decorrer do trabalho.
- [trabalho_rnag.ipynb](https://github.com/Sarah-Freire/Trabalho-RNAG/blob/main/trabalho_rnag.ipynb): É o notebook onde o trabalho foi desenvolvido.


![Logo do GitHub](https://github.com/Sarah-Freire/Trabalho-RNAG/raw/main/A1.png)

![GitHub Logo](https://github.com/Sarah-Freire/Trabalho-RNAG/raw/main/A2.png)

![LICENSE](https://img.shields.io/badge/LICENSE-GNU%20General%20Public%20License%20v3.0-red)

<h1 align="center"> Nutrella: The Genetic Algorithm That Designs Your Diet! </h1>

Nutrella is a genetic algorithm based on the constrained knapsack problem. Our algorithm utilizes a Brazilian food database to build an optimized diet for your well-being. This optimization algorithm aims to maximize the consumer's nutrition by selecting the most nutritious foods, while always respecting the caloric limit the individual should consume.

Don’t fall into a routine—use Nutrella.

With Nutrella, every time you run the code, you receive a new diet.

## Welcome!

This GitHub repository is dedicated to the Neural Networks and Genetic Algorithms course from the 3rd semester of the Bachelor’s in Science and Technology at Ilum School of Science, a college within the National Center for Research in Energy and Materials (CNPEM), taught by Prof. [Cassar. Daniel](https://github.com/drcassar). The project is the final assignment of the course. Below is an explanation of the project and the contributors:

- [Barbara Perez](https://github.com/barbaraperez) - 220040  
- [Sarah Freire](https://github.com/Sarah-Freire) - 220043  
- [Vitor Barelli](https://github.com/Leprechas) - 220072

<details>
<summary>What is Nutrella and the reason for its creation :orange:</summary>
    
<p align="justify">
Nutrella is the name given to this code, which seeks a reasonable diet for the user. Thus, by using Genetic Algorithms to generate the diet, and by having a dataframe containing a list of various foods common in Brazilian cuisine, the difference from other competitors is that here, every time you interact with the code, a new diet will be generated. This avoids repetitive meals while maintaining quality choices, provided by the best individuals (foods) found through the algorithm's search.

In addition, it was created with the scientific goal of providing a diet with accessible foods for the population, tailored to each user’s objectives.
</p>
</details>

<details>
<summary>How it was done 🥗</summary>
    
<p align="justify">
The code is an adaptation of the genetic algorithm for the classic knapsack problem. Therefore, the code’s operation is similar and is based on finding the best possible solution given the options. In this case, it seeks a diet close to the "ideal" caloric number returned by previous queries.

Hence, the main change lies in the objective function. In addition to searching for a diet with good caloric values, it also seeks the best possible nutritional indexes, given the constraints. To better understand the structure of a genetic algorithm and each term used during the code steps, we have the glossary below:

- __*Individuals*__: In genetic algorithms, individuals are potential solutions to a problem. Each individual is represented by a chromosome containing genes that encode specific characteristics or traits.

- __*Population*__: A population is a collection of individuals that are evaluated and evolved over time. The population represents the current generation of potential solutions.

- __*Gene*__: A gene is a specific section of a chromosome that encodes a particular trait or characteristic. For example, in a genetic algorithm optimizing an airplane wing design, a gene might represent the angle of the wing’s inclination.

- __*Chromosomes*__: A chromosome is a sequence of genes representing an individual solution to the problem at hand. In binary-encoded genetic algorithms, chromosomes are usually represented as sequences of 0s and 1s.

- __*Generation*__: A generation refers to an iteration of the genetic algorithm. In each generation, the fitness function evaluates the population's individuals, and new individuals are created through selection, crossover, and mutation.

- __*Objective Function*__: The fitness function is used to evaluate how well each individual in the population solves the problem in question. It assigns a fitness score to each individual based on how close its solution is to optimal.

- __*Selection*__: Selection is the process by which individuals with higher fitness scores are more likely to be chosen for reproduction (i.e., to pass their genes on) than those with lower fitness scores.

- __*Crossover*__: Crossover involves combining two parent chromosomes to create one or more offspring chromosomes. This process can create new gene combinations that lead to better solutions.

- __*Mutation*__: Mutation involves randomly altering one or more genes in an individual’s chromosome. This process can introduce new traits into the population, potentially leading to better solutions.
</p>
</details>

## Main Files

<p align="justify">Guide to navigating the Nutrella Git repository:</p>

The following folders make up this repository:

- [Alimentos - Calorias.xlsx](https://github.com/Sarah-Freire/Trabalho-RNAG/blob/main/Alimentos%20-%20Calorias.xlsx): An Excel table that allows you to find foods along with their calorie data and nutritional density.
- [Alimentos.xlsx](https://github.com/Sarah-Freire/Trabalho-RNAG/blob/main/Alimentos.xlsx): An Excel table containing foods and their data on calories, protein, lipids, carbohydrates, and dietary fiber.
- [Tratando dados.ipynb](https://github.com/Sarah-Freire/Trabalho-RNAG/blob/main/Tratando%20dados.ipynb): A notebook that uses the "Alimentos.xlsx" file and modifies its data to produce nutritional density data, generating the "Alimentos - Calorias.xlsx" file.
- [LICENSE](https://github.com/Sarah-Freire/Trabalho-RNAG/blob/main/LICENSE): Presents the license used in the repository.
- [README.md](https://github.com/YgorRuas/Redes_Neuro_Anais/blob/main/README.md): Repository guide.
- [funcoes.py](https://github.com/Sarah-Freire/Trabalho-RNAG/blob/main/funcoes.py): A Python file containing all the functions used throughout the project.
- [trabalho_rnag.ipynb](https://github.com/Sarah-Freire/Trabalho-RNAG/blob/main/trabalho_rnag.ipynb): A notebook where the project was developed.

![GitHub Logo](https://github.com/Sarah-Freire/Trabalho-RNAG/raw/main/A1.png)
