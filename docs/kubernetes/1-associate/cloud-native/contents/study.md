# Kubernetes Architecture

- Nodes:
  - Master Nodes: Responsáveis pelo controle do cluster. Gerenciam a orquestração dos workloads.
  - Worker Nodes: Executam os containers das aplicações.
- Componentes - Master Node:
  - API Server: Ponto central de comunicação do cluster. Todos os componentes interagem com ele via API REST.
  - ETCD: Banco de dados chave-valor que armazena o estado do cluster.
  - Scheduler: Decide em qual nó um novo pod será executado, baseado em recursos e restrições.
  - Controller Manager: Gerencia controladores responsáveis por manter o estado desejado do cluster (ex: ReplicaSet, Node Controller, etc.).
- Componenets - Worker Node:
  - Container Runtime: Executa os containers (ex: containerd, CRI-O, RKT, Docker).
  - Kubelet: Agente que roda em cada nó, garantindo que os containers estejam rodando conforme especificado.

# CRI

- Interface que permite ao Kubernetes interagir com diferentes container runtimes sem mudanças no código do Kubernetes.
- Define um protocolo padrão usado pelo Kubelet para gerenciar containers.
- Suporta operações como:
  - Gerenciamento de imagens (pull, list, remove).
  - Criação e remoção de containers.
  - Gerenciamento de rede (via CNI - Container Network Interface).
- Principais runtimes compatíveis com CRI:
  - containerd (padrão do Kubernetes).
  - CRI-O (otimizado para Kubernetes).
  - RKT (descontinuado).
  - Docker (suportado via dockershim, mas oficialmente removido no Kubernetes 1.24).

# Networking

- Quais os tipos de Service no Kubernetes?
  - ClusterIP (padrão, comunicação interna).
  - NodePort (exposição externa via porta fixa).
  - LoadBalancer (integra com balanceadores de carga externos).
  - ExternalName (mapeia um nome DNS externo).
