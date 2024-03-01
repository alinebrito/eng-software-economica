# LAB: Medindo o tamanho de sistemas através do número de linhas de código


## Introdução

O trecho a seguir refere-se ao Capítulo 1 do livro "Análise de Pontos de Função", onde discute-se métricas para medição de software:

> _Esforço, prazo e custo são algumas das informações normalmente selecionadas como objeto de medição de estimativa. Estas métricas, e outras métricas secundárias que originam enquanto estimativa durante a condução do projeto, são coletadas e distribuídas na forma de relatórios com a situação do projeto, seu progresso atual e as expectativas quanto à sua situação futura._ -- Vazquez, et. al.

Uma etapa importante deste processo consiste em definir o que será medido, isto é, a quantificação de uma característica. Neste laboratório prático vamos estudar alguns conceitos relacionados com métricas e ferramentas para medição do tamanho de sistemas software.

## Linhas de Código (LOC)

Conforme descrito por Tetila (2019):

> _O tamanho do software é um indicador da quantidade de trabalho a ser executado no desenvolvimento de um projeto. Um projeto é estimado de acordo com o tamanho físico e de acordo com o grau de reuso de componentes. O tamanho físico é estimado por meio da medição da especificação de requisitos, análise, projeto e código, com base nas funções que o usuário obtém, na complexidade do problema que o software irá resolver._ 

O número de Linhas de Código (LOC - _Lines of Code_) não é necessariamente uma técnica de estimativa. É uma técnica de contagem empírica, que baseia-se na ideia de que certos sistemas possuem um número maior de linhas, sendo provavelmente projetos maiores e mais complexos de serem desenvolvidos. A ideia consiste em mensurar sistemas existentes, visando prever dimensões de projetos futuros. Por exemplo, erros por KLOC (milhares de linhas de código), custo por LOC, etc. A manutenção de históricos de dimensões é essencial realizar estimativas dos próximos projetos.

Porém, não existe um padrão para realizar a contagem. Observe alguns critérios para definir a contagem de linhas, mencionados por Vazquez, et. al:

* Contagem da quantidade de linhas de comentários, linhas em branco ou comandos nulos;
* Contagem de diretrizes de compilação;
* Contagem de múltiplos comandos ou declarações em uma única linha como várias linhas, uma para cada comando ou declaração;
* Contagem de uma única linha nos casos em que um único comando ou declaração é expresso em múltiplas linhas;
* Inclusão na contagem de delimitadores de blocos de comandos nos casos em que de fato haja mais de um comando;
* A desconsideração de delimitadores de blocos de comandos nos casos em que sua utilização seja opcional.

Alguns modelos (ex., COCOMO) utilizam LOC para estimativa de esforço, prazo, e custo. Porém, não é uma tarefa trivial realizar a estimativa da quantidade linhas de código, por exemplo, a quantilidade de linhas necessárias para atender uma lista de requisitos.

## Tarefa

A ferramenta [CK](https://github.com/mauricioaniche/ck) calcula várias métricas de código, incluindo LOC. Neste laboratório prático, você deve utilizar esta ferramenta para calcular o número de linhas de código de alguns projetos, discutindo os critérios utilizados.

1. Calcular LOC de um exemplo didático:

* Crie um projeto trivial, como por exemplo, um programa que exibe uma mensagem com o seu nome e a nome disciplina "Engenharia Econômica para Software". 

* Adicione comentários, altere a forma como o posicionamento das chaves é utilizado, adicione linhas em branco, etc. Em outras palavras, o seu projeto deve possuir diferentes trechos que fazem parte de sistemas do mundo real. Você pode utilizar como inspiração os tópicos discutidos neste roteiro. 

* Em seguida, utilize a ferramenta CK para calcular o número de linhas. Observe se a ferramenta contabilizou comentários e outros detalhes que você adicionou. Você concorda com a forma com o número de linhas foi computado?

2. Escolha um projeto real e relevante hospedado no GitHub. Em seguida, utilize a ferramenta CK para calcular o número de linhas dele.

**Observação: Se desejar, você pode utilizar outra ferramenta, que calcula o número de linhas de código de um sistema de software.**

**Entrega:** A entrega desta tarefa consiste na entrega de um relatório com:
- Link do seu projeto trivial no GitHub, número de linhas computadas, e os um breve comentário sobre o resultado (isto é, quais detalhes você adicionou no código e como a ferramenta lidou com eles).
- Link do projeto GitHub selecionado, número de estrelas, e número de linhas identificadas pela ferramenta CK.
- Entrega individual.

## Referências

* Análise de Pontos de Função. Carlos Vazquez, Guilherme Simões, Renato Albert. 13ed. Capítulo 1 - Por que Medir Software - Qual medida Melhor Representa o Tamanho?

* Estimativa de Software. Everon Tetila. Capítulo 3.3.3 - Linhas de Código (LOC)

* Java code metrics calculator (CK). Maurício Aniche. 2015. Disponível em: [https://github.com/mauricioaniche/ck](https://github.com/mauricioaniche/ck). Acesso em Março, 2023.






