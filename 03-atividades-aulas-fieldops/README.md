# Módulo 03: Atividades Práticas das Aulas 01 a 08 — Projeto FieldOps

- **Instituição:** Faculdade de Tecnologia SENAI Antoine Skaf (UniSENAI-SP)
- **Curso:** Tecnologia em Análise e Desenvolvimento de Sistemas (ADS)
- **Disciplina:** Gestão de Projetos de TI
- **Docente:** Prof. Me. Deivison S. Takatu
- **Discente / Gerente de Projetos:** Giovani Miamoto (`giovanimiamotob`)

---

## 1. Visão Geral do Módulo

Este diretório reúne a resolução integral de todas as atividades e exercícios propostos ao final de cada apresentação de aula em formato PDF (`Aulas/Aula 01` a `Aula 08`). As atividades foram desenvolvidas tendo como caso prático o **Projeto FieldOps — Plataforma de Inspeção Técnica em Campo**, complementado pelo Projeto Integrador (SIGAI / MetalTech S.A.).

---

## 2. Mapa das Atividades por Aula e Entregáveis

| Aula | Tema da Aula no PMBOK | Atividade Solicitada no Slide | Documento Gerado |
| :---: | :--- | :--- | :--- |
| **Aula 01** | Apresentação da Disciplina & Contextualização | Resumo acadêmico em Markdown (.md) abordando conceitos fundamentais de Gestão de Projetos, ciclo de vida, PMBOK, programas, portfólio e estratégia | [01-resumo-aula-01.md](01-resumo-aula-01.md) |
| **Aula 02** | Fundamentos da Gestão de Projetos & Iniciação | Elaborar o Termo de Abertura do Projeto (TAP) do PII e do Projeto FieldOps com objetivos SMART, escopo em alto nível, marcos e orçamento | [02-tap-fieldops.md](02-tap-fieldops.md)<br>*(TAP do PII em [02-projeto-integrador](../02-projeto-integrador/avaliacao-1-planejamento-inicial/01-termo-de-abertura-tap.md))* |
| **Aula 03** | Processos e Áreas de Conhecimento (Escopo) | Elaborar a Estrutura Analítica do Projeto (EAP) do FieldOps com decomposição hierárquica, requisitos classificados e Dicionário da EAP | [03-eap-e-requisitos-fieldops.md](03-eap-e-requisitos-fieldops.md) |
| **Aula 04** | Planejamento do Projeto & Gerenciamento do Tempo | Elaborar o cronograma do FieldOps contendo **pelo menos 50 itens** com dependências, durações, responsáveis, marcos e Gantt Mermaid | [04-cronograma-fieldops-50-itens.md](04-cronograma-fieldops-50-itens.md) |
| **Aula 05** | Gerenciamento de Custos e Qualidade | 1. Orçamento com **pelo menos 30 itens** (PERT de três pontos, responsáveis e categorias)<br>2. Aplicação das **Sete Ferramentas Básicas da Qualidade** (Ishikawa, Fluxograma, Folha de Verificação, Pareto, Histograma, Carta de Controle e Dispersão) | [05-orcamento-e-qualidade-fieldops.md](05-orcamento-e-qualidade-fieldops.md) |
| **Aula 06** | Recursos Humanos & Comunicação | 1. Organograma da equipe e Matriz RACI detalhada<br>2. Plano de Comunicação completo com destinatários, responsáveis, canais, frequência e matriz 5W2H | [06-recursos-humanos-e-comunicacao-fieldops.md](06-recursos-humanos-e-comunicacao-fieldops.md) |
| **Aula 07** | Gerenciamento de Riscos | Análise de Riscos completa com EAR, Matriz 5x5 de Probabilidade × Impacto, estratégias de resposta (evitar, mitigar, transferir, aceitar), gatilhos e contingência | [07-gerenciamento-de-riscos-fieldops.md](07-gerenciamento-de-riscos-fieldops.md) |
| **Aula 08** | Aquisições & Partes Interessadas (Stakeholders) | 1. Tabela de Gerenciamento das Aquisições (item, urgência, motivo, fornecedores, quantidade, custo unitário e total)<br>2. Matriz de Rede de Poder/Interesse dos Stakeholders (Monitorar, Manter Informado, Manter Satisfeito, Gerenciar com Atenção) | [08-aquisicoes-e-stakeholders-fieldops.md](08-aquisicoes-e-stakeholders-fieldops.md) |

---

## 3. Síntese do Caso de Estudo: Projeto FieldOps

O **FieldOps** é uma plataforma corporativa web e mobile projetada para transformar a rotina operacional de equipes técnicas externas que realizam vistorias e manutenções em equipamentos industriais, climatização, subestações e instalações prediais:
- **Mobile (*Offline-First*):** Aplicativo React Native (Android) com persistência local SQLite, leitura de etiquetas QR Code nos ativos, checklists dinâmicos, captura de fotografias comprimidas com georreferenciamento e assinatura na tela.
- **Web Administrativo:** Painel de controle em Next.js para cadastro de plantas, ativos, usuários, construtor de formulários de vistoria, agendamento de OS e módulo de auditoria com aprovação/reprovação de laudos.
- **Backend & Nuvem:** API REST Node.js/TypeScript conteinerizada (AWS ECS), banco de dados relacional PostgreSQL (AWS RDS Multi-AZ) e repositório de evidências em nuvem (AWS S3).
