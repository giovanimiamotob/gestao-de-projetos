# CENTRO UNIVERSITÁRIO SENAI SÃO PAULO — UNISENAI-SP
## CAMPUS SOROCABA — SANTA ROSÁLIA
### CURSO SUPERIOR DE TECNOLOGIA EM ANÁLISE E DESENVOLVIMENTO DE SISTEMAS

<br/><br/>

# 📘 RELATÓRIO TÉCNICO-ACADÊMICO CONSOLIDADO
## IMPLANTAÇÃO DO SISTEMA INTEGRADO DE AUTOMAÇÃO E GESTÃO INDUSTRIAL (SIGAI) E DIRECIONAMENTO ESTRATÉGICO DE PORTFÓLIO NA METALTECH S.A.

<br/><br/>

**Autor:** Giovani Miamoto  
**Matrícula / Usuário:** `giovanimiamotob`  
**Orientador:** Prof. Me. Deivison Takatu  
**Disciplina:** Gestão de Projetos  

**SOROCABA — SP**  
**2026**

---

## FOLHA DE ROSTO

**GIOVANI MIAMOTO**

### IMPLANTAÇÃO DO SISTEMA INTEGRADO DE AUTOMAÇÃO E GESTÃO INDUSTRIAL (SIGAI) E DIRECIONAMENTO ESTRATÉGICO DE PORTFÓLIO NA METALTECH S.A.

Trabalho de Conclusão e Avaliação Integrada apresentado ao Centro Universitário SENAI São Paulo — UniSENAI-SP Campus Sorocaba - Santa Rosália como instrumento formal de avaliação da disciplina de **Gestão de Projetos** do Curso Superior de Tecnologia em Análise e Desenvolvimento de Sistemas.

**Área de Concentração:** Engenharia de Software, Gestão Estratégica e Automação Industrial 4.0.  
**Orientador:** Prof. Me. Deivison Takatu  

**SOROCABA — SP**  
**2026**

---

## RESUMO

O presente relatório técnico-acadêmico consolida o planejamento, estruturação estratégica de portfólio e gestão integrada do projeto de modernização tecnológica da empresa fictícia MetalTech S.A., fabricante de componentes metálicos para a cadeia automotiva. Em face de um ambiente industrial com apontamentos manuais descentralizados, altos índices de refugo e perdas operacionais por paradas não programadas, a diretoria executiva instituiu quatro objetivos estratégicos para o ciclo de 12 meses: elevação de 15% na produtividade, redução de 20% nas paradas de linha, redução de 10% nos custos operacionais e redução de 30% no retrabalho interno, sob uma restrição orçamentária máxima de R$ 2,5 milhões e com uma equipe enxuta de 7 especialistas técnicos. A metodologia adotada fundamentou-se nos preceitos do Guia PMBOK (Project Management Body of Knowledge), integrando práticas ágeis (Scrum/Kanban) e normas técnicas consagradas (ISO 9001:2015, IATF 16949, ISO/IEC 25010, NR-10 e NR-12). Como primeira etapa, procedeu-se à análise multicritério de 8 projetos candidatos, estruturando um portfólio composto por dois programas integrados ("Excelência Operacional" e "Qualidade Integrada"), alocando R$ 2,1 milhões e preservando R$ 400 mil em reserva gerencial estratégica. Na segunda etapa, detalhou-se o planejamento de ponta a ponta do Projeto SIGAI (Sistema Integrado de Automação e Gestão Industrial), abarcando o Termo de Abertura do Projeto (TAP), matriz de partes interessadas, plano de comunicação 5W2H, declaração de escopo, Estrutura Analítica do Projeto (EAP) com dicionário analítico, cronograma em rede com caminho crítico e gráfico de Gantt, orçamento por curva S, garantia e controle da qualidade, registro analítico de 10 riscos com planos de mitigação, comitê de controle de mudanças (CCB) e procedimentos de encerramento e transição. Os resultados evidenciam a plena viabilidade da estratégia proposta, comprovando o cumprimento de 100% das metas corporativas com alocação equilibrada de recursos humanos e mitigação antecipada dos riscos operacionais.

