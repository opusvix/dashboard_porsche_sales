# Porsche Enterprise Sales Intelligence

![Capa do Porsche Enterprise Sales Intelligence](assets/dashboard-porsche-sales-cover.png)

Dashboard executivo de vendas desenvolvido para transformar uma base comercial de veículos Porsche em uma experiência analítica interativa, responsiva e orientada à tomada de decisão.

> **Acesse o dashboard:** [Porsche Enterprise Sales Intelligence](https://opusvix.github.io/dashboard_porsche_sales/)

## Sobre o projeto

O projeto simula um cenário de análise comercial no qual gestores precisam acompanhar volume de vendas, receita, ticket médio, comportamento temporal, concentração geográfica, preferência por modelos e métodos de pagamento.

A solução foi construída com uma navegação inspirada em ferramentas corporativas de Business Intelligence, preservando uma identidade visual premium baseada no conceito **Executive Dark**.

## Objetivos de negócio

- Identificar os modelos Porsche mais vendidos.
- Comparar volume, receita e ticket médio entre períodos equivalentes.
- Avaliar a distribuição das vendas por cidade.
- Identificar o Model Year com maior participação.
- Analisar os métodos de pagamento utilizados.
- Explorar os registros por meio de drill-through.
- Transformar indicadores em insights executivos acionáveis.

## Indicadores acompanhados

| Indicador | Descrição |
|---|---|
| Veículos vendidos | Quantidade de registros no contexto selecionado |
| Receita | Soma do valor de venda dos veículos |
| Ticket médio | Receita dividida pela quantidade de vendas |
| Modelo líder | Modelo com maior volume de vendas |
| Cidade destaque | Cidade com maior quantidade de vendas |
| Variação temporal | Comparação do período atual com o período anterior equivalente |
| Qualidade temporal | Proporção de registros com data válida |

## Páginas do dashboard

### 01 — Resumo Executivo

- KPIs comerciais.
- Comparação com o período anterior.
- Evolução mensal das vendas.
- Ranking dos modelos.
- Insights executivos automáticos.

### 02 — Geografia

- Ranking das cidades.
- Distribuição geográfica das vendas.
- Heatmap Cidade × Modelo.
- Identificação do modelo líder em cada cidade.
- Drill-through por cidade, modelo ou combinação dos dois.

### 03 — Diagnóstico

- Receita por método de pagamento.
- Participação dos modelos na receita.
- Volume por Model Year.
- Indicadores de qualidade da base.
- Diagnóstico automático no contexto selecionado.

### 04 — Detalhamento

- Registros transacionais filtrados.
- Busca por modelo, cidade, pagamento, ano ou identificador.
- Resumo de quantidade, receita e ticket médio.
- Exportação dos resultados para CSV.

## Recursos de interação

- Filtros compartilhados por modelo, Model Year, cidade, método de pagamento e período.
- Períodos móveis de 3, 6, 12 ou 24 meses.
- Comparação automática com o período anterior equivalente.
- Drill-through a partir de gráficos, rankings, insights e heatmap.
- Tooltips analíticos com valor e participação.
- Bookmarks armazenados no dispositivo para recuperar visões personalizadas.
- Layout responsivo para computadores, tablets e smartphones.

## Qualidade e tratamento dos dados

A base utilizada contém **100 registros sanitizados**. Entre eles, **76 possuem datas válidas** e participam das análises temporais. Registros sem data permanecem disponíveis nos indicadores que não dependem da dimensão de tempo.

Esse tratamento evita que datas inválidas distorçam a evolução mensal e a comparação entre períodos.

## Tecnologias e conceitos aplicados

- React
- TypeScript
- HTML5 e CSS3
- Visualizações com SVG e CSS
- JavaScript `Intl` para formatação numérica
- `localStorage` para bookmarks
- Design responsivo
- Storytelling com dados
- Análise exploratória e definição de KPIs
- Cross-filter e drill-through

## Arquitetura analítica

```mermaid
flowchart LR
    A[Base sanitizada] --> B[Regras de filtros]
    B --> C[KPIs e agregações]
    C --> D[Visuais interativos]
    D --> E[Drill-through]
    E --> F[Detalhamento e CSV]
```

## Estrutura deste repositório

```text
dashboard_porsche_sales/
├── assets/
│   └── dashboard-porsche-sales-cover.png
├── docs/
│   ├── LINKEDIN_POST.md
│   ├── PORTFOLIO_ENTRY.md
│   └── PUBLICATION_GUIDE.md
└── README.md
```

## Principais aprendizados

- Sanitização de datas antes da criação de análises temporais.
- Desenvolvimento de filtros persistentes e sincronizados.
- Criação de visuais orientados a perguntas de negócio.
- Implementação de comparação entre períodos equivalentes.
- Construção de drill-through sem perder o contexto dos filtros.
- Comunicação transparente sobre qualidade e limitações da base.

## Desenvolvimento assistido por IA

O projeto foi concebido, direcionado e validado por **Maurício Barros**, com apoio do **ChatGPT/Codex da OpenAI** na estruturação da interface, implementação das interações, revisão do código, documentação e evolução do dashboard.

A colaboração com IA foi utilizada como ferramenta de produtividade e desenvolvimento, mantendo as decisões de negócio, critérios analíticos e validação final sob responsabilidade do autor.

## Aviso

Este é um projeto independente, criado para fins educacionais e de portfólio. Não possui vínculo, patrocínio ou afiliação oficial com a Porsche AG.

## Autor

**Maurício Barros**  
Analista de Dados | BI | Analytics

- [Portfólio](https://opusvix.github.io)
- [LinkedIn](https://www.linkedin.com/in/mauriciodasilvabarros/)
- [GitHub](https://github.com/opusvix)

