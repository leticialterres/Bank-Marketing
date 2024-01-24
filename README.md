# Projeto de Classificação para Previsão de Subscrição a Depósito a Prazo em uma Instituição Bancária Portuguesa

O projeto em questão tem como objetivo principal desenvolver um modelo de classificação capaz de prever se um cliente de uma instituição bancária portuguesa irá ou não subscrever um depósito a prazo. Utiliza-se um conjunto de dados relacionados às campanhas de marketing direto realizadas pela instituição, baseadas em ligações telefônicas, para realizar essa previsão. A classificação é realizada utilizando a biblioteca XGBoost, conhecida por sua eficácia em problemas desse tipo.

Contextualização do Problema:
O conjunto de dados utilizado é proveniente de campanhas de marketing que ocorreram entre maio de 2008 e novembro de 2010. Durante essas campanhas, os clientes eram contatados via telefone, e muitas vezes era necessário realizar mais de um contato para determinar se o cliente iria ou não subscrever um depósito a prazo. O objetivo do projeto é, portanto, criar um modelo que, com base em informações disponíveis antes e durante a campanha, seja capaz de prever se um cliente irá ou não realizar essa subscrição.

Descrição do Conjunto de Dados:
O conjunto de dados é composto por diversas variáveis, dados relacionados à última campanha de marketing, e características específicas da ligação telefônica, como duração e mês do contato. A variável alvo é binária, indicando se o cliente subscreveu ou não ao depósito a prazo.

Pré-processamento dos Dados:
Antes de aplicar o modelo, são realizadas etapas de pré-processamento nos dados. Isso inclui a remoção de linhas com valores ausentes em variáveis-chave, como profissão, educação, tipo de contato e resultado da campanha anterior. Além disso, são realizadas transformações como a codificação de variáveis categóricas, utilizando técnicas como o LabelEncoder e OneHotEncoder.

Análise Exploratória dos Dados:
Uma análise inicial dos dados é conduzida para entender melhor o perfil dos clientes e identificar possíveis padrões. Isso inclui visualizações da distribuição de idade em relação à subscrição, contagem de profissões em relação às subscrições, distribuição do estado civil, nível educacional e a relação entre a duração da chamada e as subscrições.

Construção do Modelo:
Para a construção do modelo de classificação, é utilizado o XGBoost, uma biblioteca de boosting que tem se mostrado eficiente em diversos problemas de aprendizado de máquina. O modelo é treinado e ajustado utilizando técnicas como validação cruzada e ajuste de hiperparâmetros.

Avaliação do Modelo:
Após a construção do modelo, são avaliadas diversas métricas de desempenho, incluindo acurácia, precisão, revocação, F1 Score, AUC-ROC, e são geradas visualizações como a matriz de confusão, curva ROC e curva Precision-Recall. Essas métricas fornecem insights sobre quão bem o modelo está performando na tarefa de previsão.

Conclusões e Resultados:
Com base nas métricas e visualizações obtidas, o projeto conclui se o modelo é capaz de prever de forma satisfatória se um cliente irá subscrever ou não a um depósito a prazo. Esses resultados podem ser utilizados pela instituição bancária para otimizar futuras campanhas de marketing, direcionando esforços de maneira mais eficiente.

Considerações Finais:
O projeto não apenas fornece um modelo de previsão, mas também insights valiosos sobre os fatores que mais influenciam na subscrição de depósitos a prazo. Isso pode contribuir para uma abordagem mais estratégica por parte da instituição bancária, melhorando a eficácia de suas campanhas de marketing direto. O uso de técnicas de aprendizado de máquina, aliado à análise exploratória de dados, proporciona uma abordagem completa e informada para lidar com problemas complexos como este.
