<!-- BEGIN_DOCS -->

[◀ Voltar](../../README.md)

<div align="center">

<a name="readme-top"></a>

<img src="https://github.com/lpsm-dev/lpsm-dev/blob/86bb739f86b7cbd57740ba65adfdad6ec2b8641d/.github/assets/kcna.png" width="200"/>

## Guia de Estudos

</div>

# Sumário

<details>
  <summary><strong>Expandir</strong></summary>

- [Visão Geral](#visão-geral)
  - [Contexto](#contexto)
  - [Disclaimer](#disclaimer)
- [Exame](#exame)
  - [Sobre](#sobre)
  - [Estrutura](#estrutura)
- [Domínios de Conhecimento](#domínios-de-conhecimento)
  - [1 - Fundamentos do Kubernetes](#1---fundamentos-do-kubernetes)
  - [2 - Orquestração de Containers](#2---orquestração-de-containers)
  - [3 - Arquitetura Cloud-Native](#3---arquitetura-cloud-native)
  - [4 - Rede no Kubernetes](#4---rede-no-kubernetes)
  - [5 - Observabilidade e Monitoramento](#5---observabilidade-e-monitoramento)
  - [6 - Segurança e Conformidade](#6---segurança-e-conformidade)
  - [7 - Troubleshooting](#7---troubleshooting)
- [Tips & Tricks](#tips--tricks)
  - [Exame](#exame-1)
  - [Estudo](#estudo)
- [Referências](#referências)
- [Conclusão](#conclusão)

</details>

# Visão Geral

## Contexto

Olá, Dev! 👋
Este guia é focado na certificação **Kubernetes Associate Cloud Native (KCNA)**, que valida conhecimentos em Kubernetes e ecossistema cloud-native. Você aprenderá:

- Conceitos fundamentais do Kubernetes,
- Arquitetura cloud-native,
- Melhores práticas para operação e segurança,
- Ferramentas essenciais do ecossistema.

> [!NOTE]
> Profissionais com certificação Kubernetes têm alta demanda no mercado, com salários até **40% maiores** (Fonte: CNCF, 2023).

## Disclaimer

> [!WARNING]
> Este guia não substitui cursos práticos ou mão na massa. Use-o como roteiro complementar.

<p align="right">(<a href="#readme-top">voltar ao topo</a>)</p>

# Exame

## Sobre

| Detalhes           | Informações                                 |
| ------------------ | ------------------------------------------- |
| **Pré-requisitos** | Conhecimento básico em containers e Linux   |
| **Nível**          | Associado                                   |
| **Duração**        | 90 minutos                                  |
| **Custo**          | US$ 250                                     |
| **Formato**        | Online, múltipla escolha e respostas curtas |
| **Nota de Corte**  | 70%                                         |

## Estrutura

- **Tipos de Questões**:
  - Múltipla escolha (única resposta),
  - Múltipla resposta,
  - Associação de colunas,
  - Ordenação de passos.

<p align="right">(<a href="#readme-top">voltar ao topo</a>)</p>

# Domínios de Conhecimento

## 1 - Fundamentos do Kubernetes (25%)

**Conceitos Essenciais**:

- Arquitetura do Kubernetes: Control Plane (API Server, etcd, Scheduler), Worker Nodes (kubelet, kube-proxy).
- Objetos do Kubernetes: Pods, Deployments, Services, Namespaces.
- Comandos básicos do `kubectl` (get, describe, logs, exec).

**Casos de Uso**:

- Diferença entre ReplicaSet e Deployment.
- Gerenciamento de ciclos de vida de aplicações.

> [!NOTE]
> Foco em entender como o Kubernetes gerencia recursos e estados.

## 2 - Orquestração de Containers (20%)

**Tópicos**:

- Criação e gerenciamento de Pods.
- ConfigMaps e Secrets para gerenciamento de configurações.
- Jobs e CronJobs para tarefas em lote.
- Rolling Updates e Rollbacks em Deployments.

**Ferramentas**:

- Helm para gerenciamento de pacotes.
- Kustomize para personalização de manifests.

## 3 - Arquitetura Cloud-Native (15%)

**Princípios**:

- Microsserviços vs Monolitos.
- Service Mesh (Istio, Linkerd).
- CI/CD em ambientes Kubernetes (Argo CD, Tekton).

**Padrões**:

- Sidecar, Adapter, Ambassador.
- Autoscaling (Horizontal Pod Autoscaler).

## 4 - Rede no Kubernetes (15%)

**Conceitos**:

- Service Types: ClusterIP, NodePort, LoadBalancer.
- Ingress Controllers (Nginx, Traefik).
- Network Policies para segurança.

**Ferramentas**:

- CoreDNS para resolução interna.
- CNI plugins (Calico, Flannel).

## 5 - Observabilidade e Monitoramento (10%)

**Tópicos**:

- Coleta de logs com Fluentd ou Loki.
- Monitoramento com Prometheus e Grafana.
- Métricas de recursos (CPU, memória) com Metrics Server.

**Práticas**:

- Configuração de Liveness e Readiness Probes.

## 6 - Segurança e Conformidade (10%)

**Foco**:

- RBAC (Role-Based Access Control).
- SecurityContext em Pods.
- Gerenciamento de Secrets (criptografia, Vault integration).
- Políticas de segurança com OPA Gatekeeper.

## 7 - Troubleshooting (5%)

**Cenários Comuns**:

- Pods em estado `Pending` ou `CrashLoopBackOff`.
- Problemas de rede entre serviços.
- Falhas de scheduling de recursos.

**Ferramentas**:

- `kubectl describe` e `kubectl logs`.
- Debugging com `kubectl debug`.

<p align="right">(<a href="#readme-top">voltar ao topo</a>)</p>

# Tips & Tricks

## Exame

- **Gestão de Tempo**: Reserve 1 minuto por questão; deixe as complexas para o final.
- **Comandos `kubectl`**: Pratique autocompletar e alias (ex: `alias k=kubectl`).
- **YAML**: Entenda a estrutura básica (apiVersion, kind, metadata, spec).

## Estudo

- **Ambiente Prático**: Use [Kind](https://kind.sigs.k8s.io/) ou [Minikube](https://minikube.sigs.k8s.io/) para criar clusters locais.
- **Simulados**: Faça exames práticos no [Killer.sh](https://killer.sh/).
- **Documentação Oficial**: Consulte sempre a [Kubernetes Docs](https://kubernetes.io/docs/).

# Referências

- [Documentação Oficial do Kubernetes](https://kubernetes.io/docs/)
- [Curso KCNA da Linux Foundation](https://training.linuxfoundation.org/)
- [Livro: "Kubernetes Up & Running"](https://www.oreilly.com/library/view/kubernetes-up-and/9781098110192/)

# Conclusão

A jornada para dominar o Kubernetes é desafiadora, mas recompensadora! 🚀
Foque em praticar diariamente, explore cenários reais e participe de comunidades (ex: [CNCF Slack](https://community.cncf.io/)). **Boa sorte!**

<p align="right">(<a href="#readme-top">voltar ao topo</a>)</p>

<!-- END_DOCS -->
