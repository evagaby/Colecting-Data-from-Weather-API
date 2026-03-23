# 🌦️ Colecting Data from Weather API

## 📌 Descrição

Este projeto implementa um pipeline de ingestão de dados meteorológicos utilizando Python. A aplicação realiza a coleta de dados a partir de uma API de clima, processa as informações em formato JSON e armazena os dados tratados em um banco de dados relacional (SQL Server).

O foco do projeto é demonstrar habilidades fundamentais de engenharia de dados, como consumo de APIs, transformação de dados semi-estruturados e persistência em banco de dados.

---

## 🎯 Objetivo

Construir um fluxo de dados capaz de:

* Consumir dados de uma API meteorológica
* Tratar e padronizar os dados recebidos (JSON)
* Armazenar os dados em um banco SQL Server
* Garantir maior robustez com tratamento de erros

---

## 🛠️ Tecnologias Utilizadas

* Python
* Requests (consumo de API)
* SQL Server
* PyODBC / Conexão com banco
* JSON

---

## ⚙️ Como funciona

1. A aplicação realiza uma requisição HTTP para a API de clima
2. Os dados retornados (JSON) são extraídos e tratados
3. Informações relevantes como:

   * Cidade
   * Estado
   * Temperatura
   * Sensação térmica
   * Umidade

   são selecionadas e padronizadas
4. Os dados são inseridos em uma tabela no SQL Server

---
## 🧱 Estrutura do Projeto
├── script_api  # Script responsável pela coleta, tratamento e carga dos dados
└── README.md

## 🗄️ Estrutura dos Dados

Os dados armazenados seguem o seguinte modelo:

| Campo            | Descrição         |
| ---------------- | ----------------- |
| cidade           | Nome da cidade    |
| estado           | Estado            |
| temperatura      | Temperatura atual |
| sensacao_termica | Sensação térmica  |
| umidade          | Umidade do ar     |

---

## ⚠️ Tratamento de Erros

O projeto considera possíveis falhas durante a execução, como:

* Erros na requisição da API
* Dados incompletos ou inconsistentes
* Falhas na conexão com o banco

Esses cenários são tratados para evitar interrupções no fluxo de dados.

---

## 🚀 Possíveis melhorias

* Implementação de orquestração de pipelines
* Armazenamento de logs de execução
* Versionamento dos dados
* Criação de dashboards para visualização
* Deploy em ambiente cloud

---

## 📚 Aprendizados

Este projeto permitiu aplicar na prática conceitos como:

* Consumo de APIs REST
* Manipulação de dados JSON
* Integração com banco de dados relacional
* Estruturação de pipelines de dados
* Boas práticas em organização de código

---

## 👩‍💻 Autora

Projeto desenvolvido por **Eva Gabriela** como parte dos estudos em Engenharia de Dados.
