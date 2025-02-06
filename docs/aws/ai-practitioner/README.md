<!-- BEGIN_DOCS -->
<div align="center">
<a name="readme-top"></a>
</div>

- [Visão Geral](#Visão%20Geral)
	- [Contexto](##Contexto)
	- [Disclaimer](##Disclaimer)
- [Sobre](#Sobre)
- [Estrutura do Exame](#Estrutura%20do%20Exame)
- [Domínios de Conhecimento](#Domínios%20de%20Conhecimento)
	- [Fundamentos de IA e ML](##Fundamentos%20de%20IA%20e%20ML)
	- [Fundamentos de IA generativa](##Fundamentos%20de%20IA%20generativa)
	- [Aplicações de modelos de base](##Aplicações%20de%20modelos%20de%20base)
	- [Diretrizes de IA responsável](##Diretrizes%20de%20IA%20responsável)
	- [Segurança, conformidade e governança para soluções de IA](##Segurança,%20conformidade%20e%20governança%20para%20soluções%20de%20IA)
- [Dicas](#Dicas)
- [Referências](#Referências)
- [Conclusão](#Conclusão)

# Visão Geral

## Contexto

Fala pessoal! Sejam muito bem-vindos 👋.

Hoje, irei compartilhar com vocês meu guia de estudos para a certificação **AWS Certified AI Practitioner** (**AIF-C01**). Minha ideia é criar uma base de conhecimento com informações essenciais sobre o exame, como: estrutura, domínios, dicas e links. Todas essas informações irão te ajudar a se preparar para a prova e aumentar suas chances de conquistar a certificação.

Vamos começar essa jornada de aprendizado? 🚀

## Disclaimer

> [!NOTE]
> Segundo um estudo da AWS realizado no final de 2023, os empregadores estão dispostos a pagar 43% a mais para contratar trabalhadores qualificados em IA para vendas e marketing, 42% a mais para aqueles na área de finanças, 41% a mais para operações comerciais e 47% a mais para profissionais de TI.

# Sobre

A certificação **AWS Certified AI Practitioner** é uma prova introdutório que vai validar seus conceitos básicos sobre inteligência artificial (IA), machine learning (ML) e IA generativa na AWS. Por esse tema estar em ampla assenção, a certificação é uma ótima oportunidade para profissionais que desejam ingressar na área de IA e ML, ou que já trabalham na área de tecnologia e desejam expandir seus conhecimentos.

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

# Estrutura do Exame

A prova contém perguntas dos seguintes tipos:

- **Múltipla escolha**: uma ou mais respostas corretas.
- **Múltipla resposta**: duas ou mais respostas corretas.
- **Ordenaçã**: ordene as opções em uma sequência correta.
- **Correspondência**: corresponda as opções de uma coluna com as da outra.
- **Estudos de caso**: cenários com perguntas relacionadas.

Além disso, temos:

- Perguntas não respondidas não são pontuadas, então é importante responder todas as questões.
- Não há penalidade por tentar adivinhar.
- O exame inclui 50 perguntas que podem afetar sua pontuação. Ou seja, 15 perguntas não são avaliadas e não afetam sua pontuação.

# Domínios de Conhecimento

O exame tem os seguintes domínios:

## Fundamentos de IA e ML

Corresponde a 20% das questões do exame e aborda os seguintes tópicos:

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

Aproximadamente 10 pontuadas e 3 não pontuadas.

## Fundamentos de IA generativa

Corresponde a 24% das questões do exame e aborda os seguintes tópicos:

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

Aproximadamente 12 pontuadas e 4 não pontuadas.

## Aplicações de modelos de base

Corresponde a 28% das questões do exame e aborda os seguintes tópicos:

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

Aproximadamente 14 pontuadas e 4 não pontuadas.

## Diretrizes de IA responsável

Corresponde a 14% das questões do exame e aborda os seguintes tópicos:

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

Aproximadamente 7 pontuadas e 2 não pontuadas.

## Segurança, conformidade e governança para soluções de IA

Corresponde a 14% das questões do exame e aborda os seguintes tópicos:

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

Aproximadamente 7 pontuadas e 2 não pontuadas.

# Dicas

- **Planejamento:**
  - Estabeleça um cronograma de estudo dividido entre os domínios principais.
  - Dedique sessões de estudo para revisões teóricas e práticas.
- **Estude os Domínios:**
  - Entenda os tópicos de cada domínio e foque nos que você tem menos conhecimento.
- **Pratique com Questões de Exames Anteriores:**
  - Faça simulados para se acostumar com o estilo das perguntas.
- **Foque nos Domínios com Maior Peso:**
  - Priorize os tópicos que têm mais questões no exame.
- **Revise os Conceitos Fundamentais:**
  - Entenda os conceitos básicos de IA e ML.
- **Leia a Documentação Oficial:**
  - A AWS conta com uma documentação rica e detalhada sobre os serviços de IA.
- **Utilize o AWS Skill Builder:**
  - Explore e pratique com o AWS Skill Builder, que oferece cenários reais e exercícios práticos para reforçar seu aprendizado.

# Referências

Links úteis para sua preparação:

- [AWS Certified AI Practitioner](https://aws.amazon.com/certification/certified-ai-practitioner/)
- [AWS Training and Certification](https://aws.amazon.com/training/)
- [AWS Documentation](https://docs.aws.amazon.com/)
- [AWS Developer Forums](https://forums.aws.amazon.com/)
- [Stack Overflow - AWS Tag](https://stackoverflow.com/questions/tagged/aws)

# Conclusão

Espero que esse guia tenha te ajudado a entender melhor o exame **AWS Certified AI Practitioner** e a se preparar para a prova. Lembre-se de que a prática é essencial para fixar o conteúdo e aumentar suas chances de sucesso. **Boa sorte e bons estudos!** 👩🏻‍💻📓✍🏻💡

<p align="right">(<a href="#readme-top">back to top</a>)</p>
<!-- END_DOCS -->
