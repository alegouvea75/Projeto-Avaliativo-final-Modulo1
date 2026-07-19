# Projeto-Avaliativo-final-Modulo1
Previsão para app e-commerce Churn- setor varejo

## Descrição do Problema de Negócio
Um aplicativo de vendas (e-commerce) enfrenta o desafio constante de reter seus usuários. O objetivo deste projeto é construir um modelo preditivo de Machine Learning capaz de identificar antecipadamente quais clientes estão prestes a abandonar a plataforma. 
Com essa inteligência, a empresa deixa de ser reativa e passa a atuar de forma preventiva, oferecendo cupons de retenção estrategicamente para os clientes em risco, protegendo a receita e a base de usuários do aplicativo.

## Resumo Executivo: Insights da (Análise Exploratória).
Durante a fase de Análise Exploratória de Dados, alguns padrões importantes sobre o comportamento dos clientes foram identificados para guiar a modelagem: A base de dados apresentou um forte desbalanceamento na variável alvo, com a maioria dos clientes permanecendo ativos, o que exigiu técnicas de balanceamento durante o treino.

## Veredito do Melhor Modelo de Negócios

Após rigorosos testes comparando algoritmos e controlando o *overfitting*, o modelo selecionado para entrar em produção foi o (KNN).
O modelo KNN destacou-se ao alcançar um Recall de 0,85 para a classe 1 (Churn). Nenhuma Inteligência Artificial é 100% assertiva, mas as decisões de negócio devem focar na maximização do lucro e mitigação de danos. 

## A Justificativa Financeira

Neste cenário de e-commerce, avaliamos os impactos dos erros do modelo:
Falso Positivo: O modelo prevê abandono, a empresa envia um cupom (10% a 15% de desconto), mas o cliente não iria sair. O custo é apenas a margem do desconto.
Falso Negativo: O modelo não prevê o abandono, a empresa não faz nada, e o cliente pode sair. O custo é a perda total da lucratividade futura do cliente e o aumento drástico no gasto com marketing para tentar recuperar esse usuário depois.

Portanto, financeiramente e estrategicamente, é muito mais vantajoso acreditar na previsão de risco do modelo e assumir o custo baixo de um cupom preventivo do que arcar com a perda definitiva do cliente. O KNN provou ser a ferramenta mais segura para esta estratégia de retenção focada no potencial Churn.
