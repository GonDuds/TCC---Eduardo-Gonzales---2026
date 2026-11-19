# TCC---Eduardo-Gonzales---2026
Repositorio dedicado a documentação do  trabalho de conclusão de curso Engenharia de software


# 🧁 Delícia Cupcakes — Web App (PIT Engenharia de Software)

Aplicação Web Responsiva (*Mobile-First*) desenvolvida como Projeto Integrador Transdisciplinar (PIT) do curso de Bacharelado em Engenharia de Software, aplicando o ciclo de melhoria contínua (**Kaizen**) sobre o planejamento inicial de requisitos, modelagem UML, IHC e banco de dados relacional.

**Autor:** Eduardo de Melo Gonzales (RGM: 35226960)

---

## 🎯 Objetivo e Melhorias Aplicadas (Kaizen)
A solução atende a uma confeitaria gourmet que precisava reestruturar sua operação digital após falhas anteriores de levantamento de requisitos. Na evolução para a etapa de desenvolvimento e testes, foram aplicadas as seguintes melhorias:
* **Alinhamento de Escopo (MVP):** Consolidação da arquitetura em Web App Responsivo (Mobile-First), unificando a jornada do cliente (vitrine, personalização, carrinho, PIX) e a operação interna (Kanban da cozinha e estoque).
* **Refinamento UML:** Correção de tipagem e atributos multivalorados no Diagrama de Classes de Persistência, inclusão de entidades associativas para receitas personalizadas e adição do Diagrama de Atividades e Diagrama de Sequência transacional.
* **Evolução de IHC e Prototipação:** Inclusão de telas de checkout com busca automática de CEP (ViaCEP), pagamento via PIX com cronômetro, rastreamento de status e feedback visual de erros (prevenção de combinações térmicas inválidas e cupons expirados).
* **Banco de Dados Normalizado (3FN):** Estrutura relacional com integridade referencial, chaves primárias/estrangeiras e controle transacional de baixa de insumos.

---

## 🛠️ Tecnologias Utilizadas
* **Back-end:** Python 3, FastAPI, Uvicorn, Pydantic
* **Front-end:** HTML5, Tailwind CSS, JavaScript (Vanilla ES6+ / Fetch API)
* **Banco de Dados:** SQLite (com script DDL compatível com PostgreSQL)
* **Modelagem & Design:** Draw.io (UML e DER) e Figma (Wireframes e Protótipo Navegável)

---

## 📂 Estrutura do Repositório
```text
├── app.py                  # API REST (FastAPI) e regras de negócio
├── index.html              # Interface Web Responsiva (Cliente + Cozinha/Admin)
├── criar_banco.py          # Script DDL de criação das 9 tabelas relacionais
├── popular_banco.py        # Script de carga inicial (seed) de produtos, insumos e pedidos
├── delicia_cupcakes.db     # Banco de dados SQLite pronto para execução
├── requirements.txt        # Dependências do projeto Python
└── docs/                   # Documentação de dados (DER, 3FN e Dicionário de Dados)