**Palavras-chave:** Gestão de Projetos; PMBOK; Gestão de Portfólio; Indústria 4.0; Automação Industrial; OEE; Qualidade Assegurada.

---

## ABSTRACT

This comprehensive academic and technical report consolidates the project planning, strategic portfolio alignment, and integrated project management for the technological modernization of the fictional company MetalTech S.A., an automotive metal component manufacturer. Confronted with decentralized manual floor records, high scrap rates, and severe production downtimes, the executive board mandated four 12-month strategic goals: a 15% increase in productivity, a 20% reduction in production stoppages, a 10% cut in operational costs, and a 30% reduction in internal rework, constrained by a strict budgetary ceiling of R$ 2.5 million and a specialized team of 7 professionals. The applied methodology was grounded in the PMBOK Guide framework, blending agile practices (Scrum/Kanban) and industrial standards (ISO 9001:2015, IATF 16949, ISO/IEC 25010, NR-10, and NR-12). In the initial phase, a multicriteria decision matrix evaluated 8 candidate initiatives, organizing the approved projects into two synergetic programs ("Operational Excellence" and "Integrated Quality"), committing R$ 2.1 million while shielding R$ 400,000.00 in strategic reserves. In the second phase, an end-to-end management baseline was developed for the SIGAI Project (Integrated Industrial Automation and Management System), encompassing the Project Charter, stakeholder register, 5W2H communication plan, scope statement, WBS dictionary, CPM schedule with Gantt visual representation, cost baseline with S-curve, quality control, an analytical register of 10 risks with response strategies, change control board governance, and formal closeout procedures. The resulting implementation demonstrates the total feasibility of the strategy, fulfilling 100% of the strategic targets while preventing resource burnout and ensuring predictable operational returns.

**Keywords:** Project Management; PMBOK; Portfolio Management; Industry 4.0; Industrial Automation; OEE; Quality Assurance.

---

## LISTA DE SIGLAS E ABREVIATURAS

* **ABNT:** Associação Brasileira de Normas Técnicas
* **BAC:** Budget at Completion (Orçamento Total no Término)
* **CAD:** Computer Aided Design (Desenho Assistido por Computador)
* **CCB:** Change Control Board (Comitê de Controle de Mudanças)
* **CLP:** Controlador Lógico Programável
* **CPI:** Cost Performance Index (Índice de Desempenho de Custos)
* **DMZ:** Demilitarized Zone (Zona Desmilitarizada de Rede)
* **EAP:** Estrutura Analítica do Projeto (WBS - Work Breakdown Structure)
* **EVM:** Earned Value Management (Gerenciamento do Valor Agregado)
* **FAT:** Factory Acceptance Test (Teste de Aceitação em Fábrica)
* **IHM:** Interface Homem-Máquina
* **IoT:** Internet of Things (Internet das Coisas)
* **MTBF:** Mean Time Between Failures (Tempo Médio Entre Falhas)
* **MTTR:** Mean Time to Repair (Tempo Médio Para Reparo)
* **NR:** Norma Regulamentadora Brasileira
* **OEE:** Overall Equipment Effectiveness (Eficiência Global do Equipamento)
* **OPC UA:** Open Platform Communications Unified Architecture
* **PCP:** Planejamento e Controle da Produção
* **PERT:** Program Evaluation and Review Technique
* **PMBOK:** Project Management Body of Knowledge
* **PMO:** Project Management Office (Escritório de Gerenciamento de Projetos)
* **POP:** Procedimento Operacional Padrão
* **QA / QC:** Quality Assurance / Quality Control (Garantia e Controle da Qualidade)
* **RACI:** Responsible, Accountable, Consulted, Informed
* **RNC:** Relatório de Não Conformidade
* **SAT:** Site Acceptance Test (Teste de Aceitação em Campo)
* **SIGAI:** Sistema Integrado de Automação e Gestão Industrial
* **SPI:** Schedule Performance Index (Índice de Desempenho de Prazos)
* **TAP:** Termo de Abertura do Projeto (Project Charter)

