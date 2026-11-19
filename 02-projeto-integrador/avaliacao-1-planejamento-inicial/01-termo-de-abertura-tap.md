# 📜 Termo de Abertura do Projeto (TAP) — Project Charter

**Documento Referência:** Padrão PMBOK / Modelo Institucional UniSENAI-SP  
**Status do Documento:** Aprovado  
**Versão:** 1.0  
**Data de Aprovação:** 15/01/2026  

---

## 1. Identificação Geral do Projeto

| Campo | Informação |
|---|---|
| **Título do Projeto** | Implantação do Sistema Integrado de Automação e Gestão Industrial (SIGAI) |
| **Código do Projeto** | PRJ-MT-2026-01 |
| **Organização Executora** | MetalTech S.A. — Planta Fabril de Componentes Metalmecânicos |
| **Sponsor / Patrocinador** | Carlos Eduardo Albuquerque (Diretor Industrial) |
| **Gerente do Projeto** | Giovani Miamoto (Gerente de Projetos de TI / ADS) |
| **Comitê Diretivo / Stakeholders-Chave** | Diretoria de TI, Gerência de Manutenção, Gerência da Qualidade e Gerência de RH |
| **Data Prevista de Início** | 01/02/2026 |
| **Data Prevista de Término** | 30/11/2026 (10 meses) |
| **Orçamento Global Aprovado** | R$ 1.500.000,00 |

---

## 2. Contextualização e Justificativa do Projeto

A **MetalTech S.A.** atua no fornecimento de componentes metálicos de alta precisão para montadoras de veículos e bens de capital. Historicamente, os dados de chão de fábrica (contagem de peças usinadas, paradas de prensas, medições de tolerância dimensional e consumo elétrico) são coletados por fichas manuais de papel ou planilhas descentralizadas, gerando defasagem de até 24 horas para tomada de decisão gerencial.

Esse cenário acarreta:
1. **Perdas por Paradas Ocultas:** Atraso no acionamento da manutenção em quebras iminentes de fusos e servomotores.
2. **Elevado Índice de Retrabalho:** Peças fora de especificação só são detectadas no fim do lote, gerando 8% de refugo de ligas metálicas nobres.
3. **Falta de Rastreabilidade:** Exigência contratual de montadoras de rastrear lote de matéria-prima, operador e máquina associada a cada peça estampada.

A implantação do **SIGAI** se justifica pela necessidade estratégica de elevar a disponibilidade das linhas, eliminar apontamentos manuais, integrar dados em tempo real ao PCP (Planejamento e Controle da Produção) e garantir conformidade com os padrões da Indústria 4.0.

---

## 3. Objetivos do Projeto (Metas SMART)

* **Objetivo Geral:**  
  Desenvolver, integrar e comissionar uma plataforma tecnológica unificada (hardware industrial e software) conectando 100% dos maquinários da Linha 1 de Usinagem aos sistemas de monitoramento em tempo real, controle de qualidade e gestão da produção da MetalTech S.A.

* **Objetivos Específicos (Critérios SMART):**
  1. **Produtividade:** Aumentar a disponibilidade operacional da Linha 1 em no mínimo **15%** até o 8º mês de implantação.
  2. **Qualidade e Retrabalho:** Reduzir o retrabalho em **30%** e o refugo em **25%** por meio de postos de inspeção automatizados até o 9º mês.
  3. **Tempo de Resposta à Manutenção:** Reduzir o tempo médio de reparo (MTTR) em **20%** com alertas preditivos automáticos integrados em menos de 10 segundos da anomalia.
  4. **Digitalização:** Eliminar 100% dos formulários físicos de apontamento de chão de fábrica na Linha 1 até o encerramento do projeto.

---

## 4. Requisitos de Alto Nível e Principais Entregas

### Requisitos Funcionais e Técnicos:
- Coleta automática de telemetria de 12 centros de usinagem CNC e 4 prensas via protocolo industrial (OPC UA / Modbus TCP).
- Dashboard gerencial web responsivo para monitoramento de OEE (Overall Equipment Effectiveness) em tempo real.
- Módulo de rastreabilidade com leitura por código DataMatrix impresso nas peças metálicas.
- Integração bidirecional de ordens de produção e estoque de matéria-prima com a base de dados corporativa.

