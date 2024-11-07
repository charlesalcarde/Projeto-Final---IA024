# Projeto-Final---IA024  
Sumarização de Múltiplos Documentos Científicos Utilizando o Dataset SurveySum

## Descrição do Projeto  
Com o aumento exponencial de publicações científicas, manter-se atualizado com as últimas tendências e avanços tornou-se um desafio para pesquisadores e profissionais. Este projeto tem como objetivo desenvolver um sistema que automatize a sumarização de múltiplos artigos científicos, gerando uma seção coesa de revisão de literatura (survey), facilitando a análise e o entendimento das contribuições mais relevantes dentro de um tema específico.

## 1. Objetivo do Projeto  
Desenvolver um sistema capaz de realizar a sumarização automática de múltiplos artigos científicos nas áreas de Inteligência Artificial (IA), Processamento de Linguagem Natural (PLN) e Aprendizado de Máquina (ML), utilizando o dataset SurveySum. A proposta é criar uma solução que gere uma seção de revisão de literatura baseada em um conjunto de artigos científicos relacionados a um tema específico, como "Mitigação de Viés em Modelos de Linguagem" ou "Modelos Transformers para PLN".

## 2. Escopo do Projeto  

O projeto será conduzido em etapas práticas e estruturadas, abrangendo desde a exploração dos dados até a avaliação dos resultados:

### Exploração do Dataset SurveySum
- Analisar e entender a estrutura do dataset SurveySum, selecionando um conjunto específico de seções para treinar e avaliar o modelo.
- Concentrar-se em temas delimitados para a sumarização, como "Transformers em PLN" ou "Redes Neurais Recorrentes em IA", com foco na relevância e coerência temática.

### Modelo de Sumarização com Pegasus-X
- Utilizar o modelo de linguagem pré-treinado Pegasus-X, que suporta contextos extensos (até 16k tokens), permitindo a sumarização de textos longos sem necessidade de truncamento excessivo.
- Implementar um pipeline de processamento que inclua:
  - **Extração de Chunks Relevantes**: Filtragem das partes mais informativas dos artigos científicos com base em similaridade semântica (SciBERT).
  - **Sumarização Abstrativa**: Geração do resumo final utilizando o Pegasus-X, integrando as referências (BIBREFs) dos artigos para formar um survey coeso.

### Avaliação da Qualidade
- Avaliar a qualidade das sumarizações geradas utilizando métricas automáticas como F1-Score com embeddings (SciBERT), G-Eval e Check-Eval semântico, garantindo uma análise mais abrangente da fidelidade semântica e da cobertura dos conceitos chave.
- Comparar o desempenho do sistema com as seções do survey original do dataset para verificar a precisão, consistência e relevância dos resumos.

### Relatório Final
- Documentar o pipeline implementado e os resultados obtidos, discutindo as limitações e propondo melhorias para trabalhos futuros.
- Analisar a eficácia do modelo em gerar resumos coerentes e relevantes, com base na consolidação de múltiplos documentos científicos, e apresentar possibilidades de expansão para tarefas mais complexas.

## 3. Ferramentas e Tecnologias  
- **Dataset**: SurveySum (disponível no Hugging Face Datasets).
- **Modelo de Sumarização**: Pegasus-X, ajustado para sumarização abstrativa de contexto longo.
- **Modelo de Similaridade**: SciBERT, para análise semântica e seleção de chunks.
- **Ambiente de Desenvolvimento**: Google Colab.
- **Avaliação**: Métricas como F1-Score com Embeddings, G-Eval, e Check-Eval para medir a qualidade e cobertura dos resumos gerados.

---

Esta abordagem oferece um sistema robusto para a sumarização de múltiplos artigos científicos, permitindo uma análise aprofundada e automatizada de literatura, com a flexibilidade de adaptação para diversos temas de pesquisa.
