# **Maratona FullCycle**

## Visão macro do projeto

- Autenticação entre micro-serviços
  - keycloak
  - OpenID connect
- Entrega da aplicação
  - Git
  - Config do CI- Integração continua
  - Config do CD - Entrega continua
- APM (application performance monitor)
  - observalidade
  - metricas
  - logs

---

## O que é FullCycle?

Dev que tem a capacidade de:

arquitetar,
desenvolver,
testar,
deployar,
monitorar,
dar suporte ao microsserviços.

---
## 3 pilares

1. operate what you build ("operar o que você constroi")
2. Ferramentas para escalar
3. FullCycle dev
---
## Diferença entre FullCycle e FullStack

- FullStack

  habilidades de desenvolvimento > backend > frontend > mobile

- FullCylcle

  habilidade de desenvolvimento > arquitetar > testar> deployar > monitorada
---
## Microsserviços?

1. Disponibiliza informação.
2. Realiza transações.
3. Resolve problemas de negocio.
   independente de tecnologia ou protocolo.
4. Pode estabelecer comunicação com diversos clientes "dependências".
---
## O que usaremos no estudo de caso?

- Teremos 3 aplicações independentes. Backend, SPA e Auth server.

- cada aplicação é executada em servidores diferentes, serão monitoradas de forma independentes outras aplicações ou até mesmo microsserviços podem ser adicionados
Backend e frontend possuem muita responsabilidade.
---
## Estudo de caso\*\*

    - Plataforma de comunicação em tempo real parecida com o discord ou slack.
    - o sistema está dividido em 3 partes: backend, frontend com spa e um servidor de autenticação
    - o usuário poderá se registrar. No momento do registro, a conta será criada no servidor de autenticação
    - o usuário poderá realizar o login no servidor de autenticação e receber os tokens de acesso
    - apos o login, o usuário poderá criar um novo servidor
    - Dentro de um servidor o usuário tembém poderá criar categorias, bem como os canais de comunicação
    - o usuário também poderá gerar um convite para que outros usuários acessem seu servidor
    - os usuários poderão se comunicar em tempo real
---
## Tecnologias utilizadas

- Autenticação

  OAuth 2
  openId Connection
  Keycloack

- Backend

  TypeScript
  Nest.js
  loopback
  Elasticsearch
  kibana

- SPA (single page application)

  TypeScript
  React.js
  Websockets

- Controle de versão CI/CD

  github
  politicas de acesso aos branches
  code owner
  code Review
  integração continua / google cloud build
  kubernetes no gke
  autoscaling com hpa

- Observabilidade

  elasticsearch
  filebeat
  metrics
  apm server
