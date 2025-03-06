# Zero Shot

- O runtime do OCI é runC
- O container é um processo isolado

# Questions

## Stateless vs Stateful

- **Stateless**:
  - Não armazena informações sobre o estado da sessão do cliente entre requisições. Cada requisição é tratada como independente.
  - Características:
    - Sem persistência de estado: O servidor não guarda dados do cliente após a resposta.
    - Escalabilidade fácil: Pode ser replicada horizontalmente sem problemas.
  - Exemplos: APIs RESTful, servidores HTTP básicos, microsserviços que usam tokens (JWT).
- **Stateful**:
  - Armazena estado entre execuções.

## O que são SIGs (Special Interest Groups)

- **SIGs**:
  - Grupos de interesse especializados dentro da comunidade Kubernetes.
  - Função:
    - Desenvolvimento de recursos específicos.
    - Comunicação e colaboração entre membros.
  - Exemplos: SIG Apps, SIG CLI, SIG Storage.

## Which approach exposes cluster credentials outside the cluster, potentially posing security risks?

Push Based Deployment Approach

## In Kubernetes, when considering network policies within a namespace, what is the default behavior regarding ingress and egress traffic to and from pods if no policies are defined?

All ingress and egress traffic is allowed to and from pods in the namespace.

# What native runtime is Open Container Initiative (OCI) compliant?

A **runtimes nativas compatíveis com a OCI (Open Container Initiative)** são:

### **`runc`**

- **É a principal runtime de containers compatível com a OCI**.
- **Padrão de fato** para execução de containers, usado por ferramentas como Docker, containerd e CRI-O.
- Implementa as especificações OCI:
  - **image-spec** (formato de imagem).
  - **runtime-spec** (execução do container).

### **Outras runtimes OCI-compliant (usam `runc` internamente):**

- **containerd** (usado pelo Docker e Kubernetes via CRI).
- **CRI-O** (otimizada para Kubernetes).
