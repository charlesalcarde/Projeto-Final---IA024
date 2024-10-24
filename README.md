# Projeto-Final---IA024
Sumarização de Múltiplos Documentos Científicos utilizando o Dataset SurveySum
## Descrição do Projeto
Com o crescente volume de publicações científicas, acompanhar as últimas tendências e avanços tornou-se um desafio significativo para pesquisadores e profissionais. Nosso objetivo é desenvolver um sistema que automatize a sumarização de múltiplos artigos científicos, gerando uma seção coesa de revisão de literatura (survey), facilitando a análise e o entendimento das contribuições mais relevantes dentro de um tema específico.
## 1. Objetivo do Projeto
O objetivo do projeto será desenvolver um sistema que realiza sumarização de múltiplos documentos científicos nas áreas de Inteligência Artificial (IA), Processamento de Linguagem Natural (PLN) e Aprendizado de Máquina (ML), utilizando o dataset SurveySum. O foco será em criar uma solução que possa gerar uma seção de revisão de literatura com base em um conjunto de artigos científicos relacionados a um tema específico.

## 2. Escopo do Projeto
Este projeto está dividido em etapas práticas e definidas:

### Exploração do Dataset SurveySum:

* Compreender a estrutura do SurveySum e selecionar uma pequena parte do dataset (por exemplo, algumas seções de surveys) para treinar e testar o modelo.
* Focar em sumarizar um conjunto pequeno de artigos para um tema específico, como "Transformers em PLN" ou "Redes Neurais Recorrentes em IA".

### Modelo de Sumarização:

* Utilizar um modelo de linguagem pré-treinado como BART para a tarefa de sumarização abstrativa. Esses modelos são eficazes para resumir textos longos e podem ser ajustados para essa tarefa.
* Implementar um pipeline simples de retrieval + summarization:
** Recuperação: Coletar e segmentar os artigos científicos relacionados ao tema 
** Sumarização: Alimentar esses textos segmentados no modelo de linguagem para gerar o resumo (seção do survey).

###  Avaliação da Qualidade:

* Avaliar a qualidade das sumarizações geradas com base em métricas automáticas simples, como ROUGE (para medir a sobreposição entre os textos de referência e os textos gerados) ou uma avaliação manual, comparando com as seções do survey original.
* Para simplificar, será testado o modelo em apenas algumas seções do survey para verificar se o modelo consegue gerar resumos coesos e relevantes.

### Relatório Final:

* Documentar o pipeline implementado e os resultados obtidos, discutindo as limitações e sugerindo melhorias. O foco será na eficácia do modelo em gerar resumos adequados e coesos com base em múltiplos documentos científicos.
* O relatório deverá incluir uma análise dos resultados e uma proposta de como o projeto poderia ser expandido para tarefas mais complexas no futuro.

## 3. Ferramentas e Tecnologias
* Dataset: SurveySum (disponível no Hugging Face Datasets).
* Modelo de Sumarização: BART.
* Ambiente de Desenvolvimento: Google Colab (para experimentos com modelos de linguagem e acesso ao dataset).
* Avaliação: Métricas como ROUGE para medir a qualidade dos resumos gerados.
