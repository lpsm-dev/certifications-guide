# Anotações

## Como técnicas de optimização de machine learning, temos:

- **Prunning**:
  - Seu objetivo é remover partes desnecessárias do modelo para reduzir o tamanho e melhorar a eficiência.
  - Redes neurais possuiem muitos parâmetros, e muitos deles podem ser desnecessários. O prunning indentifica e remove os parâmetros que não são necessários.
- **Quantization**:
  - Seu objetivo é reduzir a precisão numérica dos pesos/ativações para acelerar a inferência e diminuir tamanho do modelo.
  - Modelos treinam usando valores em ponto flutuante (FP32). A quantização reduz a precisão para FP16, INT8 ou até INT4, reduzindo o tamanho do modelo e acelerando cálculos.
- **Knowledge Distillation**:
  - Seu objetivo é criar um modelo menor (student model) que aprende a partir de um modelo grande (teacher model), preservando o desempenho.
  - Modelos maiores são mais precisos, mas também mais lentos e consomem mais recursos. O conhecimento de um modelo maior pode ser transferido para um modelo menor, mais rápido e eficiente.
- **Fine-Tuning**:
  - Seu objetivo é ajustar um modelo pré-treinado (FM) para um novo conjunto de dados (nova tarefa específica), em vez de treinar um modelo do zero.
  - FMs são treinados em grandes conjuntos de dados e podem ser ajustados para tarefas específicas com menos dados e tempo.

## Métricas para avaliar o desempenho de um FM:

- **ROUGE**:
  - Usado principalmente para avaliação de resumos automáticos e geração de texto.
  - Calcula a similaridade entre um resumo gerado automaticamente com uma referência humana.
- **BLEU**:
  - Usado principalmente para avaliação de tradução automática.
  - Calcula a similaridade entre uma tradução gerada automaticamente com uma referência humana, com base em n-gramas.
  - Usa um penalizador de comprimento para evitar frases curtas que maximizem a precisão.
- **BERTScore**:
  - Calcula a similaridade entre uma tradução gerada automaticamente com uma referência humana, com base em embeddings de palavras.
  - Captura significados em diferentes palavras, enquanto BLEU/ROUGE dependem de correspondências exatas de palavras.

> Se precisar de uma métrica robusta para semântica, BERTScore é melhor. Se precisar de uma métrica leve para resumo/tradução, BLEU ou ROUGE são boas opções.

## O que são Vector Embeddings?

Vector embeddings são representações numéricas de dados, transformadas em vetores de alta dimensão. Eles são amplamente usados em Machine Learning, NLP, busca semântica e recomendações para capturar significados e relações entre palavras, imagens, ou qualquer outro tipo de dado.

O objetivo dos embeddings é converter dados não estruturados (como palavras ou imagens) em vetores numéricos, preservando seus significados e relações no espaço vetorial. Isso facilita operações como similaridade, classificação e clustering.

## O que é Chunking?

Chunking é uma técnica usada para dividir um grande conjunto de dados em partes menores (chamadas de "chunks") para facilitar o processamento, armazenamento ou análise.

## Inferência, Viés e Imparcialidade

- **Inferência**:
  - Inferência refere-se à capacidade de um modelo de fazer previsões utilizando novos dados com base no que aprendeu durante o treinamento.
  - Modelos de Machine Learning são treinados em dados históricos para fazer previsões sobre novos dados.
- **Viés** (Bias):
  - Viés refere-se a preconceitos ou distorções nos dados ou algoritmos que podem levar a decisões injustas ou imprecisas.
  - Viés pode surgir de dados desbalanceados, amostras não representativas, ou algoritmos discriminatórios.
  - Pode ser dos dados, algoritmo ou humano.
- **Imparcialidade** (Fairness):
  - Imparcialidade refere-se à ausência de viés ou discriminação em modelos de Machine Learning (decisões justas e equitativas).
  - Modelos imparciais devem fazer previsões justas e precisas para todos os grupos, sem discriminação ou preconceito.

## Tipos de Inferência

- **Inferência em lote**:
  - Processa um grande conjunto de dados de uma só vez.
  - Usado para treinamento, validação e teste de modelos.
  - Ex: Recomendações de produtos geradas uma vez ao dia.
- **Inferência em tempo real**:
  - Processa dados em tempo real, à medida que chegam.
  - Usado para previsões em tempo real, detecção de fraudes, recomendações em tempo real.
  - Ex: Detecção de fraudes bancárias instantaneamente
- **Inferência Edge**:
  - Processa dados localmente em dispositivos de borda (IoT, sensores, dispositivos móveis).
  - Usado para aplicações de IoT, visão computacional, reconhecimento de fala.
  - Ex: Reconhecimento facial em um smartphone.
- **Inferência Assíncrona**:
  - Processa dados em segundo plano, sem interrupção do usuário.
  - Ideal para cargas de trabalho variáveis.
  - Ex: Sistemas de análise de documentos enviados por usuários.

## Dados Estruturados vs. Não Estruturados

- **Dados Estruturados**:
  - Dados organizados em tabelas ou formatos tabulares, com colunas e linhas bem definidas.
  - Exemplos: bancos de dados, planilhas, CSV.
  - Fácil de processar, analisar e visualizar.
- **Dados Não Estruturados**:
  - Dados sem formato definido, como texto, imagens, áudio, vídeo.
  - Exemplos: texto livre, imagens, vídeos, áudio.
  - Difícil de processar, analisar e extrair informações.

## Underfitting vs. Overfitting

- **Underfitting**:
  - Ocorre quando um modelo é muito simples para capturar a complexidade dos dados.
  - O modelo não consegue aprender padrões nos dados de treinamento e tem baixo desempenho.
  - Solução: aumentar a complexidade do modelo, adicionar mais dados, ajustar hiperparâmetros.
