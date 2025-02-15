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
