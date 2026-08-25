# Microservices and Web Engineering

## Check Point 1 — 2º semestre/2026  
**Prof. Antonio Carlos de Lima Júnior**

## Instruções Gerais

- Atividade a ser desenvolvida em **grupos de até 2 pessoas**.
- Cada integrante deverá possuir o projeto em seu próprio repositório.
- A entrega deverá ser realizada **apenas por um representante do grupo**.
- Observe o projeto proposto e cumpra todos os requisitos descritos abaixo.
- **Valor total: 10 pontos.**

---

# Projeto

Criar ou utilizar uma aplicação existente em **Java com Spring Boot**, que possua:

- API REST;
- acesso a banco de dados;
- documentação Swagger/OpenAPI;
- configuração por profiles;
- empacotamento e execução utilizando Docker.

> **Restrição:** não poderá ser utilizado o projeto `study-apir`.

---

# Atividades e Critérios de Avaliação

## 1. Aplicação e configuração dos Profiles — 2,0 pontos

A aplicação deverá possuir pelo menos dois profiles de execução:

- `default`;
- `prd`.

### Critérios

| Critério | Pontuação |
|---|---:|
| Aplicação Spring Boot executando corretamente | 0,5 |
| Configuração do profile padrão | 0,5 |
| Configuração específica para o profile `prd` | 0,5 |
| No profile `prd`, o banco de dados e suas tabelas não podem ser criados automaticamente pela aplicação | 0,5 |

---

## 2. Criação do Dockerfile — 2,0 pontos

Criar um `Dockerfile` capaz de gerar uma imagem Docker da aplicação.

### Requisitos

- utilizar uma imagem Java adequada;
- copiar corretamente o artefato da aplicação;
- configurar a inicialização da aplicação;
- disponibilizar a porta **8080**;
- permitir a utilização do profile `prd`.

### Critérios

| Critério | Pontuação |
|---|---:|
| Dockerfile válido e organizado | 0,5 |
| Build da imagem executado com sucesso | 0,5 |
| Container inicia e disponibiliza a aplicação na porta 8080 | 0,5 |
| Possibilidade de selecionar o profile `prd` durante a execução | 0,5 |

---

## 3. Publicação no Docker Hub — 2,0 pontos

Publicar a imagem criada em um repositório no **Docker Hub**.

O repositório deverá possuir o **mesmo nome utilizado no GitHub**.

### Critérios

| Critério | Pontuação |
|---|---:|
| Repositório criado no Docker Hub | 0,5 |
| Imagem publicada corretamente | 0,5 |
| Imagem pode ser baixada utilizando `docker pull` | 0,5 |
| Imagem publicada pode ser executada corretamente | 0,5 |

> A imagem será considerada válida somente se puder ser baixada e executada durante a correção.

---

## 4. Documentação do projeto — 3,0 pontos

O arquivo `README.md` do GitHub deverá conter todas as instruções necessárias para execução da aplicação a partir da imagem publicada no Docker Hub.

### Critérios

| Critério | Pontuação |
|---|---:|
| Instruções para download da imagem Docker | 0,5 |
| Comando de execução utilizando `docker run` | 1,0 |
| Documentação das variáveis de ambiente necessárias | 0,5 |
| Instruções para acesso ao Swagger/OpenAPI | 0,5 |
| Clareza e organização geral da documentação | 0,5 |

O comando de execução deverá contemplar:

- mapeamento da porta 8080;
- configuração do profile;
- variáveis de ambiente necessárias para execução da aplicação.

---

## 5. Organização e reprodutibilidade da entrega — 1,0 ponto

Será avaliada a capacidade de reproduzir a solução utilizando apenas os recursos e instruções disponibilizados pelo grupo.

### Critérios

| Critério | Pontuação |
|---|---:|
| GitHub e Docker Hub possuem o mesmo nome de repositório | 0,25 |
| Código disponibilizado no GitHub corresponde à aplicação publicada | 0,25 |
| Projeto pode ser executado seguindo exclusivamente o README | 0,25 |
| Repositórios e links entregues estão acessíveis | 0,25 |

---

# Resumo da Pontuação

| Item | Pontuação |
|---|---:|
| 1. Aplicação e Profiles | **2,0** |
| 2. Dockerfile | **2,0** |
| 3. Docker Hub | **2,0** |
| 4. Documentação / README | **3,0** |
| 5. Organização e reprodutibilidade | **1,0** |
| **Total** | **10,0 pontos** |

---

# Instruções de Entrega

## a. GitHub e Docker Hub

- O repositório no GitHub e o repositório no Docker Hub deverão possuir **o mesmo nome**.
- O código disponível no GitHub deverá corresponder à versão utilizada para geração da imagem publicada no Docker Hub.

## b. Portal do Aluno / Área de Entrega de Trabalhos

Enviar um único arquivo `.txt` contendo:

- URL do repositório no GitHub;
- URL do repositório no Docker Hub;
- nome completo e RM dos integrantes do grupo.

A entrega deverá ser realizada **por apenas um representante do grupo**.

---

# Regras para Correção

- Ausência do Dockerfile implica **zero no item 2**.
- Ausência da imagem no Docker Hub implica **zero no item 3**.
- Imagem publicada que não puder ser executada perderá a pontuação correspondente à execução.
- Aplicação que criar automaticamente banco de dados ou tabelas no profile `prd` perderá a pontuação correspondente a esse requisito.
- Ausência das instruções de execução via `docker run` perderá a pontuação correspondente na documentação.
- Swagger/OpenAPI inacessível ou não documentado perderá a pontuação correspondente.
- Links inválidos, privados ou inacessíveis poderão impedir a avaliação dos respectivos critérios.
