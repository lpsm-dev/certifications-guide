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

- [Definições avançadas](#defini%C3%A7%C3%B5es-avan%C3%A7adas)
  - [O que é Foundation Model?](#o-que-%C3%A9-foundation-model)
  - [O que é LLM (Large Language Model)?](#o-que-%C3%A9-llm-large-language-model)
  - [O que é Difussion Models?](#o-que-%C3%A9-difussion-models)
  - [O que é RAG (Retrieval-Augmented Generation)?](#o-que-%C3%A9-rag-retrieval-augmented-generation)
  - [O que é Fine-Tuning?](#o-que-%C3%A9-fine-tuning)
  - [Tipos de Aprendizado](#tipos-de-aprendizado)
    - [Aprendizado Supervisionado](#aprendizado-supervisionado)
    - [Aprendizado Não Supervisionado](#aprendizado-n%C3%A3o-supervisionado)
    - [Aprendizado Semi-Supervisionado](#aprendizado-semi-supervisionado)
    - [Aprendizado por Reforço](#aprendizado-por-refor%C3%A7o)
  - [O que é Clusterização?](#o-que-%C3%A9-clusteriza%C3%A7%C3%A3o)
  - [O que é IDP?](#o-que-%C3%A9-idp)
  - [O que é Modelo multimodal?](#o-que-%C3%A9-modelo-multimodal)
  - [O que é Prompt Engineering?](#o-que-%C3%A9-prompt-engineering)
  - [O que são Redes Neurais (Neural Networks)?](#o-que-s%C3%A3o-redes-neurais-neural-networks)
  - [O que é Regressão Linear?](#o-que-%C3%A9-regress%C3%A3o-linear)
  - [O que é K-Means Clustering?](#o-que-%C3%A9-k-means-clustering)
  - [O que é Árvore de Decisão (Decision Tree)](#o-que-%C3%A9-%C3%A1rvore-de-decis%C3%A3o-decision-tree)
  - [O que é Random Forest?](#o-que-%C3%A9-random-forest)
  - [O que é Support Vector Machine (SVM)?](#o-que-%C3%A9-support-vector-machine-svm)
  - [O que é PCA?](#o-que-%C3%A9-pca)
  - [O que é N-Gram?](#o-que-%C3%A9-n-gram)
  - [O que é AutoML?](#o-que-%C3%A9-automl)
  - [O que é Epochs?](#o-que-%C3%A9-epochs)
  - [O que é Accuracy (Acurácia) em Machine Learning?](#o-que-%C3%A9-accuracy-acur%C3%A1cia-em-machine-learning)
  - [O que é Hallucination?](#o-que-%C3%A9-hallucination)
- [Técnicas de Otimização em Machine Learning](#t%C3%A9cnicas-de-otimiza%C3%A7%C3%A3o-em-machine-learning)
- [PEFT (Parameter-Efficient Fine-Tuning) vs Full Fine-Tuning](#peft-parameter-efficient-fine-tuning-vs-full-fine-tuning)
- [Métricas para Avaliar Desempenho de Modelos](#m%C3%A9tricas-para-avaliar-desempenho-de-modelos)
- [Conceitos e Técnicas Complementares](#conceitos-e-t%C3%A9cnicas-complementares)
- [Inferência, Viés e Imparcialidade](#infer%C3%AAncia-vi%C3%A9s-e-imparcialidade)
- [Tipos de Inferência](#tipos-de-infer%C3%AAncia)
- [Dados Estruturados vs. Não Estruturados](#dados-estruturados-vs-n%C3%A3o-estruturados)
- [Underfitting vs. Overfitting](#underfitting-vs-overfitting)
- [Hiperparâmetros](#hiperpar%C3%A2metros)
- [Temperatura, Top-P, Top-K e Max-Length](#temperatura-top-p-top-k-e-max-length)
- [O que é Knowledge Cut-Off?](#o-que-%C3%A9-knowledge-cut-off)
- [AWS Services](#aws-services)
  - [Amazon Connect](#amazon-connect)
  - [Amazon Bedrock](#amazon-bedrock)
  - [Amazon SageMaker](#amazon-sagemaker)
  - [Amazon Comprehend](#amazon-comprehend)
  - [Amazon Titan](#amazon-titan)
- [Princípios de Responsible AI na AWS](#princ%C3%ADpios-de-responsible-ai-na-aws)
- [Terms](#terms)

<!-- END doctoc generated TOC please keep comment here to allow auto update -->

<p align="right">(<a href="#readme-top">back to top</a>)</p>

</details>

# Definições avançadas

## O que é Foundation Model?

Foundation Models (FMs) são modelos de linguagem de grande escala pré-treinados em grandes conjuntos de dados para capturar conhecimento geral da linguagem. Eles são usados como base para tarefas específicas de NLP, como tradução, resumo, geração de texto, classificação de texto, entre outros.

## O que é LLM (Large Language Model)?

Large Language Models (LLMs) são modelos de linguagem de grande escala treinados em grandes conjuntos de dados para capturar conhecimento geral da linguagem. Eles são usados para tarefas de NLP, como tradução, resumo, geração de texto, classificação de texto, entre outros.

## O que é Difussion Models?

Difussion Models são modelos de linguagem que geram previsões baseadas em uma combinação de amostras de texto e amostras de ruído. Eles são usados para gerar previsões mais diversificadas e criativas, evitando previsões repetitivas e conservadoras.

## O que é RAG (Retrieval-Augmented Generation)?

RAG (Retrieval-Augmented Generation) é um modelo de linguagem que combina geração de texto com recuperação de informações. Ele gera previsões baseadas em um modelo de geração de texto e uma base de conhecimento externa, como documentos, páginas da web, ou bancos de dados.

## O que é Fine-Tuning?

Fine-Tuning é uma técnica de ajuste de modelos de Machine Learning pré-treinados para tarefas específicas. Ele envolve treinar um modelo pré-treinado em um novo conjunto de dados para melhorar o desempenho em uma tarefa específica.

Escolher o número ideal de epochs é crucial para evitar underfitting (treinar pouco) e overfitting (treinar demais). Algumas métricas ajudam a identificar esse ponto ótimo.

- **Training & Validation Loss**:
  - O objetivo é minimizar a perda (loss) sem que ela volte a subir.
  - O ponto ótimo ocorre quando a perda de validação para de diminuir e começa a estabilizar ou aumentar.
- **Training & Validation Accuracy**:
  - O objetivo é maximizar a acurácia sem que ela comece a cair.
  - O ponto ótimo ocorre quando a acurácia de validação para de aumentar e começa a estabilizar ou diminuir.
- **Early Stopping**
  - Técnica usada para interromper o treinamento quando a perda de validação começa a aumentar.
  - Evita overfitting e encontra o ponto ótimo de treinamento.

## Tipos de Aprendizado

### Aprendizado Supervisionado

- Objetivo: O objetivo do aprendizado supervisionado é treinar um modelo utilizando dados rotulados para que ele possa prever a saída correta para novas entradas não vistas.
- Exemplos:
  - Classificação de E-mails: Identificar se um e-mail é spam ou não spam.
  - Previsão de Preços de Casas: Estimar o preço de uma casa com base em características como localização, tamanho e número de quartos.
- Algoritmos:
  - Regressão Linear: Usado para prever valores contínuos.
  - Árvores de Decisão: Utilizadas para classificação e regressão.
  - Support Vector Machines (SVM): Usadas para classificação, especialmente em problemas com margens claras de separação.
  - Redes Neurais: Aplicadas em tarefas complexas como reconhecimento de imagem e processamento de linguagem natural.
- Características:
  - Necessidade de Dados Rotulados: Requer um conjunto de dados de treinamento com entradas e saídas conhecidas.
  - Aplicações: Reconhecimento de fala, diagnóstico médico, sistemas de recomendação.

### Aprendizado Não Supervisionado

- Objetivo: O aprendizado não supervisionado busca encontrar padrões ou estruturas inerentes nos dados sem a necessidade de rótulos explícitos.
- Exemplos:
  - Segmentação de Clientes: Agrupar clientes com base em comportamentos de compra semelhantes.
  - Detecção de Anomalias: Identificar transações fraudulentas em dados financeiros.
- Algoritmos Comuns:
  - K-Means Clustering: Utilizado para agrupar dados em K grupos distintos.
  - Análise de Componentes Principais (PCA): Usado para redução de dimensionalidade e visualização de dados.
  - Redes Neurais Autoencoders: Aplicadas para compressão de dados e detecção de anomalias.
- Características:
  - Exploratório: Não há necessidade de dados rotulados, o que permite a descoberta de estruturas ocultas.
  - Aplicações: Análise de mercado, compressão de dados, bioinformática.

### Aprendizado Semi-Supervisionado

- Objetivo: Combina elementos de aprendizado supervisionado e não supervisionado para melhorar o desempenho do modelo utilizando um pequeno conjunto de dados rotulados e um grande conjunto de dados não rotulados.
- Exemplos:
  - Classificação de Textos: Usar um pequeno conjunto de textos rotulados para treinar um modelo que classifica uma grande quantidade de dados não rotulados.
  - Reconhecimento Facial: Aprimorar a precisão de modelos de reconhecimento facial com base em um pequeno conjunto de imagens rotuladas.
- Algoritmos Comuns:
  - Modelos de Propagação de Rótulos: Usados para propagar rótulos de dados rotulados para não rotulados.
  - Redes Neurais Semi-Supervisionadas: Aproveitam o aprendizado não supervisionado para melhorar a generalização.
- Características:
  - Eficiência de Dados: Maximiza o uso de dados disponíveis, reduzindo a necessidade de grandes quantidades de dados rotulados.
  - Aplicações: Análise de dados médicos, reconhecimento de imagem em larga escala.

### Aprendizado por Reforço

O aprendizado por reforço é uma técnica de aprendizado de máquina em que um agente interage com um ambiente dinâmico para aprender a tomar ações que maximizam uma recompensa. Ele é usado em jogos, robótica, otimização e controle de processos.

Utiliza uma estratégia de tentativa e erro, onde o agente toma ações, observa o resultado e ajusta sua política de ação para maximizar a recompensa ao longo do tempo.

## O que é Clusterização?

Clusterização é uma técnica de aprendizado não supervisionado usada para agrupar dados semelhantes em clusters ou grupos. O objetivo é encontrar padrões ou estruturas nos dados que não são rotulados.

## O que é IDP?

Intelligent Document Processing (IDP) é uma tecnologia que automatiza a captura, classificação e extração de dados de documentos estruturados, semiestruturados e não estruturados. Ele combina OCR (Reconhecimento Óptico de Caracteres), Processamento de Linguagem Natural (NLP), Machine Learning (ML) e IA para transformar documentos em informações processáveis digitalmente

## O que é Modelo multimodal?

Modelos multimodais são modelos de IA que processam e combinam informações de diferentes modalidades, como texto, imagem, áudio e vídeo. Eles são usados em tarefas de NLP, visão computacional, reconhecimento de fala e multimídia.

Eles possuem inputs e outputs em diferentes formatos e modalidades, permitindo a análise e geração de conteúdo multimodal.

## O que é Prompt Engineering?

Prompt Engineering é uma técnica usada para projetar prompts ou instruções específicas para modelos de linguagem gerarem previsões desejadas. Ele ajuda a controlar o comportamento e a qualidade das previsões geradas por modelos de linguagem.

## O que são Redes Neurais (Neural Networks)?

As redes neurais são modelos computacionais inspirados no funcionamento do cérebro humano, usadas principalmente em aprendizado de máquina (ML) e inteligência artificial (IA). Elas são compostas por neurônios artificiais organizados em camadas, que processam e aprendem padrões a partir de dados.

## O que é Regressão Linear?

A Regressão Linear é um modelo de aprendizado supervisionado usado para prever valores numéricos com base em variáveis independentes. O objetivo é encontrar a melhor linha reta que se ajusta aos dados, minimizando a diferença entre os valores previstos e reais.

## O que é K-Means Clustering?

O K-Means é um algoritmo de aprendizado não supervisionado usado para agrupar dados em K grupos (clusters). Ele tenta minimizar a distância dentro dos clusters e maximizar a separação entre os clusters.

## O que é Árvore de Decisão (Decision Tree)

Uma Árvore de Decisão é um modelo de aprendizado supervisionado usado para classificação e regressão. Ele divide os dados em ramificações baseadas em perguntas que minimizam a impureza.

## O que é Random Forest?

Random Forest é um modelo de aprendizado supervisionado que combina várias árvores de decisão para melhorar a precisão e reduzir o overfitting. Ele treina várias árvores em subconjuntos aleatórios dos dados e faz previsões com base na média ou votação das árvores.

## O que é Support Vector Machine (SVM)?

Support Vector Machine (SVM) é um modelo de aprendizado supervisionado usado para classificação e regressão. Ele encontra o hiperplano que melhor separa os dados em classes, maximizando a margem entre as classes.

## O que é PCA?

PCA (Principal Component Analysis) é uma técnica de redução de dimensionalidade usada para projetar dados em um espaço de menor dimensão. Ele encontra os componentes principais que capturam a maior variância nos dados.

## O que é N-Gram?

N-Gram é uma sequência contígua de N itens (palavras, caracteres, tokens) em um texto. É usado em NLP para capturar a estrutura e a semântica dos dados.

Seu objetivo é capturar a estrutura e a semântica dos dados, considerando a ordem e a proximidade das palavras.

## O que é AutoML?

AutoML (Automated Machine Learning) é um conjunto de técnicas e ferramentas que automatizam o processo de construção, treinamento e ajuste de modelos de Machine Learning. Ele ajuda a acelerar o desenvolvimento de modelos e reduzir a necessidade de conhecimento especializado.

## O que é Epochs?

No contexto de AWS AI/ML, epochs (ou épocas) representam o número de vezes que um modelo de machine learning percorre todo o conjunto de dados de treinamento.

## O que é Accuracy (Acurácia) em Machine Learning?

Accuracy (Acurácia) é uma métrica de avaliação usada em modelos de classificação para medir a proporção de previsões corretas em relação ao total de amostras analisadas.

## O que é Hallucination?

Hallucination é um fenômeno em modelos de linguagem em que o modelo gera previsões incorretas ou fictícias, sem base nos dados de entrada. Pode ocorrer devido a overfitting, falta de dados de treinamento ou problemas na arquitetura do modelo.

# Técnicas de Otimização em Machine Learning

**Prunning**:

- Objetivo: Remover partes desnecessárias de um modelo, como neurônios ou camadas.
- Vantagens:
  - Reduz o tamanho do modelo.
  - Melhora a eficiência computacional.
- Como funciona: Identifica e remove parâmetros que pouco contribuem para o desempenho do modelo.
- Exemplo de Uso: Em redes neurais profundas para dispositivos móveis, onde a eficiência e o uso de memória são cruciais.

**Quantization**:

- Objetivo: Reduzir a precisão numérica dos modelos.
- Vantagens:
  - Acelera a inferência.
  - Reduz o tamanho do modelo.
- Como funciona: Transforma valores de ponto flutuante (FP32) em formas mais compactas como INT8.
- Exemplo de Uso: Implementação em dispositivos IoT para modelos de visão computacional

**Knowledge Distillation**:

- Objetivo: Criar um modelo menor (student) que aprende com um maior (teacher).
- Vantagens: Mantém a precisão enquanto reduz a quantidade de recursos exigidos.
- Como funciona:
  - Usado quando é necessário implantar modelos em dispositivos com recursos limitados.
- Exemplo de Uso: Em assistentes pessoais virtuais, onde o tempo de resposta é crítico.

**Fine-Tuning**:

- Objetivo: Ajustar modelos pré-treinados para novas aplicações.
- Vantagens:
  - Necessita de menos dados para treinar.
  - Aproveita conhecimento anterior.
- Exemplo de Uso: Ajuste de modelos de linguagem como BERT para tarefas específicas de análise de sentimento.
- Tipos:
  - **Full Fine-Tuning**:
    - Ajusta todos os parâmetros do modelo e requer muitos recursos computacional.
    - Indicado quando a tarefa-alvo é significativamente diferente da tarefa original do modelo pré-treinado.
  - **Parameter-Efficient Fine-Tuning (PEFT)**:
    - Ajusta apenas um subconjunto de parâmetros.
    - Indicado quando a tarefa-alvo é semelhante à tarefa original do modelo pré-treinado.

# PEFT (Parameter-Efficient Fine-Tuning) vs Full Fine-Tuning

A principal diferença entre PEFT (Parameter-Efficient Fine-Tuning) e Full Fine-Tuning está na quantidade de parâmetros ajustados durante o treinamento de um modelo de machine learning, especialmente em Large Language Models (LLMs) e Foundation Models (FMs).

**Full Fine-Tuning**

No Full Fine-Tuning, todos os pesos e parâmetros do modelo pré-treinado são ajustados para uma nova tarefa.

Vantagens:

- Permite maior adaptação do modelo para tarefas específicas.
- Maior capacidade de ajuste fino e personalização.

Desvantagens:

- Altíssimo custo computacional (precisa de mais memória e GPUs).
- Demanda grandes quantidades de dados rotulados.
- Pode causar catastrophic forgetting, onde o modelo perde conhecimento original.

**PEFT (Parameter-Efficient Fine-Tuning)**

O PEFT ajusta apenas um pequeno subconjunto dos parâmetros do modelo, mantendo a maior parte dos pesos congelados. Métodos populares incluem LoRA (Low-Rank Adaptation), Adapters, e Prompt Tuning.

Vantagens:

- Muito mais eficiente – reduz custo computacional e consumo de memória.
- Menos risco de overfitting – menos parâmetros treináveis ajudam a evitar sobreajuste.
- Facilidade de adaptação – pode ser aplicado a múltiplas tarefas sem precisar treinar o modelo inteiro.

Desvantagens:

- Pode ter menor capacidade de adaptação para mudanças drásticas nos dados.
- Nem sempre atinge o mesmo desempenho do Full Fine-Tuning para tarefas muito complexas.

# Métricas para Avaliar Desempenho de Modelos

Na avaliação de modelos de Machine Learning, é crucial utilizar métricas adequadas para determinar a qualidade e a eficácia das saídas geradas pelos modelos em tarefas específicas. Aqui estão algumas das métricas mais comuns:

**ROUGE**:

- Utilização: Avaliação de resumos automáticos.
- Objetivo: Mede a qualidade de resumos gerados automaticamente, comparando-os com resumos de referência criados por humanos.
- Exemplo de Uso: Utilizado em sistemas de geração de resumos de artigos científicos ou notícias para garantir que a essência do conteúdo original seja capturada adequadamente.

**BLEU**:

- Utilização: Tradução automática.
- Objetivo: Avalia a precisão de traduções automáticas comparando-as com traduções humanas de referência, utilizando correspondência de n-gramas.
- Exemplo de Uso: Avaliação de serviços de tradução automática, como aqueles implementados em plataformas de e-commerce para traduzir descrições de produtos.

**BERTScore**:

- Utilização: Avaliação de captura semântica.
- Objetivo: Usa embeddings de BERT para avaliar a similaridade semântica entre textos gerados e textos de referência, compreendendo o contexto e a semântica.
- Exemplo de Uso: Avaliação de chatbots ou assistentes virtuais, garantindo que as respostas geradas sejam contextualmente apropriadas e semanticamente corretas.

# Conceitos e Técnicas Complementares

**Vector Embeddings**

- Conceito: Encapsulam dados em representações numéricas de alta dimensão.
- Aplicações: NLP, motores de busca semânticos e recomendações.
- Exemplo de Uso: Embeddings de palavras em sistemas de recomendação de filmes.

**Chunking**

- Finalidade: Dividir dados em segmentos menores.
- Utilização: Digestão mais fácil para armazenamento e análise em modelos maiores de IA.
- Exemplo de Uso: Processamento de grandes conjuntos de dados de texto em sistemas de análise de sentimento.

**Tokenization**

- Definição: É o processo de dividir um texto em unidades menores chamadas tokens, que podem ser palavras, subpalavras, caracteres ou até mesmo pedaços de palavras.
- Utilização: Pré-processamento de texto para análise de linguagem natural (NLP).

# Inferência, Viés e Imparcialidade

**Inferência**:

- Definição: Inferência refere-se à capacidade de um modelo de Machine Learning de fazer previsões ou gerar saídas com base em novos dados, usando o conhecimento adquirido durante o treinamento.
- Exemplo de Uso: Em sistemas financeiros, um modelo pode usar inferência para prever fluxos de caixa futuros com base em dados históricos e transações recentes.

**Viés** (Bias):

- Definição: Viés em Machine Learning refere-se a preconceitos ou distorções nos dados ou nos algoritmos que podem levar a decisões injustas ou imprecisas.
- Origem: Pode surgir de dados desbalanceados, amostras não representativas, ou algoritmos que não consideram todas as variáveis relevantes.
- Exemplo de Uso: Avaliação de viés em sistemas de recrutamento automatizados, onde o viés pode afetar a seleção de candidatos com base em dados históricos enviesados.

**Imparcialidade** (Fairness):

- Definição: Imparcialidade significa garantir que os modelos de Machine Learning façam previsões justas e equitativas para todos os grupos, sem discriminação ou preconceito.
- Como alcançar: Desenvolver modelos que sejam neutros em relação a atributos sensíveis, como gênero, raça ou idade, e utilizar técnicas de mitigação de viés durante o treinamento.
- Exemplo de Uso: Implementação de modelos de crédito que avaliem a elegibilidade de candidatos sem discriminação, assegurando que todos tenham acesso justo a oportunidades financeiras.

# Tipos de Inferência

**Inferência em Lote (Batch Inference)**

- Descrição: Este tipo de inferência processa grandes conjuntos de dados de uma só vez. É adequado para situações onde não é necessário um resultado imediato.
- Exemplo de Uso: Análise de dados históricos para gerar relatórios de vendas mensais em uma empresa de varejo. Os dados são processados durante a noite para fornecer insights no início do próximo dia útil.

**Inferência em Tempo Real (Real-Time Inference)**

- Descrição: Processa dados instantaneamente à medida que chegam, permitindo previsões imediatas.
- Exemplo de Uso: Sistemas de recomendação em plataformas de streaming, que sugerem novos conteúdos aos usuários com base em suas atividades recentes e preferências.

**Inferência Edge**

- Descrição: Realiza o processamento localmente em dispositivos finais, como smartphones ou dispositivos IoT, minimizando a necessidade de comunicação com um servidor central.
- Exemplo de Uso: Reconhecimento facial em smartphones para desbloqueio seguro, onde o processamento é feito no próprio dispositivo para aumentar a segurança e a velocidade.

**Inferência Assíncrona (Asynchronous Inference)**

- Descrição: Os dados são processados em segundo plano, em vez de imediatamente, permitindo que o sistema suporte cargas de trabalho variáveis sem impactar a experiência do usuário.
- Exemplo de Uso: Processamento de pedidos em sistemas de e-commerce, onde a validação e a confirmação do pedido podem ser realizadas sem interromper a navegação do usuário na plataforma.

# Dados Estruturados vs. Não Estruturados

- Estruturados: Organizados em esquemas conhecidos, como tabelas.
- Não Estruturados: Sem um formato fixo, por exemplo, texto e imagens.
- Exemplo de Uso: Análise de dados de redes sociais (texto livre) para tendências de marketing.

# Underfitting vs. Overfitting

- **Underfitting**
  - Ocorre quando um modelo é muito simples para capturar a complexidade dos dados.
  - O modelo não consegue aprender padrões nos dados de treinamento e tem baixo desempenho.
  - Solução: aumentar a complexidade do modelo, adicionar mais dados, ajustar hiperparâmetros.
- **Overfitting**
  - Ocorre quando um modelo é muito complexo e se ajusta demais aos dados de treinamento.
  - O modelo aprende padrões específicos dos dados de treinamento que não se generalizam para novos dados.
  - Solução: simplificar o modelo, adicionar regularização, aumentar dados de treinamento.

# Hiperparâmetros

Hiperparâmetros são configurações ajustáveis que controlam o comportamento e desempenho de um modelo de Machine Learning. Eles são definidos antes do treinamento e não são aprendidos pelo modelo.

As técnicas comuns para ajustar hiperparâmetros incluem:

- **Grid Search**:
  - Testa todas as combinações possíveis de hiperparâmetros em uma grade.
  - Pode ser lento e exigir muitos recursos computacionais.
- **Random Search**:
  - Testa aleatoriamente um subconjunto de combinações de hiperparâmetros.
  - Mais eficiente que Grid Search e pode encontrar boas combinações rapidamente.
- **Bayesian Optimization**:
  - Usa métodos probabilísticos para encontrar a melhor combinação de hiperparâmetros.
  - Mais eficiente que Grid Search e Random Search para otimização de hiperparâmetros.

# Temperatura, Top-P, Top-K e Max-Length

- **Temperatura**:
  - Controla a aleatoriedade das previsões geradas por um modelo de linguagem.
  - Baixa temperatura: previsões mais conservadoras e repetitivas.
  - Alta temperatura: previsões mais diversificadas e criativas.
- **Top-P**:
  - Gera previsões baseadas nas probabilidades cumulativas das palavras mais prováveis, até atingir uma probabilidade acumulada definida.
  - Evita previsões de baixa probabilidade e gera previsões mais diversificadas.
- **Top-K**:
  - Gera previsões baseadas nas K palavras mais prováveis, excluindo palavras menos prováveis.
  - Evita previsões de baixa probabilidade e gera previsões mais diversificadas.
- **Max-Length**:
  - Limita o número de tokens gerados em uma previsão.
  - Evita previsões muito longas e controla a extensão das previsões.

# O que é Knowledge Cut-Off?

Knowledge Cut-Off é uma técnica usada para limitar o conhecimento de um modelo de linguagem a um determinado contexto ou janela de tokens. Ele ajuda a controlar a extensão do conhecimento do modelo e a evitar previsões baseadas em informações irrelevantes ou distantes.

# AWS Services

## Amazon Connect

Amazon Connect é um serviço de central de atendimento na nuvem que permite criar e gerenciar centrais de atendimento virtuais de forma escalável e flexível. Ele oferece recursos de voz, chat e integração com IA para melhorar a experiência do cliente.

## Amazon Bedrock

- Watermark Detection: Cria imagens com amazon Titan
- Pricing:
  - **On-Demand**:
    - Pay as you go. Sem compromissos.
    - Text e Embedding Models: cobrados por cada input/output token processado.
    - Image Models: cobrados por cada imagem gerada.
    - Funciona só com modelos base.
    - Bom para cargas de trabalho não previsíveis e sem comprometimento de tempo.
  - **Batch**:
    - Várias predições no mesmo tempo (joga o output em um único S3)
    - Pode promober 50% de descontos.
  - **Provisioned Throughput**:
    - Compre unidades de um modelo por um determinado tempo
    - Throughput é a quantidade de tokens que você pode processar por minutos.
    - Não necessariamente é o melhor em custos.
    - Funciona com Base, Fine-Tuned e Custom Models.
    - Bom para reservar a capacidade.

Model Improvement Tech Cust Order

1. Prompt Engineering: Não precisa de model training. Apenas ajusta o prompt.
2. RAG: Usa bases de conhecimento externas e não muda o FM.
3. Instruction Base Fine-Tuning: Ajusta o FM com instruções específicas. Precisa de recurso computacional.
4. Domain Base Fine-Tuning: Ajusta o FM para um domínio específico. Precisa de mt recurso computacional.

> - Temp, Top K e Top P não impactam no preço do modelo. Oq impacta é a quantidade de token (maior causa de aumento de custo)
> - Modelos pequenos são mais baratos.

## Amazon SageMaker

Amazon SageMaker é um serviço de Machine Learning totalmente gerenciado que permite criar, treinar e implantar modelos de Machine Learning de forma rápida e escalável. Ele oferece uma plataforma integrada para todo o ciclo de vida do Machine Learning, desde a preparação dos dados até a implantação dos modelos.

Seus principais serviços são:

- **Amazon SageMaker Studio**: Ambiente de desenvolvimento integrado para criar, treinar e implantar modelos de Machine Learning.
- **Amazon SageMaker Autopilot**: Automatiza o processo de construção e treinamento de modelos de Machine Learning.
- **Amazon SageMaker Ground Truth**: Serviço de rotulagem de dados para treinar modelos de Machine Learning.
- **Amazon SageMaker Hosting**: Serviço de hospedagem de modelos de Machine Learning para inferência em escala.
- **Amazon SageMaker Pipelines**: Serviço de automação de pipelines de Machine Learning para orquestrar o ciclo de vida dos modelos.
- **Amazon SageMaker Edge Manager**: Serviço de gerenciamento de modelos de Machine Learning em dispositivos de borda.
- **Amazon SageMaker Feature Store**: Serviço de armazenamento e gerenciamento de features para modelos de Machine Learning.
- **Amazon SageMaker Data Wrangler**: Serviço de preparação de dados para Machine Learning.
- **Amazon SageMaker Clarify**: Serviço de detecção de viés e interpretabilidade de modelos de Machine Learning.
- **Amazon SageMaker JumpStart**: Catálogo de modelos de Machine Learning pré-treinados e aceleradores de Machine Learning.
- **Amazon SageMaker Model Monitor**: Serviço de monitoramento de modelos de Machine Learning em produção.
- **Amazon SageMaker Debugger**: Serviço de depuração de modelos de Machine Learning para identificar problemas de desempenho e qualidade.
- **Amazon SageMaker Experiments**: Serviço de rastreamento e gerenciamento de experimentos de Machine Learning.
- **Amazon SageMaker Copilot**: Assistente de desenvolvimento de Machine Learning para acelerar o desenvolvimento de modelos.

> Amazon SageMaker Ground Truth Plus é um serviço gerenciado da AWS que facilita a rotulagem de dados para treinamento de modelos de machine learning, sem necessidade de gerenciar a infraestrutura ou equipes de anotação.

SageMaker Inference options

- Real-Time Inference: Immediate responses for high-traffic, low-latency applications.
- Asynchronous Inference: Near real-time for large payloads and longer processing.
- Batch Transform: Large-scale, offline processing without real-time needs.
- Serverless Inference: Low-latency inference for intermittent or unpredictable traffic without managing infrastructure.

## Amazon Comprehend

Serviço capaz de fazer processamento de linguagem natural (PLN) para análise de sentimentos, extração de entidades, classificação de documentos, entre outras tarefas.

## Amazon Titan

É o FM da AWS, que é um modelo de linguagem de grande escala treinado em 1 trilhão de parâmetros. Ele é usado para tarefas de NLP, como tradução, resumo, geração de texto, classificação de texto, entre outros.

# Princípios de Responsible AI na AWS

A AWS adota princípios fundamentais para o desenvolvimento responsável da IA:

- Justiça (Fairness) – Evita vieses indesejados nos modelos de IA.
- Explicabilidade (Explainability) – Fornece transparência nos resultados dos modelos.
- Privacidade & Segurança (Privacy & Security) – Protege dados e garante conformidade regulatória.
- Robustez & Confiabilidade (Robustness & Reliability) – Garante modelos resilientes e de alto desempenho.
- Governança (Governance) – Estabelece controles para monitoramento contínuo e conformidade.

# Terms

- GPT: Transformer - Gera texto e código humano com base em inputs
- BERT: Transformer - Entende contexto e semântica de palavras
- SVM: Support Vector Machine - Classificação e regressão
- GAN: Generative Adversarial Network - Gera dados realísticos.
- WAVE NET: Rede Neural - Gera áudio realístico.
- RESNET: Rede Neural - Reconhecimento de imagem.

<p align="right">(<a href="#readme-top">back to top</a>)</p>
<!-- END_DOCS -->