- **Overfitting**:
  - Ocorre quando um modelo é muito complexo e se ajusta demais aos dados de treinamento.
  - O modelo aprende padrões específicos dos dados de treinamento que não se generalizam para novos dados.
  - Solução: simplificar o modelo, adicionar regularização, aumentar dados de treinamento.

## Hiperparâmetros

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

## Temperatura, Top-P, Top-K e Max-Length

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

## Aprendizado Supervisionado vs. Não Supervisionado

- **Aprendizado Supervisionado**:
  - Algoritmos de Machine Learning treinados em pares de entrada/saída rotulados.
  - Objetivo: prever a saída correta para novas entradas com base no treinamento.
  - Exemplos: classificação, regressão.
- **Aprendizado Não Supervisionado**:
  - Algoritmos de Machine Learning treinados em entradas não rotuladas.
  - Objetivo: descobrir padrões, estruturas ou relações nos dados.
  - Exemplos: clustering, redução de dimensionalidade.
- **Aprendizado Semi-Supervisionado**:
  - Combina elementos de aprendizado supervisionado e não supervisionado.
  - Usa um pequeno conjunto de dados rotulados e um grande conjunto de dados não rotulados.
  - Objetivo: melhorar o desempenho do modelo com dados não rotulados.

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

## O que é Knowledge Cut-Off?

Knowledge Cut-Off é uma técnica usada para limitar o conhecimento de um modelo de linguagem a um determinado contexto ou janela de tokens. Ele ajuda a controlar a extensão do conhecimento do modelo e a evitar previsões baseadas em informações irrelevantes ou distantes.

## O que é Foundation Model?

Foundation Models (FMs) são modelos de linguagem de grande escala pré-treinados em grandes conjuntos de dados para capturar conhecimento geral da linguagem. Eles são usados como base para tarefas específicas de NLP, como tradução, resumo, geração de texto, classificação de texto, entre outros.

## O que é LLM (Large Language Model)?

Large Language Models (LLMs) são modelos de linguagem de grande escala treinados em grandes conjuntos de dados para capturar conhecimento geral da linguagem. Eles são usados para tarefas de NLP, como tradução, resumo, geração de texto, classificação de texto, entre outros.

## O que é Difussion Models?

Difussion Models são modelos de linguagem que geram previsões baseadas em uma combinação de amostras de texto e amostras de ruído. Eles são usados para gerar previsões mais diversificadas e criativas, evitando previsões repetitivas e conservadoras.

## O que é Clusterização?

Clusterização é uma técnica de aprendizado não supervisionado usada para agrupar dados semelhantes em clusters ou grupos. O objetivo é encontrar padrões ou estruturas nos dados que não são rotulados.

## O que é RAG (Retrieval-Augmented Generation)?

RAG (Retrieval-Augmented Generation) é um modelo de linguagem que combina geração de texto com recuperação de informações. Ele gera previsões baseadas em um modelo de geração de texto e uma base de conhecimento externa, como documentos, páginas da web, ou bancos de dados.

## O que é Prompt Engineering?

Prompt Engineering é uma técnica usada para projetar prompts ou instruções específicas para modelos de linguagem gerarem previsões desejadas. Ele ajuda a controlar o comportamento e a qualidade das previsões geradas por modelos de linguagem.

## Bedrock - Provisioned Throughput vs On-Demand

- **Provisioned Throughput**:
  - Capacidade de leitura/gravação predefinida para tabelas e índices.
  - Ideal para cargas de trabalho previsíveis e consistentes.
  - Custos previsíveis, mas pode ser subutilizado em cargas de trabalho variáveis.
  - Alguns modelos permitem fine-tuning e customização.
- **On-Demand**:
  - Capacidade de leitura/gravação ajustada automaticamente com base no uso.
  - Ideal para cargas de trabalho variáveis e imprevisíveis.
  - Custos variáveis, mas otimizados para cargas de trabalho dinâmicas.

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

## Amazon Connect

Amazon Connect é um serviço de central de atendimento na nuvem que permite criar e gerenciar centrais de atendimento virtuais de forma escalável e flexível. Ele oferece recursos de voz, chat e integração com IA para melhorar a experiência do cliente.

## O que é AutoML?

AutoML (Automated Machine Learning) é um conjunto de técnicas e ferramentas que automatizam o processo de construção, treinamento e ajuste de modelos de Machine Learning. Ele ajuda a acelerar o desenvolvimento de modelos e reduzir a necessidade de conhecimento especializado.

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

## Amazon Titan

É o FM da AWS, que é um modelo de linguagem de grande escala treinado em 1 trilhão de parâmetros. Ele é usado para tarefas de NLP, como tradução, resumo, geração de texto, classificação de texto, entre outros.

## PEFT (Parameter-Efficient Fine-Tuning) vs Full Fine-Tuning

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

## Princípios de Responsible AI na AWS

A AWS adota princípios fundamentais para o desenvolvimento responsável da IA:

- Justiça (Fairness) – Evita vieses indesejados nos modelos de IA.
- Explicabilidade (Explainability) – Fornece transparência nos resultados dos modelos.
- Privacidade & Segurança (Privacy & Security) – Protege dados e garante conformidade regulatória.
- Robustez & Confiabilidade (Robustness & Reliability) – Garante modelos resilientes e de alto desempenho.
- Governança (Governance) – Estabelece controles para monitoramento contínuo e conformidade.

## SageMaker Inference options

- Real-Time Inference: Immediate responses for high-traffic, low-latency applications.
- Asynchronous Inference: Near real-time for large payloads and longer processing.
- Batch Transform: Large-scale, offline processing without real-time needs.
- Serverless Inference: Low-latency inference for intermittent or unpredictable traffic without managing infrastructure.
