<!-- BEGIN_DOCS -->
<div align="center">
  
<a name="readme-top"></a>

<img src="https://github.com/lpsm-dev/lpsm-dev/blob/41c8e670d12ddffcea19a04c0a7ac3cdd3c929f7/.github/assets/ai-practitioner.png" width="350"/>

## Guia de Estudos

</div>

# Sumário

<details>
  <summary><strong>Expandir</strong></summary>

- [Visão Geral](#Visão%20Geral)
	- [Contexto](##Contexto)
	- [Disclaimer](##Disclaimer)
- [Sobre](#Sobre)
- [Estrutura do Exame](#Estrutura%20do%20Exame)
- [Domínios de Conhecimento](#Domínios%20de%20Conhecimento)
	- [1 - Fundamentos de IA e ML](##1%20-%20Fundamentos%20de%20IA%20e%20ML)
	- [2 - Fundamentos de IA generativa](##2%20-%20Fundamentos%20de%20IA%20generativa)
	- [3 - Aplicações de modelos de base](##3%20-%20Aplicações%20de%20modelos%20de%20base)
	- [4 - Diretrizes de IA responsável](##4%20-%20Diretrizes%20de%20IA%20responsável)
	- [5 - Segurança, conformidade e governança para soluções de IA](##5%20-%20Segurança,%20conformidade%20e%20governança%20para%20soluções%20de%20IA)
- [Dicas](#Dicas)
- [Prompts](#Prompts)
- [Referências](#Referências)
- [Conclusão](#Conclusão)

<p align="right">(<a href="#readme-top">back to top</a>)</p>

</details>

# Visão Geral

## Contexto

Fala pessoal! Sejam muito bem-vindos 👋.

Hoje, irei compartilhar com vocês meu guia de estudos para a certificação **AWS Certified AI Practitioner** (**AIF-C01**). Minha ideia é criar uma base de conhecimento com informações essenciais sobre o exame, como: 

- estrutura,
- domínios,
- dicas,
- links e muito mais.

Todas essas informações irão te ajudar a se preparar para a prova e aumentar suas chances de conquistar essa tão sonhada certificação.

Vamos começar essa jornada de aprendizado? 🚀

> [!NOTE]
> Segundo um estudo da AWS realizado no final de 2023, os empregadores estão dispostos a pagar 43% a mais para contratar trabalhadores qualificados em IA para vendas e marketing, 42% a mais para aqueles na área de finanças, 41% a mais para operações comerciais e 47% a mais para profissionais de TI.

## Disclaimer

> [!WARNING]
> Essa documentação não substitui um curso ou simulado. Olhe para ela como um complemento + guia inicial.

<p align="right">(<a href="#readme-top">back to top</a>)</p>

# Sobre

A certificação **AWS Certified AI Practitioner** é uma prova introdutória que vai validar seus conceitos básicos sobre inteligência artificial (IA), machine learning (ML) e IA generativa (Gen AI) na AWS. 

Por esse tema estar em ampla assenção, essa certificação é uma ótima oportunidade para profissionais que desejam ingressar na área de IA e ML, ou que já trabalham na área de tecnologia e desejam expandir seus conhecimentos sobre esse tema.

| Detalhes       | Informações                                 |
| -------------- | ------------------------------------------- |
| Pré-requisitos | Nenhum                                      |
| Nível          | Fundamental                                 |
| Validade       | 3 anos                                      |
| Nota de Corte  | 700/1000 pontos                             |
| Questões       | 65 questões                                 |
| Idiomas        | Coreano, Português, Inglês, Japonês, Chinês |
| Custo          | 100 USD                                     |
| Duração        | 150 minutos                                 |

<p align="right">(<a href="#readme-top">back to top</a>)</p>

# Estrutura do Exame

A prova contém perguntas dos seguintes tipos:

- **Múltipla escolha**: uma ou mais respostas corretas.
- **Múltipla resposta**: duas ou mais respostas corretas.
- **Ordenaçã**: ordene as opções em uma sequência correta.
- **Correspondência**: corresponda as opções de uma coluna com as da outra.
- **Estudos de caso**: cenários com perguntas relacionadas.

<p align="right">(<a href="#readme-top">back to top</a>)</p>

# Domínios de Conhecimento

O exame tem os seguintes domínios:

## 1 - Fundamentos de IA e ML

Corresponde a 20% das questões e aborda os seguintes tópicos:

- **Conceitos e terminologias básicas de IA**:
  - Definição de termos como IA, ML, aprendizado profundo, redes neurais, visão computacional, PLN, modelo, algoritmo, treinamento, inferência, viés, imparcialidade, ajuste e LLM.
  - Diferenças entre IA, ML e aprendizado profundo.
  - Tipos de inferência (em lote e em tempo real).
  - Tipos de dados (rotulados, não rotulados, tabulares, séries temporais, imagens, texto, estruturados e não estruturados).
  - Métodos de aprendizado: supervisionado, não supervisionado e por reforço.
- **Casos de uso práticos de IA**:
  - Aplicações onde IA/ML agregam valor (tomada de decisão, escalabilidade, automação).
  - Situações onde IA/ML não são adequadas (análises de custo-benefício, necessidade de resultados específicos).
  - Técnicas de ML para casos de uso (regressão, classificação, agrupamento).
  - Exemplos de aplicações reais: visão computacional, PLN, reconhecimento de fala, sistemas de recomendação, detecção de fraude e previsão.
  - Serviços de IA/ML da AWS (SageMaker, Transcribe, Translate, Comprehend, Lex, Polly).
- **Ciclo de vida do desenvolvimento de ML**:
  - Componentes do pipeline de ML: coleta de dados, análise exploratória (AED), pré-processamento, engenharia de atributos, treinamento, ajuste de hiperparâmetros, avaliação, implantação e monitoramento.
  - Origem dos modelos: pré-treinados (open-source) ou treinamento personalizado.
  - Métodos para usar modelos em produção (serviço de API gerenciado ou auto-hospedado).
  - Serviços AWS para cada estágio do pipeline.
  - Conceitos de MLOps: experimentação, processos repetíveis, escalabilidade, gerenciamento de dívidas técnicas, monitoramento e retreinamento.
  - Métricas de desempenho (acurácia, AUC, F1) e métricas empresariais (custo por usuário, ROI, feedback de clientes).

> [!NOTE]
> Aproximadamente 10 pontuadas e 3 não pontuadas.

## 2 - Fundamentos de IA generativa

Corresponde a 24% das questões e aborda os seguintes tópicos:

- **Conceitos básicos de IA generativa**:
  - Definição de IA generativa e suas aplicações.
  - Diferença entre IA generativa e IA tradicional.
  - Modelos de linguagem grandes (LLMs) e sua arquitetura.
  - Técnicas de geração de conteúdo (texto, imagens, áudio).
- **Casos de uso de IA generativa**:
  - Geração de texto (chatbots, redação automática).
  - Geração de imagens (arte, design).
  - Geração de áudio (síntese de voz, música).
  - Aplicações em marketing, entretenimento e educação.
- **Serviços de IA generativa da AWS**:
  - Amazon Bedrock.
  - Amazon CodeWhisperer.
  - Integração com modelos de terceiros (por exemplo, OpenAI).

> [!NOTE]
> Aproximadamente 12 pontuadas e 4 não pontuadas.

## 3 - Aplicações de modelos de base

Corresponde a 28% das questões e aborda os seguintes tópicos:

- **Conceitos de modelos de base**:
  - Definição de modelos de base (foundation models).
  - Diferença entre modelos de base e modelos personalizados.
  - Aplicações de modelos de base em diversas indústrias.
- **Treinamento e ajuste de modelos de base**:
  - Transfer learning e fine-tuning.
  - Uso de modelos pré-treinados para tarefas específicas.
  - Técnicas de ajuste de modelos para melhorar a precisão.
- **Serviços da AWS para modelos de base**:
  - Amazon SageMaker JumpStart.
  - Amazon Bedrock.
  - Integração com modelos de código aberto (por exemplo, Hugging Face).

> [!NOTE]
> Aproximadamente 14 pontuadas e 4 não pontuadas.

## 4 - Diretrizes de IA responsável

Corresponde a 14% das questões e aborda os seguintes tópicos:

- **Princípios de IA responsável**:
  - Transparência, justiça, privacidade e segurança.
  - Mitigação de viés em modelos de IA.
  - Considerações éticas no desenvolvimento de IA.
- **Práticas recomendadas para IA responsável**:
  - Avaliação de impacto de modelos de IA.
  - Monitoramento de viés e desempenho.
  - Engajamento com stakeholders e comunidades.
- **Ferramentas e serviços da AWS para IA responsável**:
  - Amazon SageMaker Clarify.
  - Amazon Comprehend para análise de viés.
  - AWS AI Ethics Toolkit.

> [!NOTE]
> Aproximadamente 7 pontuadas e 2 não pontuadas.

## 5 - Segurança, conformidade e governança para soluções de IA

Corresponde a 14% das questões e aborda os seguintes tópicos:

- **Segurança em soluções de IA**:
  - Proteção de dados e modelos.
  - Criptografia e controle de acesso.
  - Prevenção de ataques adversariais.
- **Conformidade e governança**:
  - Normas e regulamentações (por exemplo, GDPR, HIPAA).
  - Auditoria e monitoramento de modelos de IA.
  - Gerenciamento de riscos e conformidade contínua.
- **Serviços da AWS para segurança e conformidade**:
  - AWS Identity and Access Management (IAM).
  - AWS Key Management Service (KMS).
  - AWS CloudTrail para auditoria.
  - AWS CloudTrail para auditoria.

> [!NOTE]
> Aproximadamente 7 pontuadas e 2 não pontuadas.

<p align="right">(<a href="#readme-top">back to top</a>)</p>

# Tips & Tricks

> [!NOTE]
> As provas da AWS possuem algumas características e essa não é diferente:
> - Perguntas não respondidas não são pontuadas, então é importante responder todas as questões.
> - Não há penalidade por "tentar adivinhar" a resposta de uma questão.
> - O exame possui perguntas que não afetam sua pontuação. Nesse caso, das 65 questões, 15 não são avaliadas e não afetam sua pontuação (são usadas como banco de questões da AWS em futuras provas).
> - A quem diga que se durante a prova oficial você marcar uma questão para revisão, as próximas questões serão parecidas com ela. Mas cuidado, isso mais me parece um boato kkk. 

No geral, sugiro essas dicas:

- **Planejamento:**
  - Estabeleça um cronograma de estudo dividido entre os domínios principais.
  - Dedique sessões de estudo para revisões teóricas e práticas.
- **Estude os Domínios:**
  - Entenda os tópicos de cada domínio e foque nos que você tem menos conhecimento.
- **Pratique com questões de exames anteriores:**
  - Faça simulados para se acostumar com o estilo das perguntas.
- **Foque nos domínios com maior Peso:**
  - Priorize os tópicos que têm mais questões no exame.
- **Revise os conceitos fundamentais:**
  - Entenda os conceitos básicos de IA e ML.
- **Leia a documentação oficial:**
  - A AWS conta com uma documentação rica e detalhada sobre os serviços de IA.
- **Utilize o AWS Skill Builder:**
  - Explore e pratique com o AWS Skill Builder, que oferece cenários reais e exercícios práticos para reforçar seu aprendizado.

<p align="right">(<a href="#readme-top">back to top</a>)</p>

# Prompts

- Escolha um Provedor de Certificação: Navegue até o diretório correspondente ao provedor (e.g., aws).
- Selecione uma Certificação: Localize o diretório da certificação e nível desejado.
- Copie e Cole o Prompt: Utilize o prompt no modelo de IA escolhido (e.g., ChatGPT, Claude).
- Simulação Interativa: Responda às perguntas e receba feedback em tempo real com explicações detalhadas.
- Revisão com Flashcards: Opcionalmente, revise conceitos importantes usando flashcards baseados nas perguntas respondidas.

Para mais informações, acesse o arquivo de [prompt](prompt.md).

<p align="right">(<a href="#readme-top">back to top</a>)</p>

# Referências

Links úteis para sua preparação:

- [Página oficial AWS Certified AI Practitioner](https://aws.amazon.com/pt/certification/certified-ai-practitioner/)
- [Exam Guide](https://d1.awsstatic.com/pt_BR/training-and-certification/docs-ai-practitioner/AWS-Certified-AI-Practitioner_Exam-Guide.pdf)
- [Skill Builder](https://explore.skillbuilder.aws/learn/learning_plan/view/2194/plan)

<p align="right">(<a href="#readme-top">back to top</a>)</p>

# Conclusão

Espero que esse guia tenha te ajudado a entender melhor o exame **AWS Certified AI Practitioner** e a se preparar para a prova. Lembre-se de que a prática é essencial para fixar o conteúdo e aumentar suas chances de sucesso. **Boa sorte e bons estudos!** 👩🏻‍💻📓✍🏻💡

<p align="right">(<a href="#readme-top">back to top</a>)</p>
<!-- END_DOCS -->
