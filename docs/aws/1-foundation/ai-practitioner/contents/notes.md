<!-- BEGIN_DOCS -->

[◀ Voltar](../README.md)

<div align="center">

<a name="readme-top"></a>

<img src="https://github.com/lpsm-dev/lpsm-dev/blob/24c8c8777f1170ae63113f3b1f9338416df0ffc3/.github/assets/guide.png" width="350"/>

## Anotações

</div>

# Sumário

<details>
  <summary><strong>Expandir</strong></summary>

<!-- START doctoc generated TOC please keep comment here to allow auto update -->
<!-- DON'T EDIT THIS SECTION, INSTEAD RE-RUN doctoc TO UPDATE -->

- [1. Fundamentos de IA e Aprendizado de Máquina](#1-fundamentos-de-ia-e-aprendizado-de-m%C3%A1quina)
  - [1.1. Definições Avançadas](#11-defini%C3%A7%C3%B5es-avan%C3%A7adas)
  - [1.2. Tipos de Aprendizado](#12-tipos-de-aprendizado)
  - [1.3. Técnicas de Treinamento e Otimização](#13-t%C3%A9cnicas-de-treinamento-e-otimiza%C3%A7%C3%A3o)
- [2. Conceitos e Técnicas Complementares em IA](#2-conceitos-e-t%C3%A9cnicas-complementares-em-ia)
- [3. Técnicas de Otimização em Machine Learning](#3-t%C3%A9cnicas-de-otimiza%C3%A7%C3%A3o-em-machine-learning)
  - [Prunning](#prunning)
  - [Quantization](#quantization)
  - [Knowledge Distillation](#knowledge-distillation)
  - [Fine-Tuning: Full vs. PEFT](#fine-tuning-full-vs-peft)
- [4. Métricas para Avaliar Desempenho e Ajuste de Hiperparâmetros](#4-m%C3%A9tricas-para-avaliar-desempenho-e-ajuste-de-hiperpar%C3%A2metros)
  - [Métricas de Desempenho](#m%C3%A9tricas-de-desempenho)
  - [Ajuste de Hiperparâmetros](#ajuste-de-hiperpar%C3%A2metros)
  - [Parâmetros de Geração de Texto](#par%C3%A2metros-de-gera%C3%A7%C3%A3o-de-texto)
  - [Knowledge Cut-Off](#knowledge-cut-off)
- [5. Inferência, Viés e Imparcialidade](#5-infer%C3%AAncia-vi%C3%A9s-e-imparcialidade)
  - [Conceitos de Inferência](#conceitos-de-infer%C3%AAncia)
  - [Tipos de Inferência](#tipos-de-infer%C3%AAncia)
  - [Outros Conceitos Relacionados](#outros-conceitos-relacionados)
- [6. AWS Services](#6-aws-services)
  - [Amazon Connect](#amazon-connect)
  - [Amazon Bedrock](#amazon-bedrock)
  - [Amazon SageMaker](#amazon-sagemaker)
  - [Amazon Comprehend](#amazon-comprehend)
  - [Amazon Titan](#amazon-titan)
  - [AWS Inferentia](#aws-inferentia)
  - [AWS Trainium](#aws-trainium)
- [7. Princípios de Responsible AI na AWS](#7-princ%C3%ADpios-de-responsible-ai-na-aws)
- [9. Termos](#9-termos)

<!-- END doctoc generated TOC please keep comment here to allow auto update -->

<p align="right">(<a href="#readme-top">back to top</a>)</p>

</details>

# 1. Fundamentos de IA e Aprendizado de Máquina

## 1.1. Definições Avançadas

**O que é Foundation Model?**
Foundation Models (FMs) são modelos de linguagem de grande escala pré-treinados em vastos conjuntos de dados para capturar conhecimento geral. São usados como base para tarefas específicas de NLP, como tradução, resumo, geração de texto e classificação.

**O que é LLM (Large Language Model)?**
LLMs são modelos treinados em grandes conjuntos de dados para capturar o conhecimento da linguagem, aplicáveis a tradução, resumo, geração e classificação de texto.

**O que é Difussion Models?**
Difussion Models geram previsões combinando amostras de texto e ruído, resultando em previsões diversificadas e criativas, evitando repetições e conservadorismo.

**O que é RAG (Retrieval-Augmented Generation)?**
RAG combina geração de texto com recuperação de informações, utilizando bases de conhecimento externas, como documentos e bancos de dados.

**O que é Fine-Tuning?**
Fine-Tuning é o ajuste de modelos pré-treinados para tarefas específicas, treinando o modelo em um novo conjunto de dados para melhorar seu desempenho.

## 1.2. Tipos de Aprendizado

**Aprendizado Supervisionado**

- **Objetivo:** Treinar modelos utilizando dados rotulados para prever saídas corretas para novos exemplos.
- **Exemplos:**
  - Classificação de E-mails (spam ou não spam)
  - Previsão de Preços de Casas
- **Algoritmos Comuns:**
  - Regressão Linear
  - Árvores de Decisão
  - Support Vector Machines (SVM)
  - Redes Neurais

**Aprendizado Não Supervisionado**

- **Objetivo:** Encontrar padrões ou estruturas inerentes nos dados sem a necessidade de rótulos.
- **Exemplos:**
  - Segmentação de Clientes
  - Detecção de Anomalias
- **Algoritmos Comuns:**
  - K-Means Clustering
  - PCA
  - Autoencoders

**Aprendizado Semi-Supervisionado**

- **Objetivo:** Combinar dados rotulados e não rotulados para melhorar o desempenho do modelo.
- **Exemplos:**
  - Classificação de Textos com dados limitados
  - Reconhecimento Facial aprimorado

**Aprendizado por Reforço**

- **Objetivo:** Treinar um agente para interagir com um ambiente dinâmico e maximizar uma recompensa através da tentativa e erro.
- **Exemplos:**
  - Jogos, robótica e otimização de processos

## 1.3. Técnicas de Treinamento e Otimização

- **Early Stopping:** Técnica que interrompe o treinamento quando a perda de validação começa a aumentar, prevenindo overfitting.
- **Training & Validation Loss/Accuracy:** Monitoramento das métricas para identificar o ponto ótimo de treinamento, evitando underfitting e overfitting.

# 2. Conceitos e Técnicas Complementares em IA

- **Redes Neurais (Neural Networks):** Modelos inspirados no funcionamento do cérebro, compostos por neurônios artificiais organizados em camadas para aprender padrões a partir de dados.
- **Regressão Linear:** Modelo supervisionado que ajusta uma linha reta para prever valores numéricos minimizando discrepâncias.
- **K-Means Clustering:** Algoritmo não supervisionado que agrupa dados em K clusters, minimizando a distância intra-grupo e maximizando a separação entre clusters.
- **Árvore de Decisão (Decision Tree):** Modelo que utiliza uma estrutura de ramificações para tomar decisões de classificação ou regressão por meio de perguntas sucessivas.
- **Random Forest:** Conjunto (ensemble) de árvores de decisão que melhora a precisão e reduz o risco de overfitting.
- **Support Vector Machine (SVM):** Modelo que encontra o hiperplano que melhor separa os dados em classes.
- **PCA (Principal Component Analysis):** Técnica para redução de dimensionalidade que identifica os componentes principais responsáveis pela variância dos dados.
- **N-Gram:** Sequências contíguas de N tokens (palavras, caracteres) usadas em NLP para capturar estrutura e semântica.
- **AutoML:** Automatiza a construção, treinamento e ajuste de modelos de Machine Learning, reduzindo a necessidade de conhecimento altamente especializado.
- **Epochs:** Número de vezes que o modelo percorre o conjunto de dados durante o treinamento.
- **Accuracy (Acurácia):** Métrica que indica a proporção de previsões corretas em relação ao total de amostras.
- **Hallucination:** Fenômeno em que modelos de linguagem geram previsões incorretas ou fictícias sem base nos dados reais.
- **Prompt Engineering:** Técnica para a criação de prompts precisos que direcionam os modelos de linguagem a fornecerem respostas desejadas.
- **Modelo Multimodal:** Modelos que processam e combinam informações provenientes de diferentes modalidades (ex.: texto, imagem, áudio).
- **Clusterização:** Técnica de agrupamento em que dados semelhantes são organizados em clusters ou grupos.
- **IDP (Intelligent Document Processing):** Tecnologia que automatiza a captura, classificação e extração de dados de documentos utilizando OCR, NLP, ML e técnicas de IA.

# 3. Técnicas de Otimização em Machine Learning

## Prunning

- **Objetivo:** Remover componentes desnecessários de um modelo (como neurônios ou camadas) para otimizar recursos.
- **Vantagens:** Reduz o tamanho do modelo e melhora a eficiência computacional.
- **Exemplo de Uso:** Redes neurais profundas em dispositivos com recursos limitados.

## Quantization

- **Objetivo:** Reduzir a precisão numérica dos modelos (ex.: converter FP32 para INT8).
- **Vantagens:** Acelera a inferência e diminui o tamanho do modelo.
- **Exemplo de Uso:** Modelos implantados em dispositivos IoT para visão computacional.

## Knowledge Distillation

- **Objetivo:** Transferir o conhecimento de um modelo maior (teacher) para um modelo menor (student).
- **Vantagens:** Mantém a precisão com menor custo computacional.
- **Exemplo de Uso:** Assistentes pessoais virtuais com restrições de tempo de resposta.

## Fine-Tuning: Full vs. PEFT

- **Full Fine-Tuning:**
  - Ajusta todos os parâmetros do modelo pré-treinado.
  - **Vantagens:** Maior capacidade de personalização.
  - **Desvantagens:** Alto custo computacional, necessidade de grandes quantidades de dados e risco de catastrophic forgetting.
- **PEFT (Parameter-Efficient Fine-Tuning):**
  - Ajusta apenas um subconjunto dos parâmetros (ex.: LoRA, Adapters, Prompt Tuning).
  - **Vantagens:** Mais eficiência computacional e menor risco de overfitting.
  - **Desvantagens:** Pode ter menor capacidade de adaptação para tarefas muito complexas.

# 4. Métricas para Avaliar Desempenho e Ajuste de Hiperparâmetros

## Métricas de Desempenho

- **ROUGE:** Utilizado para avaliar a qualidade de resumos automáticos comparando-os com resumos de referência.
- **BLEU:** Mede a precisão de traduções automáticas comparando-as com traduções humanas, baseando-se em n-gramas.
- **BERTScore:** Utiliza embeddings para comparar a similaridade semântica entre textos gerados e textos de referência.

## Ajuste de Hiperparâmetros

- **Grid Search:** Testa exaustivamente todas as combinações possíveis de hiperparâmetros.
- **Random Search:** Avalia combinações de hiperparâmetros de forma aleatória, sendo mais eficiente em tempo.
- **Bayesian Optimization:** Utiliza métodos probabilísticos para identificar a melhor combinação de parâmetros.

## Parâmetros de Geração de Texto

- **Temperatura:** Determina a aleatoriedade na geração de texto; valores baixos resultam em previsões conservadoras, e valores altos promovem diversidade.
- **Top-P:** Seleciona palavras considerando a probabilidade acumulada, garantindo diversidade sem incluir previsões de baixa probabilidade.
- **Top-K:** Limita a seleção às K palavras mais prováveis.
- **Max-Length:** Restringe o número máximo de tokens gerados para evitar saídas excessivamente longas.

## Knowledge Cut-Off

- **Definição:** Limita o conhecimento do modelo a uma determinada janela de tokens ou contexto, evitando o uso de informações irrelevantes ou desatualizadas.

---

# 5. Inferência, Viés e Imparcialidade

## Conceitos de Inferência

- **Inferência:** Capacidade de um modelo de aplicar o conhecimento adquirido durante o treinamento em novos dados para gerar previsões ou saídas.

## Tipos de Inferência

- **Inferência em Lote (Batch Inference):**
  - Processa grandes volumes de dados de uma só vez.
  - _Exemplo:_ Geração de relatórios mensais com dados históricos.
- **Inferência em Tempo Real (Real-Time Inference):**
  - Processa dados instantaneamente, permitindo respostas imediatas.
  - _Exemplo:_ Sistemas de recomendação que sugerem conteúdos baseados na atividade recente dos usuários.
- **Inferência Edge:**
  - Realizada localmente em dispositivos finais, como smartphones ou dispositivos IoT.
  - _Exemplo:_ Reconhecimento facial em dispositivos móveis para desbloqueio.
- **Inferência Assíncrona (Asynchronous Inference):**
  - Processamento ocorre em segundo plano, suportando cargas variáveis sem impactar a experiência do usuário.
  - _Exemplo:_ Processamento de pedidos em plataformas de e-commerce.

## Outros Conceitos Relacionados

- **Dados Estruturados vs. Não Estruturados:**
  - _Estruturados:_ Dados organizados em formatos definidos, como tabelas.
  - _Não Estruturados:_ Dados sem um formato fixo, como textos, imagens, etc.
- **Underfitting vs. Overfitting:**
  - _Underfitting:_ Modelo simples demais, incapaz de capturar a complexidade dos dados.
  - _Overfitting:_ Modelo excessivamente complexo que se ajusta muito aos dados de treinamento, perdendo a capacidade de generalização.
- **Viés (Bias):**
  - Preconceitos ou distorções presentes nos dados ou algoritmos que podem levar a decisões injustas.
- **Imparcialidade (Fairness):**
  - Garantir que os modelos tomem decisões ou gerem previsões sem discriminar grupos ou indivíduos.

# 6. AWS Services

## Amazon Connect

- **Descrição:** Serviço na nuvem para a criação e gerenciamento de centrais de atendimento virtuais.
- **Recursos:** Suporte a voz, chat e integração com IA para melhorar a experiência do cliente.

## Amazon Bedrock

- **Descrição:** Serviço que possibilita o uso de Foundation Models da AWS.
- **Recursos e Modelos:**
  - **Modelos Base:** Utilizados sem ajustes adicionais.
  - **Modelos de Imagem e Texto:**
    - Preços baseados no número de tokens processados (para texto e embeddings) ou imagens geradas.
  - **Modos de Preço:**
    - **On-Demand:** Pagamento conforme uso, ideal para cargas de trabalho variáveis.
    - **Batch:** Processamento em lote com possibilidade de descontos.
    - **Provisioned Throughput:** Compra de capacidade de processamento por tempo determinado, adequado para reservas de capacidade.
- **Model Improvement Tech:**
  - **Prompt Engineering:** Ajuste do prompt sem necessidade de treinar o modelo.
  - **RAG (Retrieval-Augmented Generation):** Utiliza bases de conhecimento externas.
  - **Instruction Base Fine-Tuning e Domain Base Fine-Tuning:** Ajustes específicos para melhorar o desempenho em determinadas tarefas, com variáveis custos computacionais.

## Amazon SageMaker

- **Descrição:** Plataforma de Machine Learning totalmente gerenciada para criar, treinar e implantar modelos de forma escalável.
- **Principais Serviços:**
  - **SageMaker Studio:** Ambiente de desenvolvimento integrado.
  - **SageMaker Autopilot:** Automatiza a criação e treinamento de modelos.
  - **SageMaker Ground Truth & Ground Truth Plus:** Serviço para rotulagem de dados.
  - **SageMaker Hosting:** Hospedagem de modelos para inferência.
  - **SageMaker Pipelines:** Orquestração de fluxos de trabalho de ML.
  - **Edge Manager:** Gerenciamento de modelos para dispositivos de borda.
  - **Feature Store, Data Wrangler, Clarify, JumpStart, Model Monitor, Debugger, Experiments, Copilot:** Conjunto de serviços complementares que suportam o ciclo de vida completo do ML.
- **SageMaker Inference Options:**
  - **Real-Time Inference:** Respostas imediatas para aplicações de alta demanda e baixa latência.
  - **Asynchronous Inference:** Processamento para cargas maiores e com maior latência aceitável.
  - **Batch Transform:** Processamento offline de grandes volumes de dados.
  - **Serverless Inference:** Inferência escalável para tráfego intermitente sem gerenciamento de infraestrutura.

## Amazon Comprehend

- **Descrição:** Serviço de processamento de linguagem natural (NLP) que analisa sentimentos, extrai entidades e realiza classificação de documentos, entre outras tarefas.

## Amazon Titan

- **Descrição:** Modelo de linguagem de grande escala (Foundation Model) da AWS, treinado com 1 trilhão de parâmetros.
- **Aplicações:** Tarefas de NLP como tradução, resumo, geração e classificação de texto.

## AWS Inferentia

- Chip desenvolvido especialmente para acelerar a inferência de modelos de machine learning.
- Permite reduzir custos enquanto mantém alta performance para aplicações de inferência em larga escala.

## AWS Trainium

- Chip otimizado para treinamento de modelos de machine learning.
- Focado em oferecer alta velocidade e eficiência no treinamento, competindo com outras soluções de GPUs para deep learning.

# 7. Princípios de Responsible AI na AWS

- **Justiça (Fairness):**
  - Evita vieses indesejados nos modelos, garantindo igualdade no tratamento entre diferentes grupos.
- **Explicabilidade (Explainability):**
  - Fornece transparência na tomada de decisões e nos resultados dos modelos.
- **Privacidade & Segurança (Privacy & Security):**
  - Protege dados sensíveis e assegura conformidade com regulamentações.
- **Robustez & Confiabilidade (Robustness & Reliability):**
  - Garante que os modelos sejam resilientes e performáticos mesmo em condições adversas.
- **Governança (Governance):**
  - Estabelece controles contínuos para monitoramento e conformidade dos modelos.

# 9. Termos

- **GPT:** Transformer - Modelo gerador de texto e código com base em prompts.
- **BERT:** Transformer - Modelo que entende o contexto e a semântica das palavras.
- **SVM:** Support Vector Machine - Usado para tarefas de classificação e regressão.
- **GAN:** Generative Adversarial Network - Modelo que gera dados realísticos.
- **WAVE NET:** Rede Neural - Modelo que gera áudio realístico.
- **RESNET:** Rede Neural - Utilizado para reconhecimento de imagem.
- **IDP:** Intelligent Document Processing - Tecnologia para automação na captura, classificação e extração de informações de documentos.
- **PEFT:** Parameter-Efficient Fine-Tuning - Técnica de fine-tuning que ajusta apenas um subconjunto dos parâmetros de um modelo.

<p align="right">(<a href="#readme-top">back to top</a>)</p>
<!-- END_DOCS -->
