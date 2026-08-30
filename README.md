# 🧪 Teste de API – Urban.Grocers

## 📌 Sobre o projeto

Projeto de testes manuais de API realizado durante a formação em QA, com foco na validação de novas funcionalidades da API de uma aplicação de mercado/entrega de produtos (Urban.Grocers).

O projeto envolveu a análise de requisitos, elaboração de checklist, execução de testes utilizando o Postman e registro das falhas identificadas no Jira.

## 🎯 Objetivo

Validar o comportamento das novas funcionalidades da API, verificando se os requisitos definidos para o gerenciamento de produtos em kits e para o serviço de entrega estavam sendo atendidos.

Os testes também buscaram identificar problemas relacionados à validação de dados, regras de negócio, limites e tratamento de entradas inválidas.

## 🔍 Escopo dos testes

Foram testadas as seguintes funcionalidades:

- Adição e atualização de produtos em kits;
- Validação dos parâmetros do endpoint de kits;
- Limite de produtos permitidos em um kit;
- Verificação da disponibilidade do serviço de entrega Order and Go;
- Validação do cálculo do custo de entrega;
- Validação dos parâmetros utilizados no cálculo da entrega;
- Tratamento de valores nulos, vazios, negativos, inválidos e parâmetros ausentes.

A autorização não fez parte do escopo dos testes, conforme definido na tarefa.

## 🛠️ Tecnologias e ferramentas

- **Postman**
- **Jira**
- **API Testing**
- **Testes manuais**
- **Análise de requisitos**
- **Checklist de testes**
- **JSON**

## 📊 Resultados dos testes

Foram executados **70 casos de teste** nos dois endpoints analisados.

| Endpoint | Casos executados | Aprovados | Reprovados |
|---|---:|---:|---:|
| `POST /api/v1/kits/:id/products` | 26 | 6 | 20 |
| `POST /order-and-go/v1/delivery` | 44 | 13 | 31 |
| **Total** | **70** | **19** | **51** |

Os testes permitiram validar cenários positivos, valores de limite e diferentes condições de entrada, além de identificar comportamentos divergentes em relação aos requisitos.

As falhas encontradas foram documentadas e reportadas no Jira para acompanhamento.

## 🐞 Bugs encontrados

Durante a execução dos testes foram identificadas falhas relacionadas principalmente a:

- Validação inadequada de parâmetros;
- Aceitação de valores inválidos ou negativos;
- Tratamento incorreto de parâmetros nulos, vazios ou ausentes;
- Retorno de `500 Internal Server Error` em situações que deveriam resultar em `400 Bad Request`;
- Divergências nas regras de cálculo do serviço de entrega;
- Comportamentos diferentes dos esperados em determinados limites de quantidade, peso e tempo de entrega.

Todos os casos de teste classificados como **REPROVADO** tiveram suas respectivas falhas documentadas e reportadas no Jira.

## 📋 Documentação dos testes

A documentação apresenta o planejamento e a execução dos testes realizados, incluindo os dados utilizados, resultados esperados, resultados obtidos, status dos testes e referências aos relatórios de bug.

➡️ [Acessar documentação dos testes](./test-cases/api-testing.md)

## 📚 Competências desenvolvidas

- Análise e interpretação de requisitos;
- Planejamento e elaboração de testes;
- Testes funcionais de API;
- Testes de validação de dados;
- Testes de valores limite;
- Identificação e documentação de bugs;
- Utilização do Postman para testes de API;
- Registro e acompanhamento de bugs no Jira;
- Documentação de resultados de testes.
