PROJETO INTEGRADOR - Exercício 3
================
Prof. Neylson Crepalde
2018, Março, 5 a 16

Olá pessoal\! Vamos praticar um pouco as análises preliminares sobre um
banco de dados. Hoje, vamos trabalhar com o banco de dados do ENADE. O
banco de dados que vamos usar é uma amostra aleatória de apenas 10 mil
alunos. Usaremos essa amostra para facilitar um pouco o uso de memória
em nossas máquinas. A versão original dos dados, bem como o dicionário
de variáveis, pode ser obtido em <http://portal.inep.gov.br/microdados>.

Para ler o banco de dados direto da internet, use o comando:

``` r
library(readr)
enade14 <- read_csv2("https://raw.githubusercontent.com/neylsoncrepalde/introducao_ao_r/master/dados/enade_2014_amostra.csv")
```

Este exercício já deve ser entregue num documento do tipo RMarkdown.
Você deve apresentar o arquivo .Rmd e o html gerado\! Imagina um
cliente olhando para uma apresentação caprichada dessas\!\!\!\!\! S2

1.  Mostre com um comando e usando um gráfico a distribuição das idades
    dessa amostra de alunos que fizeram ENADE em 2014. Comente o
    resultado.

2.  Monte uma tabela exibindo as porcentagens e os valores absolutos das
    proporções de alunos por COR/RAÇA. O descobrimos sobre isso?

3.  Apresente a proporção de alunos casados e solteiros. Atenção,
    queremos apenas CASADOS e SOLTEIROS. Exclua de sua análise os alunos
    que tiverem outro tipo de estado civil.

4.  Apresente estatísticas descritivas sobre a nota geral dos alunos no
    Enade. Apresente também a informação em um gráfico. Qual é o gráfico
    mais adequado para a visualização desta variável? Por quê? Comente
    sobre a nota geral. Os alunos parecem ter, no geral, um bom
    desempenho ou um mal desempenho?

5.  Crie uma variável binária chamada `PUBLICA`. Nessa variável, você
    deve marcar 1 se a universidade em que o aluno estudou foi pública e
    0 se foi privada. **ATENÇÃO**: existe uma variável com a categoria
    administrativa da IES mas ela possui várias subclassificações. É
    preciso que você crie outra variável com as categorias corretas.

6.  Mostre a distribuição da renda para os alunos do ENADE 2014. Mostre
    também a distribuição de renda apenas para os alunos das escolas
    públicas e das escolas privadas.

7.  Mostre agora a nota geral dos alunos das faculdades públicas e dos
    alunos das faculdades privadas. O que você acha desses dados?

8.  **BÔNUS**: Existe um teste estatístico para verificar se a média da
    nota geral desta amostra dos alunos que fizeram ENADE pode ser
    inferida para toda a população? Faça o teste e apresente os
    resultados. Qual é o intervalo de confiança do teste?

9.  **BÔNUS**: Existe um teste estatístico para verificar se a diferença
    entre as notas dos alunos das universidades públicas e dos alunos
    das universidades privadas é estatisticamente significante? Faça o
    teste e apresente os resultados.

## Divirta-se\!
