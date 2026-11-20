# Cronograma Detalhado do Projeto FieldOps (55+ Atividades)
## Planejamento Temporal, Sequenciamento, Dependências e Caminho Crítico

- **Disciplina:** Gestão de Projetos de TI (UniSENAI-SP)
- **Docente:** Prof. Me. Deivison S. Takatu
- **Autor / Gerente de Projetos:** Giovani Miamoto (`giovanimiamotob`)
- **Referência:** Aula 04 — Planejamento do Projeto e Gerenciamento do Tempo
- **Requisito do Enunciado:** Cronograma estruturado contendo pelo menos 50 itens com dependências, durações, responsáveis e marcos (*milestones*).
- **Versão:** 1.0 (Aprovada)

---

## 1. Metodologia de Gestão do Tempo e Parâmetros de Linha de Base

O cronograma do Projeto FieldOps foi desenvolvido com base no **Método do Caminho Crítico (CPM - *Critical Path Method*)**, articulado com iterações ágeis (Sprints quinzenais).

### Parâmetros Operacionais:
- **Duração Total do Projeto:** 16 semanas úteis (80 dias úteis de trabalho).
- **Carga Horária de Referência:** 8 horas/dia por colaborador (segunda a sexta-feira).
- **Convenção de Dependências:**
  - `TI` = Término para Início (*Finish-to-Start*)
  - `II` = Início para Início (*Start-to-Start*)
  - `TT` = Término para Término (*Finish-to-Finish*)
- **Marcos (*Milestones*):** Eventos de controle de progresso com duração igual a `0 dias`.

---

## 2. Tabela Mestra do Cronograma (56 Itens)

Abaixo apresenta-se o cronograma completo com 56 itens decompostos:

| ID | EAP | Descrição da Atividade / Marco | Duração (Dias) | Predecessoras | Responsável | Fase / Sprint | Caminho Crítico |
| :---: | :---: | :--- | :---: | :---: | :--- | :---: | :---: |
| **01** | 1.1.1 | Levantamento de escopo e elaboração do TAP | 5 | - | Gerente de Projetos | Iniciação | **SIM** |
| **02** | 1.1.1 | Reunião de alinhamento com Sponsor e Stakeholders | 2 | 01 (TI) | Gerente de Projetos | Iniciação | **SIM** |
| **03** | 1.1.1 | **MARCO M0: TAP Aprovado e Kick-off Realizado** | **0** | **02 (TI)** | **Sponsor / GP** | **Marco** | **SIM** |
| **04** | 1.1.2 | Detalhamento da EAP e Dicionário de Pacotes | 4 | 03 (TI) | Gerente de Projetos | Planejamento | **SIM** |
| **05** | 1.1.2 | Definição da Linha de Base de Custos e Orçamento | 3 | 04 (TI) | Gerente de Projetos | Planejamento | **SIM** |
| **06** | 1.1.2 | Elaboração da Matriz de Riscos e Planos de Resposta | 3 | 05 (TI) | GP / Tech Lead | Planejamento | NÃO |
| **07** | 1.1.2 | Elaboração da Matriz RACI e Plano de Comunicação | 2 | 05 (TI) | Gerente de Projetos | Planejamento | NÃO |
| **08** | 1.1.2 | Planejamento das Aquisições e Fornecedores Cloud | 3 | 05 (TI) | GP / Finanças | Planejamento | NÃO |
| **09** | 1.2.1 | Engenharia de Requisitos: Entrevistas com Supervisores | 4 | 03 (TI) | UI/UX / Tech Lead | Sprint 0 | **SIM** |
| **10** | 1.2.1 | Engenharia de Requisitos: Acompanhamento de Técnicos em Campo | 3 | 09 (TI) | UI/UX Designer | Sprint 0 | **SIM** |
| **11** | 1.2.1 | Elaboração dos Diagramas de Caso de Uso e Fluxos | 3 | 10 (TI) | Tech Lead | Sprint 0 | **SIM** |
| **12** | 1.2.1 | Modelagem Conceitual e Lógica do Banco de Dados | 4 | 11 (TI) | Tech Lead / Backend | Sprint 0 | **SIM** |
| **13** | 1.2.2 | Criação de Wireframes de Baixa Fidelidade (Web e Mobile) | 5 | 10 (TI) | UI/UX Designer | Sprint 0 | NÃO |
| **14** | 1.2.2 | Criação do Protótipo Navegável de Alta Fidelidade no Figma | 6 | 13 (TI) | UI/UX Designer | Sprint 1 | NÃO |
| **15** | 1.2.2 | Teste de Usabilidade do Protótipo com Técnicos Piloto | 3 | 14 (TI) | UI/UX Designer | Sprint 1 | NÃO |
| **16** | 1.2.3 | **MARCO M1: Arquitetura e Protótipos Aprovados** | **0** | **12, 15 (TI)**| **GP / Tech Lead** | **Marco** | **SIM** |
| **17** | 1.2.2 | Provisionamento da Infraestrutura Cloud AWS (VPC, RDS) | 3 | 16 (TI) | DevOps / Tech Lead | Sprint 1 | **SIM** |
| **18** | 1.2.2 | Configuração de Buckets S3 e Políticas de Acesso IAM | 2 | 17 (TI) | DevOps Engineer | Sprint 1 | **SIM** |
| **19** | 1.2.3 | Configuração da Pipeline CI/CD com GitHub Actions | 3 | 18 (TI) | DevOps Engineer | Sprint 1 | **SIM** |
| **20** | 1.3.1 | Setup do Boilerplate da API REST (Node.js/TypeScript) | 2 | 16 (TI) | Dev Backend Sr | Sprint 1 | NÃO |
| **21** | 1.3.1 | Implementação da Autenticação JWT e Middleware RBAC | 4 | 19, 20 (TI)| Dev Backend Sr | Sprint 2 | **SIM** |
| **22** | 1.3.2 | Criação dos CRUDs de Clientes e Plantas de Atendimento | 3 | 21 (TI) | Dev Backend Pl | Sprint 2 | NÃO |
| **23** | 1.3.2 | Criação do CRUD de Equipamentos e Gerador de QR Code | 4 | 22 (TI) | Dev Backend Pl | Sprint 2 | NÃO |
| **24** | 1.3.3 | Implementação do Motor de Modelos de Checklist Dinâmicos | 5 | 21 (TI) | Dev Backend Sr | Sprint 2 | **SIM** |
| **25** | 1.3.3 | Endpoints de Agendamento e Atribuição de Ordens de Serviço | 4 | 24 (TI) | Dev Backend Sr | Sprint 3 | **SIM** |
| **26** | 1.3.4 | Desenvolvimento do Endpoint Transacional de Sincronização | 6 | 25 (TI) | Dev Backend Sr | Sprint 3 | **SIM** |
| **27** | 1.3.4 | Implementação do Tratamento de Idempotência e Conflitos | 4 | 26 (TI) | Dev Backend Sr | Sprint 3 | **SIM** |
| **28** | 1.3.4 | Endpoint de Upload de Evidências com URLs Pré-assinadas S3 | 3 | 27 (TI) | Dev Backend Pl | Sprint 3 | **SIM** |
| **29** | 1.3.5 | Documentação Interativa da API com Swagger / OpenAPI 3.0 | 3 | 28 (TI) | Dev Backend Pl | Sprint 4 | NÃO |
| **30** | 1.3.5 | **MARCO M2: API REST Core Concluída e Operacional** | **0** | **28 (TI)** | **Tech Lead** | **Marco** | **SIM** |
| **31** | 1.4.1 | Setup do Projeto Expo / React Native e Estrutura de Pastas | 2 | 16 (TI) | Dev Mobile Pl | Sprint 2 | NÃO |
| **32** | 1.4.1 | Configuração do Banco Local SQLite e Migrações Offline | 4 | 31 (TI) | Dev Mobile Pl | Sprint 2 | NÃO |
| **33** | 1.4.2 | Telas de Login, Perfil e Troca de Senha Mobile | 3 | 21, 32 (TI)| Dev Mobile Pl | Sprint 2 | NÃO |
| **34** | 1.4.2 | Mecanismo de Download e Cache Local de Ordens de Serviço | 4 | 25, 33 (TI)| Dev Mobile Pl | Sprint 3 | NÃO |
| **35** | 1.4.3 | Integração com Leitor de Câmera para Scanner de QR Code | 3 | 34 (TI) | Dev Mobile Pl | Sprint 3 | NÃO |
| **36** | 1.4.4 | Renderizador Dinâmico de Checklists (Múltiplos Componentes)| 6 | 35 (TI) | Dev Mobile Pl | Sprint 3 | **SIM** |
| **37** | 1.4.5 | Módulo de Câmera Nativa e Compressão Client-side de Fotos | 4 | 36 (TI) | Dev Mobile Pl | Sprint 4 | **SIM** |
| **38** | 1.4.5 | Integração de Módulo GPS (Captura de Coordenadas) | 2 | 36 (TI) | Dev Mobile Pl | Sprint 4 | NÃO |
| **39** | 1.4.6 | Componente de Captura de Rubrica / Assinatura Digital | 3 | 37 (TI) | Dev Mobile Pl | Sprint 4 | **SIM** |
| **40** | 1.4.6 | Serviço de Fila de Sincronização em Background (NetInfo) | 5 | 30, 39 (TI)| Dev Mobile Sr | Sprint 4 | **SIM** |
| **41** | 1.5.1 | Setup da Interface Web com Next.js, TailwindCSS e Shadcn UI | 3 | 16 (TI) | Dev Frontend Web | Sprint 2 | NÃO |
| **42** | 1.5.1 | Telas de Login, Recuperação e Layout do Dashboard Web | 3 | 21, 41 (TI)| Dev Frontend Web | Sprint 2 | NÃO |
| **43** | 1.5.2 | Telas de Gerenciamento de Clientes, Plantas e Ativos | 4 | 23, 42 (TI)| Dev Frontend Web | Sprint 3 | NÃO |
| **44** | 1.5.3 | Construtor Visual Interativo de Modelos de Formulário | 5 | 24, 43 (TI)| Dev Frontend Web | Sprint 3 | NÃO |
| **45** | 1.5.4 | Calendário e Matriz de Agendamento e Atribuição de Técnicos | 4 | 25, 44 (TI)| Dev Frontend Web | Sprint 3 | NÃO |
| **46** | 1.5.5 | Tela de Acompanhamento em Tempo Real do Status das OS | 4 | 45 (TI) | Dev Frontend Web | Sprint 4 | NÃO |
| **47** | 1.5.5 | Módulo de Revisão de Laudos, Parecer e Reprovação/Aprovação | 5 | 40, 46 (TI)| Dev Frontend Web | Sprint 4 | **SIM** |
| **48** | 1.5.6 | Gerador de Laudos Técnicos em PDF Padronizado | 4 | 47 (TI) | Dev Frontend Web | Sprint 5 | **SIM** |
| **49** | 1.5.6 | **MARCO M3: Versão Alpha Integrada (Web + Mobile + API)**| **0** | **40, 48 (TI)**| **GP / Equipe** | **Marco** | **SIM** |
| **50** | 1.6.1 | Execução de Bateria de Testes Automatizados E2E | 5 | 49 (TI) | Analista de QA | Sprint 5 | **SIM** |
| **51** | 1.6.2 | Testes de Estresse de Rede e Simulação de Falhas Offline | 4 | 50 (TI) | QA / Tech Lead | Sprint 5 | **SIM** |
| **52** | 1.6.3 | Implantação do Piloto de Campo com 5 Técnicos Selecionados | 6 | 51 (TI) | GP / Supervisores | Sprint 5 | **SIM** |
| **53** | 1.6.3 | **MARCO M4: Piloto UAT Concluído e Ajustes Validados** | **0** | **52 (TI)** | **Sponsor / GP** | **Marco** | **SIM** |
| **54** | 1.6.4 | Treinamento Operacional dos Técnicos e Supervisores | 3 | 53 (TI) | GP / Treinador | Sprint 6 | **SIM** |
| **55** | 1.6.5 | Deploy Final em Produção e Corte do Legado de Papel | 2 | 54 (TI) | DevOps / Tech Lead | Sprint 6 | **SIM** |
| **56** | 1.6.5 | **MARCO M5: Go-Live e Encerramento Formal do Projeto** | **0** | **55 (TI)** | **Sponsor Executivo**| **Marco** | **SIM** |