---

## SUMÁRIO

1. **INTRODUÇÃO**
   - 1.1 Contextualização do Problema
   - 1.2 Justificativa e Objetivos
   - 1.3 Metodologia Utilizada
2. **GERENCIAMENTO DA INTEGRAÇÃO**
   - 2.1 Estrutura e Direcionamento do Portfólio
   - 2.2 Integração entre Portfólio, Programas e Projetos
   - 2.3 Termo de Abertura do Projeto (TAP)
3. **GERENCIAMENTO DO ESCOPO**
   - 3.1 Definição do Escopo e Entregas
   - 3.2 Estrutura Analítica do Projeto (EAP) e Dicionário
   - 3.3 Critérios de Aceitação e Controle de Mudanças
4. **GERENCIAMENTO DO CRONOGRAMA**
   - 4.1 Sequenciamento das Atividades e Estimativas PERT
   - 4.2 Cronograma em Rede e Caminho Crítico
   - 4.3 Roadmap do Portfólio e Marcos de Entrega
5. **GERENCIAMENTO DOS CUSTOS**
   - 5.1 Estimativa e Distribuição dos Custos (CAPEX e OPEX)
   - 5.2 Orçamento Consolidado e Linha de Base (Curva S)
   - 5.3 Metodologia de Controle por Valor Agregado (EVM)
6. **GERENCIAMENTO DA QUALIDADE**
   - 6.1 Critérios e Indicadores de Qualidade (Normas e Padrões)
   - 6.2 Garantia e Controle da Qualidade (QA/QC, FAT e SAT)
   - 6.3 Tratamento de Não Conformidades (RNC)
7. **GERENCIAMENTO DOS RECURSOS**
   - 7.1 Identificação de Recursos e Matriz RACI
   - 7.2 Alocação e Resolução de Conflitos de Recursos
8. **GERENCIAMENTO DAS COMUNICAÇÕES**
   - 8.1 Matriz de Comunicação 5W2H
   - 8.2 Engajamento e Gestão de Conflitos
9. **GERENCIAMENTO DOS RISCOS**
   - 9.1 Identificação e Análise Qualitativa/Quantitativa (5x5)
   - 9.2 Planos de Resposta, Contingência e Donos de Risco
10. **GERENCIAMENTO DAS AQUISIÇÕES**
    - 10.1 Estratégia de "Fazer ou Comprar" (*Make or Buy*)
    - 10.2 Seleção de Fornecedores e Administração Contratual
11. **GERENCIAMENTO DAS PARTES INTERESSADAS**
    - 11.1 Identificação e Matriz Poder × Interesse
    - 11.2 Estratégias de Engajamento Operacional
12. **RESULTADOS E DISCUSSÃO**
    - 12.1 Análise de Impacto nos 4 Objetivos Estratégicos
    - 12.2 Comparativo da Situação Anterior vs. Situação Projetada
13. **CONSIDERAÇÕES FINAIS E LIÇÕES APRENDIDAS**
14. **REFERÊNCIAS BIBLIOGRÁFICAS**

---

## 1. INTRODUÇÃO

### 1.1 Contextualização do Problema
No ambiente industrial contemporâneo, a manufatura avançada e a transformação digital impõem padrões rigorosos de produtividade, eficiência energética e tolerância zero a falhas. A empresa **MetalTech S.A.**, fabricante de autopeças e estruturas metálicas para máquinas industriais, deparou-se com limitações operacionais severas em sua principal linha de produção (Linha 1). A coleta de parâmetros de fabricação (como temperatura de corte, vibração de fusos e contagem volumétrica) ocorria por meio de fichas físicas preenchidas manualmente pelos operadores ao final de cada turno.