### Principais Entregas (Milestones):
- **E1:** Documentação de Engenharia e Especificação Técnica de Requisitos Aprovada.
- **E2:** Infraestrutura de Rede Industrial Cabeada (Fibra Óptica / Switch Industrial) e Sensores Instalados.
- **E3:** Módulos de Software (Backend, IHM de Chão de Fábrica e Dashboard OEE) Desenvolvidos e Homologados.
- **E4:** Linha-Piloto Comissionada e Testes de Carga Validados.
- **E5:** Equipe de Operadores e Manutentores Certificada (100% dos turnos).
- **E6:** Termo de Aceite Final Assinado e Transição para Operação Assistida.

---

## 5. Limites do Projeto (Escopo e Não-Escopo)

* **Dentro do Escopo:**
  - Toda a instrumentação, sensoriamento e rede industrial dos 16 maquinários da Linha 1.
  - Desenvolvimento e parametrização do software de supervisão de chão de fábrica.
  - Treinamento presencial de 4 turmas de operadores (turnos A, B, C e manutenção).
  - 60 dias de operação assistida pós-comissionamento.

* **Fora do Escopo (Não-Escopo):**
  - Automação das Linhas 2, 3 e 4 (objeto de fases contratuais futuras).
  - Aquisição de novos centros de usinagem ou expansão predial da fábrica.
  - Substituição total do sistema contábil/financeiro corporativo da empresa.

---

## 6. Premissas e Restrições Estratégicas

### Premissas:
1. O fornecedor de sensores ópticos e gateways industriais entregará os equipamentos em até 45 dias da emissão da ordem de compra.
2. A fábrica disponibilizará paradas programadas de fim de semana (sábado à noite / domingo) para instalação física dos painéis elétricos, sem impactar o plano de faturamento.
3. Os analistas de TI e engenheiros de automação internos terão dedicação garantida de 50% de sua jornada nas fases de integração.

### Restrições:
1. **Orçamentária:** Teto intransponível de R$ 1.500.000,00, incluindo 15% de reserva de contingência.
2. **Temporal:** Entrada em operação comercial mandatória antes do pico de demanda automotiva de final de ano (limite: 30 de novembro).
3. **Normativa:** Estrita observância às normas regulamentadoras brasileiras NR-10 (Segurança em Instalações Elétricas) e NR-12 (Segurança no Trabalho em Máquinas e Equipamentos).

---

## 7. Equipe Inicial, Responsabilidades e Autoridade do Gerente de Projeto

| Papel no Projeto | Profissional Designado | Área / Função |
|---|---|---|
| **Patrocinador Executivo (Sponsor)** | Carlos Eduardo Albuquerque | Diretor Industrial |
| **Gerente do Projeto** | Giovani Miamoto | PMO / Liderança Técnica do Projeto |
| **Líder Técnico de Automação** | Eng. Roberto Mendes | Engenharia de Automação Industrial |
| **Líder de Arquitetura de Software** | Luciana Silveira | Analista de Sistemas / TI |
| **Líder de Garantia da Qualidade** | Fernando Prado | Especialista em Qualidade e Metrologia |
| **Líder de Manutenção e Confiabilidade** | Marcos Barreto | Manutenção Industrial |

### Limites de Autoridade do Gerente de Projeto (Giovani Miamoto):
- **Autoridade Financeira:** Autorizar despesas orçadas até R$ 50.000,00 por evento sem necessidade de aprovação prévia do Sponsor. Variações acima deste teto requerem aval do Comitê.
- **Autoridade de Pessoal:** Definir a distribuição diária de tarefas técnicas e requisitar apoio de consultoria externa prevista no plano.
- **Autoridade de Escopo:** Recusar solicitações informais de mudanças que ameacem o cronograma ou o orçamento, direcionando-as formalmente ao Comitê de Controle de Mudanças (CCB).

---

## 8. Aprovação Formal

| Aprovador | Cargo | Data | Assinatura |
|---|---|:---:|:---:|
| **Carlos Eduardo Albuquerque** | Diretor Industrial (Sponsor) | 15/01/2026 | *[Assinado]* |
| **Giovani Miamoto** | Gerente do Projeto | 15/01/2026 | *[Assinado]* |
