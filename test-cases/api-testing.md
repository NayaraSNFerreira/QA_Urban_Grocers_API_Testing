# 🔌 Testes de API — Urban.Grocers

## 📌 Objetivo

Realizar testes de API no backend da aplicação Urban.Grocers, aplicando técnicas de análise e design de testes para validar as novas funcionalidades relacionadas ao gerenciamento de produtos em kits e ao serviço de entrega Order and Go.

O projeto foi desenvolvido durante minha formação em Quality Assurance (QA) na TripleTen.

---

## 🔎 Escopo

Foram testados os endpoints responsáveis por:

- Adição de produtos a kits;
- Validação do limite de produtos em kits;
- Verificação da disponibilidade do serviço de entrega Order and Go;
- Cálculo do custo de entrega;
- Validação dos parâmetros das requisições.

Foram elaborados e executados **70 casos de teste**, contemplando cenários positivos e negativos, validações de parâmetros, valores-limite, dados inválidos e diferentes condições de entrada.

### Endpoints testados

- `POST /api/v1/kits/:id/products`
- `POST /order-and-go/v1/delivery`

A autorização da API não fez parte do escopo, conforme definido na tarefa.

---

## 🧪 Técnicas de teste

- Testes positivos e negativos;
- Particionamento em classes de equivalência;
- Análise de valores-limite;
- Validação de parâmetros obrigatórios;
- Validação de dados nulos e vazios;
- Validação de formatos e tipos de dados;
- Validação de regras de negócio;
- Validação de códigos de resposta HTTP;
- Testes funcionais de API.

---

## 📋 Abordagem

O trabalho envolveu a análise dos requisitos de backend e da documentação da API, identificação das condições de teste, elaboração dos casos de teste, execução das requisições no Postman e análise dos resultados obtidos.

Foram utilizados diferentes valores de entrada para verificar o comportamento da API em situações válidas e inválidas, incluindo valores nulos, vazios, negativos, tipos de dados incompatíveis, parâmetros ausentes, identificadores inexistentes e diferentes valores de limite.

Também foram verificadas regras específicas das funcionalidades, como o limite de 30 itens por kit e as condições utilizadas para determinar a disponibilidade e o custo do serviço de entrega.

Os resultados foram registrados em checklist, contendo resultado esperado, resultado real e status de cada caso de teste. Os comportamentos divergentes dos requisitos foram documentados e reportados no Jira.

---

## 📊 Resultados

Durante a execução dos **70 casos de teste**, foram identificados **40 comportamentos divergentes do esperado**.

Os problemas encontrados estavam principalmente relacionados a:

- Validação de parâmetros de entrada;
- Tratamento de valores nulos, vazios ou ausentes;
- Validação de tipos de dados;
- Aceitação de valores inválidos;
- Aplicação de regras de negócio;
- Cálculo do custo de entrega;
- Validação da disponibilidade do serviço;
- Retornos HTTP diferentes dos esperados.

Os defeitos identificados foram registrados no Jira durante a execução dos testes.

### Resumo da execução

| Resultado | Quantidade |
| --- | ---: |
| Casos aprovados | 30 |
| Casos com falha | 40 |
| Total | 70 |

---

## 🐞 Principais defeitos identificados

Os defeitos encontrados envolveram principalmente:

- Validação de entrada;
- Valores-limite;
- Formatos e tipos de dados;
- Parâmetros obrigatórios;
- Tratamento de dados inválidos;
- Regras de negócio;
- Cálculo de valores;
- Disponibilidade do serviço de entrega;
- Códigos de resposta HTTP.

Os defeitos foram documentados e registrados no Jira durante a execução dos testes.

---

## 🛠️ Ferramentas

`Postman` `Jira` `Google Sheets` `ApiDoc` `JSON`

---

## 🧠 Competências

- Análise de requisitos;
- Planejamento e design de testes;
- Elaboração e execução de casos de teste;
- Testes de API;
- Testes funcionais;
- Validação de requisições e respostas;
- Validação de códigos HTTP;
- Aplicação de classes de equivalência e valores-limite;
- Validação de regras de negócio;
- Identificação e documentação de defeitos;
- Gerenciamento de bugs com Jira;
- Análise de dados de entrada.

---

## 📚 Contexto

Projeto prático desenvolvido como parte do Bootcamp de Analista de QA da TripleTen.

A atividade teve como foco o teste do backend da aplicação Urban.Grocers, envolvendo análise de requisitos, design de casos de teste, execução de requisições por meio do Postman e registro dos resultados.

Foram executados **70 casos de teste**, com **30 casos aprovados e 40 casos apresentando falhas**. Os comportamentos divergentes encontrados foram documentados e registrados no Jira.

Esta documentação resume as atividades realizadas durante o projeto, sem reproduzir materiais proprietários, requisitos internos ou arquivos originais da plataforma.