Esse método arcaico acarretava três problemas centrais:
1. **Defasagem Decisória:** Informações sobre quebras ou desvios de tolerância levavam até 24 horas para serem consolidadas no PCP.
2. **Elevado Custo de Sucata:** O índice de refugo de matéria-prima atingia 8% do volume faturado, em virtude da identificação tardia de desgastes de ferramentas.
3. **Paradas Críticas Não Programadas:** As quebras de rolamentos e sistemas hidráulicos paralisavam a linha por até 60 horas mensais, frustrando contratos comerciais com montadoras.

### 1.2 Justificativa e Objetivos
Diante desse diagnóstico, a diretoria executiva deliberou a necessidade de alocar investimentos de modernização nos próximos 12 meses. O objetivo geral deste trabalho é apresentar uma solução estruturada de gestão de portfólio, seleção de investimentos e planejamento integrado de engenharia para viabilizar as quatro metas corporativas estabelecidas:
* **Aumentar a produtividade** em **+15%**;
* **Reduzir as paradas de produção** em **-20%**;
* **Reduzir os custos operacionais** em **-10%**;
* **Reduzir o retrabalho** em **-30%**.

Tudo isso respeitando um teto financeiro de **R$ 2.500.000,00** e uma equipe interna de 7 especialistas (2 Engenheiros de Automação, 2 Analistas de TI, 1 Especialista em Qualidade, 1 Especialista em Manutenção e 1 Gerente de Projetos).

### 1.3 Metodologia Utilizada
A metodologia de desenvolvimento integrou as dez áreas de conhecimento preconizadas pelo Guia PMBOK (6ª e 7ª edições), aliadas ao framework ágil Scrum para gestão do fluxo diário das equipes. Empregaram-se técnicas de decisão multicritério para ranqueamento do portfólio, estimativas paramétricas e de três pontos (PERT) para cálculo de durações, diagramação em rede de precedências para determinação do caminho crítico (CPM), orçamento por linha de base analítica com acompanhamento por Valor Agregado (EVM), matriz de probabilidade e impacto 5x5 para análise de riscos e protocolos estruturados de controle de qualidade (FAT e SAT).

---

## 2. GERENCIAMENTO DA INTEGRAÇÃO

### 2.1 Estrutura e Direcionamento do Portfólio
O portfólio da MetalTech S.A. foi estruturado a partir da premissa de que investimentos isolados em maquinário sem a devida infraestrutura de dados e capacitação humana fracassam. Foram avaliados 8 projetos disponíveis:
- `P1` (Automação da Linha 1 — R$ 900k | 6m | Risco Alto);
- `P2` (Manutenção Preditiva — R$ 450k | 4m | Risco Médio);
- `P3` (Novo ERP Industrial — R$ 1,2M | 10m | Risco Alto);
- `P4` (Redução de Refugo — R$ 250k | 3m | Risco Baixo);
- `P5` (Modernização da Qualidade — R$ 350k | 4m | Risco Médio);
- `P6` (Treinamento de Operadores — R$ 150k | 2m | Risco Baixo);
- `P7` (Monitoramento IoT — R$ 600k | 5m | Risco Médio);
- `P8` (Expansão da Capacidade — R$ 1,5M | 12m | Risco Alto).

### 2.2 Integração entre Portfólio, Programas e Projetos
Para capturar sinergias e evitar conflitos de recursos humanos, o PMO organizou as iniciativas em dois programas estruturantes:
1. **Programa 1: Excelência Operacional & Manufatura Confiável** (P1 + P2 + P6 — Subtotal: R$ 1.500.000,00);
2. **Programa 2: Qualidade Integrada & Desperdício Zero** (P4 + P5 — Subtotal: R$ 600.000,00);
3. **Reserva Estratégica de Contingência do Portfólio:** R$ 400.000,00 (16% do orçamento total blindado contra riscos cambiais);
4. **Fase 2 (Posterior — Ano 2):** Projetos P7 (IoT) e P3 (ERP);
5. **Iniciativa Adiada:** Projeto P8 (Expansão de Capacidade).

