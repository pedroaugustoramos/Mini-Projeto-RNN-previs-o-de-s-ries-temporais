Mini-Projeto-Previsões com Séries Temporais e RNNs
Introdução
Neste mini-projeto, você realizará uma previsão de séries temporais usando um regressor com Rede Neural Recorrente. Usaremos dados reais para prever os futuros preços das ações da Apple usando um modelo RNN.

Carregando os Dados
Primeiro, devemos carregar nossas séries temporais - uma série histórica de cerca de 140 dias do preço das ações da Apple (extraído do site DataMarket - https://datamarket.com/data/list/?q=provider%3Atsdl). Em seguida, precisamos executar uma série de etapas de pré-processamento para preparar os dados para uso com um modelo RNN.

É uma boa prática normalizar as séries temporais - normalizando seu range. Isso nos ajuda a evitar problemas numéricos sérios associados a funções de ativação comuns (como o tanh) que transformam números muito grandes (positivos ou negativos), além de ajudar a evitar problemas relacionados ao computar derivadas.

Aqui nós normalizamos a série para ficar na faixa [0,1], mas é também é comum normalizar por um desvio padrão da série.
