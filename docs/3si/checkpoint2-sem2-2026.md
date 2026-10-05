# Microservices and Web Engineering

## Check Point 2 — 2º semestre/2026
**Prof. Antonio Carlos de Lima Júnior**

## Instruções Gerais

- Atividade a ser desenvolvida em **grupos de até 2 pessoas**.
- Cada integrante deverá possuir o projeto em seu próprio repositório.
- A entrega deverá ser realizada **apenas por um representante do grupo**.
- O projeto deverá atender ao requisito descrito abaixo.
- **Valor total: 10 pontos.**

---

# Requisito

Criar uma **API REST em Java utilizando Spring Boot**, com acesso a um **banco de dados SQL Server remoto**.

A aplicação deverá ser capaz de realizar operações sobre os dados armazenados no banco remoto por meio de endpoints da API.

> **Restrição:** não poderá ser utilizado o projeto `study-apir`.

---

# Critérios de Avaliação

## 1. API Java com Spring Boot — 3,0 pontos

A aplicação deverá ser desenvolvida utilizando **Java e Spring Boot** e disponibilizar uma API REST funcional.

| Critério | Pontuação |
|---|---:|
| Projeto desenvolvido em Java com Spring Boot | 1,0 |
| API REST implementada corretamente | 1,0 |
| Endpoints funcionando corretamente | 1,0 |

---

## 2. Conexão com SQL Server remoto — 4,0 pontos

A API deverá acessar um **SQL Server remoto/local**

| Critério | Pontuação |
|---|---:|
| Configuração de conexão com SQL Server | 1,0 |
| Conexão realizada com banco SQL Server  | 1,5 |
| Consulta/gravação de dados no banco por meio da API | 1,0 |
| Aplicação funciona utilizando o banco remoto disponibilizado | 0,5 |

Durante a correção, será verificado se a aplicação realmente realiza operações no SQL Server remoto.

---

## 3. Persistência e operações sobre os dados — 2,0 pontos

A API deverá utilizar uma camada de persistência para acessar os dados armazenados no SQL Server.

| Critério | Pontuação |
|---|---:|
| Utilização adequada de mecanismo de persistência, como Spring Data JPA | 0,5 |
| Entidades/modelos correspondentes às tabelas utilizadas | 0,5 |
| Operação de consulta dos dados | 0,5 |
| Operação de inserção, alteração ou exclusão dos dados | 0,5 |

---

## 4. Organização e demonstração do projeto — 1,0 ponto

| Critério | Pontuação |
|---|---:|
| Organização adequada do projeto | 0,5 |
| README contendo instruções para executar e testar a API | 0,5 |

O README deverá informar, no mínimo:

- como executar a aplicação;
- como configurar a conexão com o SQL Server;
- quais endpoints podem ser utilizados para testar a API;
- informações necessárias para realizar a conexão com o banco, quando aplicável.

---

# Resumo da Pontuação

| Item | Pontuação |
|---|---:|
| 1. API Java com Spring Boot | **3,0** |
| 2. Conexão com SQL Server  | **4,0** |
| 3. Persistência e operações sobre os dados | **2,0** |
| 4. Organização e demonstração | **1,0** |
| **Total** | **10,0 pontos** |

---

# Instruções de Entrega

## GitHub

O projeto deverá ser disponibilizado em um repositório no GitHub.

O código enviado deverá corresponder à versão apresentada durante a avaliação.

## Portal do Aluno / Área de Entrega de Trabalhos

Enviar um único arquivo `.txt` contendo:

- URL do repositório no GitHub;
- nome completo e RM dos integrantes do grupo.

A entrega deverá ser realizada **por apenas um representante do grupo**.

---