Essa arquitetura consome R$ 2,1 milhões em execuções no Ano 1, garantindo que 100% dos 4 objetivos estratégicos sejam atendidos e mitigando riscos sistêmicos.

### 2.3 Termo de Abertura do Projeto (TAP) — Síntese do SIGAI
Como projeto estruturante de maior envergadura dentro do Programa 1, desenvolveu-se o planejamento integral do **Sistema Integrado de Automação e Gestão Industrial (SIGAI)**. O TAP formalizou Giovani Miamoto como Gerente de Projeto, fixou o orçamento de R$ 1.500.000,00 e estabeleceu o prazo de conclusão em 10 meses (fevereiro a novembro de 2026), tendo como patrocinador formal o Diretor Industrial Carlos Eduardo Albuquerque.

---

## 3. GERENCIAMENTO DO ESCOPO

### 3.1 Definição do Escopo e Entregas
O escopo compreende o sensoriamento industrial completo de 16 centros de usinagem e prensas da Linha 1, infraestrutura de fibra óptica, painéis elétricos com nobreaks, servidores industriais em DMZ, middleware de integração OPC UA, IHM touch para apontamento operacional em campo e dashboard web de OEE e rastreabilidade metrológica. As exclusões explícitas (não-escopo) garantiram que as linhas 2, 3 e 4 e obras civis do galpão fossem protegidas contra solicitações informais de acréscimo.

### 3.2 Estrutura Analítica do Projeto (EAP)
A EAP foi concebida orientada a entregas verificáveis, desdobrada em 6 macrocomponentes e 20 pacotes de trabalho (conforme detalhado no arquivo analítico `03-escopo-e-eap.md`). Cada pacote possui descrição pormenorizada no Dicionário da EAP, associando critérios mensuráveis de aceitação.

### 3.3 Critérios de Aceitação e Controle de Mudanças
Nenhuma entrega é homologada sem evidência de laudo técnico ou teste operacional formal. As solicitações de modificação seguem o fluxo rígido do Comitê de Controle de Mudanças (CCB), exigindo aprovação do Sponsor para qualquer desvio superior a R$ 10.000,00 ou 5 dias úteis de cronograma.

---

## 4. GERENCIAMENTO DO CRONOGRAMA

### 4.1 Sequenciamento das Atividades e Estimativas PERT
A decomposição do trabalho resultou em 18 macroatividades interdependentes. Utilizou-se o método PERT de 3 pontos para calcular durações esperadas, mitigando o otimismo ingênuo em tarefas de engenharia de campo e programação.

### 4.2 Cronograma em Rede e Caminho Crítico (CPM)
O caminho crítico foi rigorosamente mapeado:
$$\text{Requisitos (A02)} \rightarrow \text{Projeto Elétrico (A03)} \rightarrow \text{Fibra Óptica (A05)} \rightarrow \text{Painéis (A06)} \rightarrow \text{Sensores (A07)} \rightarrow \text{OPC UA (A09)} \rightarrow \text{Dashboard (A11)} \rightarrow \text{FAT (A12)} \rightarrow \text{SAT (A13)} \rightarrow \text{Metrologia (A14)} \rightarrow \text{Treinamento (A16)} \rightarrow \text{Operação Assistida (A17)} \rightarrow \text{Aceite (A18)}$$
A duração total do caminho crítico soma 214 dias úteis (10 meses corridos), com término fixado em 30 de novembro de 2026.

### 4.3 Roadmap e Marcos Estratégicos
O escalonamento trimestral garantiu "Quick Wins":
- **M1 (Fev/26):** Planejamento Consolidado e TAP Aprovado.
- **M2 (Mai/26):** Infraestrutura Física e Fibra Óptica Prontas.
- **M3 (Jul/26):** Software OPC UA Homologado em Bancada (FAT).
- **M4 (Ago/26):** Linha 1 Comissionada com Carga (SAT) e Início da Operação Assistida.
- **M5 (Nov/26):** Aceite Definitivo e Homologação das Metas Estratégicas.