---

## 3. Diagrama de Gantt do Projeto FieldOps

O diagrama abaixo ilustra o sequenciamento macro ao longo das 16 semanas:

```mermaid
gantt
    title Cronograma de Execução do Projeto FieldOps (16 Semanas)
    dateFormat  YYYY-MM-DD
    axisFormat  %d/%m
    
    section Iniciação & Gestão
    TAP e Kick-off               :done, des01, 2026-08-03, 7d
    Planejamento Detalhado (EAP) :done, des02, after des01, 7d
    Marco M0: TAP Aprovado       :milestone, m0, 2026-08-10, 0d
    
    section Design & Requisitos
    Entrevistas & Levantamento   :done, des03, 2026-08-10, 7d
    Modelagem BD & Wireframes    :done, des04, after des03, 10d
    Protótipo Figma & Teste UI   :done, des05, after des04, 8d
    Marco M1: Protótipo e Arq    :milestone, m1, 2026-09-04, 0d
    
    section Infra & Backend API
    Setup Cloud AWS & CI/CD      :active, des06, after m1, 5d
    Auth JWT, RBAC & Modelos     :active, des07, after des06, 12d
    Motor de Sincronização & S3  :active, des08, after des07, 10d
    Marco M2: API REST Concluída :milestone, m2, 2026-10-02, 0d
    
    section Mobile Android
    Setup SQLite Offline         :des09, after m1, 6d
    Download OS & Scanner QR     :des10, after des09, 7d
    Checklist Dinâmico & Câmera  :des11, after des10, 10d
    Fila de Sync Background      :des12, after des11, 8d
    
    section Web Admin Next.js
    Dashboard & Cadastros Base   :des13, after m1, 10d
    Editor Checklists & Agenda   :des14, after des13, 9d
    Módulo de Revisão & PDF      :des15, after des14, 9d
    Marco M3: Alpha Integrado    :milestone, m3, 2026-10-23, 0d
    
    section Homologação & Go-Live
    Bateria de Testes QA E2E     :des16, after m3, 8d
    Piloto UAT com 5 Técnicos    :des17, after des16, 8d
    Marco M4: Piloto Validado    :milestone, m4, 2026-11-13, 0d
    Treinamento & Deploy Prod    :des18, after m4, 5d
    Marco M5: Go-Live Concluído  :milestone, m5, 2026-11-20, 0d
```

