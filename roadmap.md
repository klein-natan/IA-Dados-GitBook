# Roadmap

Nesta disciplina vamos seguir um caminho claro e estruturado: primeiro o contexto, depois os métodos de análise, e só então a inteligência artificial aplicada.

```mermaid
flowchart LR
    subgraph F1["Fase 1 · Fundamentos e contexto"]
        direction TB
        A1["Apresentação da disciplina<br/>e introdução aos dados"]
        A2["Problemas de negócio<br/>e projetos de dados"]
        A1 --> A2
    end
    subgraph F2["Fase 2 · Métodos de análise de dados"]
        direction TB
        B1["Análise de dados discretos"]
        B2["Análise de dados contínuos"]
        B3["Análise de séries temporais"]
        B4["Análise de associações"]
        B1 --> B2 --> B3 --> B4
    end
    subgraph F3["Fase 3 · Inteligência artificial na prática"]
        direction TB
        C1["Introdução à IA generativa"]
        C2["Agentes de IA"]
        C3["Análise de dados com IA"]
        C1 --> C2 --> C3
    end
    F1 --> F2 --> F3
```

Cada fase resolve um problema da anterior. A Fase 1 explica por que analisar dados muda uma decisão. A Fase 2 entrega as ferramentas para analisar. A Fase 3 usa IA para fazer em minutos o que a Fase 2 faz em horas — e para responder perguntas que a Fase 2 sozinha não alcança.