---

## 5. GERENCIAMENTO DOS CUSTOS

### 5.1 Estimativa e Distribuição dos Custos
O custo foi estruturado por meio de precificação *bottom-up*:
* **Recursos Humanos:** R$ 480.000,00 (37,5%)
* **Hardware e Equipamentos:** R$ 460.000,00 (35,9%)
* **Software e Servidores:** R$ 180.000,00 (14,1%)
* **Serviços Terceiros e Auditoria:** R$ 160.000,00 (12,5%)
* **Custo Base da Baseline:** **R$ 1.280.000,00**
* **Reservas de Governança:** R$ 128.000,00 (Contingência) + R$ 92.000,00 (Gerencial)
* **Orçamento Total Autorizado (BAC):** **R$ 1.500.000,00**

### 5.2 Linha de Base dos Custos (Curva S)
A curva de desembolso acumulado reflete um perfil sigmoidal típico de projetos de engenharia: desembolsos moderados no início (M1 a M2), forte concentração financeira nos meses de aquisição e instalação física (M3 a M5) e estabilização suave na fase de homologação e operação assistida (M6 a M10).

### 5.3 Gerenciamento do Valor Agregado (EVM)
Adotou-se o acompanhamento por EVM, com medições mensais de $PV, EV, AC, CPI$ e $SPI$. Fixou-se a regra de que variações superiores a 10% nos índices de desempenho demandam abertura imediata de relatório de análise de desvios e plano de recuperação.

---

## 6. GERENCIAMENTO DA QUALIDADE

### 6.1 Critérios e Indicadores de Qualidade
A qualidade técnica do projeto apoia-se em quatro pilares normativos:
- **ISO 9001:2015:** Padronização de processos e rastreabilidade total de componentes.
- **IATF 16949:2016:** Aderência às diretrizes automotivas de zero defeito.
- **ISO/IEC 25010:** Modelo de qualidade de software (latência $\le 1\text{s}$, disponibilidade $\ge 99,8\%$).
- **Normas NR-10 e NR-12:** Segurança estrita nas instalações elétricas e mecânicas.

### 6.2 Garantia e Controle da Qualidade (QA/QC)
Estabeleceu-se uma política de testes em duas camadas: os ensaios **FAT** (Factory Acceptance Test) em bancada de laboratório para validação lógica preliminar e os ensaios **SAT** (Site Acceptance Test) em condições reais de carga fabril por 8 horas ininterruptas. Sensores dimensionais contam com laudo de calibração credenciado pela Rede Brasileira de Calibração (RBC).

### 6.3 Tratamento de Não Conformidades (RNC)
O processo formal de RNC estabelece fluxo de contenção imediata em caso de falha, análise de causa raiz pelo método dos 5 Porquês e reteste obrigatório antes da liberação do lote de produção.

---

## 7. GERENCIAMENTO DOS RECURSOS

### 7.1 Identificação de Recursos e Matriz RACI
O quadro de especialistas foi mapeado funcionalmente através da Matriz de Responsabilidades RACI (Responsible, Accountable, Consulted, Informed), assegurando que cada uma das 18 atividades possua exatamente um único responsável final pela aprovação ("A"), eliminando ambiguidades e conflitos de autoridade.

### 7.2 Alocação e Resolução de Conflitos
O PMO solucionou dois gargalos críticos de recursos:
1. **Engenheiros de Automação (EA1 e EA2):** Escalonou-se a dedicação para que EA1 concluísse a instrumentação preditiva (P2) no primeiro trimestre, unindo-se integralmente a EA2 a partir do quarto mês para a montagem de P1.
2. **Especialista em Qualidade (EQ1):** EQ1 liderou a redução de refugo (P4) nos meses 1 a 3 e, com o projeto estabilizado, assumiu 100% da modernização metrológica (P5) a partir do mês 4.

---

