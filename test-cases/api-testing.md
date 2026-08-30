# 🧪 Testes de API – Urban.Grocers

## 📌 Escopo

Testes realizados na nova versão da API do Urban.Grocers, com foco nas seguintes funcionalidades:

- Adição de produtos a kits;
- Validação dos parâmetros do endpoint de kits;
- Validação do limite de produtos em um kit;
- Verificação da disponibilidade do serviço de entrega Order and Go;
- Validação do cálculo do custo de entrega;
- Validação dos parâmetros utilizados no cálculo da entrega;
- Tratamento de dados inválidos, ausentes, nulos, vazios e valores fora dos limites especificados.

A autorização não fez parte do escopo dos testes, conforme definido na tarefa.

## 🔧 Metodologia

Os testes foram elaborados a partir da análise dos requisitos do back-end e da documentação da API.

Foram aplicadas técnicas de validação de dados e testes de limites, considerando diferentes tipos e valores de entrada para verificar o comportamento da API em cenários positivos e negativos.

A execução dos testes foi realizada utilizando o **Postman**, com registro dos resultados e documentação das falhas encontradas no **Jira**.

## 📊 Resultados

Foram executados **70 casos de teste**, distribuídos entre os dois endpoints analisados.

| Endpoint | Casos executados | Aprovados | Reprovados |
|---|---:|---:|---:|
| `POST /api/v1/kits/:id/products` | 26 | 6 | 20 |
| `POST /order-and-go/v1/delivery` | 44 | 13 | 31 |
| **Total** | **70** | **19** | **51** |

Os testes aprovados confirmaram o funcionamento esperado de diferentes cenários, incluindo a adição e atualização de produtos em kits, o limite de 30 itens e diferentes condições para cálculo do serviço de entrega.

Os testes reprovados evidenciaram problemas principalmente relacionados ao tratamento de entradas inválidas, validação de parâmetros e aplicação de algumas regras de negócio.

## 🐞 Bugs

As falhas identificadas durante a execução foram documentadas e reportadas no **Jira**, permitindo o registro e acompanhamento dos problemas encontrados.

Entre os principais comportamentos observados estavam:

- Retorno de `200 OK` para dados que deveriam ser rejeitados com `400 Bad Request`;
- Retorno de `500 Internal Server Error` em situações de dados inválidos;
- Falhas na validação de parâmetros obrigatórios;
- Aceitação de valores negativos ou inválidos;
- Comportamentos divergentes nas regras de cálculo do serviço de entrega;
- Divergências na aplicação de limites relacionados ao peso e à quantidade de produtos.

## 🛠️ Tecnologias e ferramentas

- **Postman**
- **Jira**
- **API Testing**
- **Testes manuais**
- **Análise de requisitos**
- **Checklist de testes**
- **JSON**
