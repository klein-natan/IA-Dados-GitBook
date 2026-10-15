# Roadmap

Nesta disciplina vamos seguir um caminho claro e estruturado: primeiro o contexto, depois os métodos de análise, e só então a inteligência artificial aplicada.

```mermaid
%%{init:{"theme":"base","themeVariables":{"fontFamily":"Inter,'Segoe UI','Liberation Sans',Helvetica,Arial,sans-serif","fontSize":"15px","primaryColor":"#F4F2EE","primaryTextColor":"#1E2A25","primaryBorderColor":"#CBD8D0","lineColor":"#8A9A90","secondaryColor":"#EDF2EE","tertiaryColor":"#FFFFFF","clusterBkg":"#F8F7F4","clusterBorder":"#E2DED7","edgeLabelBackground":"#FFFFFF"},"flowchart":{"nodeSpacing":28,"rankSpacing":38,"padding":14,"curve":"basis"}}}%%
flowchart LR
    F1("<b>Fase 1</b><br/><b>Fundamentos e contexto</b><br/><br/>Apresentação da disciplina<br/>Problemas de negócio<br/>e projetos de dados")
    F2("<b>Fase 2</b><br/><b>Métodos de análise</b><br/><br/>Dados discretos<br/>Dados contínuos<br/>Séries temporais<br/>Associações")
    F3("<b>Fase 3</b><br/><b>IA na prática</b><br/><br/>Introdução à IA generativa<br/>Agentes de IA<br/>Análise de dados com IA")
    F1 --> F2 --> F3
    classDef medio fill:#C8DDD0,stroke:#AECBBB,color:#1E2A25;
    classDef nevoa fill:#EAF1EC,stroke:#C3D6CA,color:#1E2A25;
    classDef verde fill:#5F9C7A,stroke:#5F9C7A,color:#FFFFFF;
    class F1 nevoa
    class F2 medio
    class F3 verde
```

Cada fase resolve um problema da anterior. A Fase 1 explica por que analisar dados muda uma decisão. A Fase 2 entrega as ferramentas para analisar. A Fase 3 usa IA para fazer em minutos o que a Fase 2 faz em horas — e para responder perguntas que a Fase 2 sozinha não alcança.

## Fase 3 · IA na prática

Na Fase 3, cada aula entrega um projeto publicado. Os conceitos de IA, as técnicas de prompting e o spec-driven development aparecem quando o projeto precisa deles, do mais básico ao mais avançado.

```mermaid
%%{init:{"theme":"base","themeVariables":{"fontFamily":"'Segoe UI',Inter,Helvetica,Arial,sans-serif","fontSize":"15px","primaryColor":"#F3F4F8","primaryTextColor":"#171A2B","primaryBorderColor":"#DFE2EA","lineColor":"#8C90A6","secondaryColor":"#E4E2FB","tertiaryColor":"#FFFFFF","clusterBkg":"#F7F8FB","clusterBorder":"#DFE2EA","edgeLabelBackground":"#FFFFFF"},"flowchart":{"nodeSpacing":28,"rankSpacing":38,"padding":14,"curve":"basis"}}}%%
flowchart LR
    A6("<b>Aula 6</b><br/>Site pessoal<br/><i>universo da IA</i>") --> A7("<b>Aula 7</b><br/>Relatório do Vitto<br/><i>IA que calcula</i>")
    A7 --> A8("<b>Aula 8</b><br/>Dashboard<br/><i>agentes</i>")
    A8 --> A9("<b>Aula 9</b><br/>App de pedidos<br/><i>spec-driven development</i>")
    A9 --> A10("<b>Aula 10</b><br/>Agente pessoal<br/><i>API, RAG e MCP</i>")
    classDef claro fill:#E4E2FB,stroke:#C9C5F5,color:#171A2B;
    classDef medio fill:#B9B5F2,stroke:#A29DEB,color:#171A2B;
    classDef forte fill:#4F46E5,stroke:#4F46E5,color:#FFFFFF;
    classDef destaque fill:#2F2A8F,stroke:#2F2A8F,color:#FFFFFF;
    class A6,A7 claro
    class A8 medio
    class A9 forte
    class A10 destaque
```

Antes da Aula 6, siga a página [Prepare o seu computador](ia-preparacao.md). As técnicas de todas as aulas estão reunidas no [Caderno de prompts e specs](ia-caderno-de-prompts.md).