## 8. GERENCIAMENTO DAS COMUNICAÇÕES

### 8.1 Matriz de Comunicação 5W2H
O plano de comunicação estruturou canais adequados para cada audiência:
- Daily Standup matinal de 15 minutos para a equipe técnica no chão de fábrica;
- Status Report executivo mensal em PDF de 1 página e dashboard Power BI para a diretoria;
- Boletim quinzenal impresso e audiovisual "Fábrica Digital" para engajar operadores e manutenção.

### 8.2 Engajamento e Gestão de Conflitos
Definiu-se uma matriz de escalação em 3 níveis (Operacional até 24h, Tático até 48h e Estratégico/Sponsor imediato), mitigando ruídos antes que se tornem atritos interdepartamentais.

---

## 9. GERENCIAMENTO DOS RISCOS

### 9.1 Identificação e Análise Qualitativa e Quantitativa (5x5)
Mapearam-se 10 riscos essenciais categorizados em técnicos, fornecedores, humanos, operacionais e financeiros. A matriz de severidade 5x5 destacou como riscos de alta prioridade: o atraso na entrega de sensores importados ($S=12$), a resistência cultural de operadores ($S=12$) e a incompatibilidade em CLPs antigos da fábrica ($S=12$).

### 9.2 Planos de Resposta, Contingência e Donos de Risco
Cada risco prioritário recebeu um plano de ação preventiva e um plano de contingência engatilhado por métricas objetivas. Os custos de mitigação e potenciais contingências foram suportados pela Reserva de Contingência de R$ 128.000,00.

---

## 10. GERENCIAMENTO DAS AQUISIÇÕES

### 10.1 Estratégia de "Fazer ou Comprar" (*Make or Buy*)
Adotou-se a estratégia híbrida: o desenvolvimento do software de supervisão, lógica de controle e integração OPC UA foi desenvolvido internamente (*Make*), retendo o conhecimento estratégico na MetalTech S.A. Já o lançamento e fusão de fibra óptica e a certificação metrológica RBC foram contratados de terceiros especializados (*Buy*).

### 10.2 Contratos e Gestão de Fornecedores
As aquisições foram formalizadas sob modalidade de Preço Fixo (*Firm Fixed Price — FFP*) com retenção técnica de 10% do valor até a homologação final dos testes SAT, assegurando o cumprimento dos SLAs acordados.

---

## 11. GERENCIAMENTO DAS PARTES INTERESSADAS

### 11.1 Identificação e Matriz Poder × Interesse
Oito grupos de partes interessadas foram caracterizados. O Diretor Industrial figurou no quadrante de alto poder e alto interesse ("Gerenciar de Perto"), enquanto operadores de chão de fábrica foram posicionados em baixo poder e alto interesse ("Manter Informado e Capacitar").

### 11.2 Estratégias de Engajamento
A resistência à digitalização foi neutralizada com a criação do programa "Operador 4.0", valorizando os colaboradores por meio de treinamentos presenciais e demonstrando que o sistema SIGAI elimina tarefas manuais repetitivas e cansativas de preenchimento de papel.

---

## 12. RESULTADOS E DISCUSSÃO

### 12.1 Análise de Impacto nos 4 Objetivos Estratégicos
A execução simulada do planejamento e a operação assistida evidenciaram resultados plenamente aderentes às diretrizes corporativas:

| Objetivo Estratégico | Meta Fixada | Resultado Projetado pelo Plano | Status de Cumprimento |
|---|:---:|:---:|:---:|
| ⚙️ **Aumento de Produtividade** | **+15,0%** | **+15,5%** (Automação Linha 1 + Capacitação P6) | 🟢 **Atingida com Superávit** |
| 🛠️ **Redução de Paradas de Produção** | **-20,0%** | **-22,0%** (Manutenção Preditiva P2 + Sensores) | 🟢 **Atingida com Superávit** |
| 📉 **Redução de Custos Operacionais** | **-10,0%** | **-12,4%** (Refugo P4 + Otimização de Máquinas) | 🟢 **Atingida com Superávit** |
| 🎯 **Redução de Retrabalho** | **-30,0%** | **-31,2%** (Inspeção Óptica P5 + POPs) | 🟢 **Atingida com Superávit** |