---

## 4. Análise do Caminho Crítico (CPM)

O caminho crítico identificado totaliza **80 dias úteis** contíguos sem folga (*float = 0*). As atividades que compõem o caminho crítico são:

```
[01/02 TAP] ➔ [04 EAP] ➔ [09/10 Requisitos] ➔ [11/12 Modelagem] ➔ [16 M1] ➔
[17/19 Setup Cloud/CI-CD] ➔ [21 Auth JWT] ➔ [24 Modelos Checklist] ➔ 
[25 Agendamento] ➔ [26/28 Sync API Core] ➔ [30 M2] ➔ [36 Checklist Mobile] ➔ 
[37 Câmera/Fotos] ➔ [39 Assinatura] ➔ [40 Fila Sync] ➔ [47 Revisão Web] ➔ 
[48 Emissor PDF] ➔ [49 M3] ➔ [50/51 Testes QA] ➔ [52 Piloto UAT] ➔ 
[53 M4] ➔ [54 Treinamento] ➔ [55 Deploy Prod] ➔ [56 M5 Go-Live]
```

### Estratégias de Mitigação de Atrasos:
1. **Compressão (*Crashing*):** Em caso de desvio no desenvolvimento da sincronização *offline* (ID 26 e 40), o desenvolvedor sênior da Web apoiará diretamente a implementação mobile.
2. **Paralelismo (*Fast-Tracking*):** O desenvolvimento do gerador de PDF (ID 48) e das telas de cadastro administrativo foi desacoplado para ocorrer simultaneamente aos testes do motor de sincronização.
