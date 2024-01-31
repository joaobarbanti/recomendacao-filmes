## Recomendação Filme

#### Algoritmo que pega dados de usuário e notas que eles deram para determinados filmes e os usa para prever notas que eles dariam para novos filmes e assim os recomenda. 

## Processo técnico do Algoritmo

#### O modelo que realiza esse processo de análise e recomendação se chama svd++, ele atua em dois processos o primeiro seria o processo de análise e aprendizado: Nessa etapa o modelo irá olhar para as notas que os usuário já deram para determinados filmes, ele irá olhar para tais notas e tentará chegar nelas, ou seja ele irá definir números ou se preferir pesos totalmente aleatórios para os usuários e filmes e irá somar tais pesos tentando chegar na nota real que o usuário deu ao filme, a cada tentativa falha ele irá subtrair com a nota real e atualizar os pesos antes definidos, até chegar em um momento que a soma dos pesos de fato resulta na nota real dada pelo usuário ao filme no momento que isso ocorrer a etapa de análise encerra e a de recomendação se inicia: Com os pesos de cada usuário e filme definidos na fase de análise basta agora o sistema olhar para os filmes que determinado usuário não deu nota e somar o peso desse filme definido na fase anterior com o peso do usuário definido na mesma fase e somar os mesmos chegando assim na nota do filme e a partir dela o recomendando ou não. 