### 12.2 Comparativo da Situação Anterior vs. Situação Projetada
- **Apontamento de Produção:** De fichas de papel preenchidas a cada 8 horas para telemetria automatizada em tempo real (atualização a cada 1 segundo).
- **Rastreabilidade de Componentes:** De controle por amostragem em lote para rastreabilidade serial unitária via código DataMatrix.
- **Confiabilidade da Linha:** MTBF elevado de 42 horas para mais de 120 horas contínuas de operação.

---

## 13. CONSIDERAÇÕES FINAIS E LIÇÕES APRENDIDAS

O desenvolvimento deste trabalho técnico-acadêmico demonstrou na prática que a excelência em gerenciamento de projetos não reside apenas no cumprimento burocrático de ferramentas, mas na capacidade de integrar decisões de negócio, engenharia e comportamento humano em torno de metas claras.

A proposta de portfólio formulada para a **MetalTech S.A.** e o detalhamento do **Projeto SIGAI** comprovam que é possível executar transformações industriais complexas dentro de restrições severas de orçamento e equipe, desde que haja método, planejamento temporal e governança de riscos. As principais lições aprendidas incluem a importância do engajamento prévio dos operadores de chão de fábrica, a necessidade de reservas de contingência financeiras para absorver oscilações cambiais e a relevância de padronizar procedimentos operacionais antes de implementar softwares de gestão. 

A MetalTech S.A. encerra o ciclo de 12 meses não apenas com as quatro metas superadas, mas com alicerces tecnológicos e organizacionais prontos para receber o Programa de Transformação Digital (IoT e ERP) no próximo ano.

---

## 14. REFERÊNCIAS BIBLIOGRÁFICAS

1. **PROJECT MANAGEMENT INSTITUTE (PMI).** *A Guide to the Project Management Body of Knowledge (PMBOK Guide)*. 6. ed. Newtown Square: Project Management Institute, 2017.
2. **PROJECT MANAGEMENT INSTITUTE (PMI).** *The Standard for Portfolio Management*. 4. ed. Newtown Square: Project Management Institute, 2017.
3. **CARVALHO, Fábio Câmara Araújo de.** *Gestão de Projetos*. 2. ed. São Paulo: Pearson, 2018.
4. **SOUZA, Carla Patricia da Silva.** *Gestão de Projetos*. Curitiba: Contentus, 2020.
5. **FINOCCHIO JÚNIOR, José.** *Project Model Canvas: gerenciamento de projetos sem burocracia*. São Paulo: Saraiva, 2013.
6. **SUTHERLAND, Jeffrey.** *Scrum: a arte de fazer o dobro do trabalho na metade do tempo*. São Paulo: Leya, 2014.
7. **ASSOCIAÇÃO BRASILEIRA DE NORMAS TÉCNICAS (ABNT).** *NBR ISO 9001: Sistemas de gestão da qualidade — Requisitos*. Rio de Janeiro: ABNT, 2015.
8. **INTERNATIONAL ORGANIZATION FOR STANDARDIZATION (ISO).** *ISO/IEC 25010: Systems and software engineering — Systems and software Quality Requirements and Evaluation (SQReA)*. Genebra: ISO, 2011.
9. **INTERNATIONAL AUTOMOTIVE TASK FORCE (IATF).** *IATF 16949: Quality management system requirements for automotive production*. IATF, 2016.
10. **MINISTÉRIO DO TRABALHO E EMPREGO (MTE).** *Norma Regulamentadora nº 10 (Segurança em Instalações e Serviços em Eletricidade)* e *Norma Regulamentadora nº 12 (Segurança no Trabalho em Máquinas e Equipamentos)*. Brasília: MTE, 2022.
