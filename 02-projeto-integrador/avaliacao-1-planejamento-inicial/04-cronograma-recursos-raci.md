# 📅 Cronograma, Recursos e Matriz de Responsabilidades (RACI)

**Projeto:** Sistema Integrado de Automação e Gestão Industrial (SIGAI) — MetalTech S.A.  
**Área do Conhecimento:** Gerenciamento do Cronograma e Recursos (PMBOK / UniSENAI-SP)  
**Versão:** 1.0 | **Data de Elaboração:** Fevereiro de 2026  

---

## 1. Decomposição das Atividades e Estimativas de Duração (PERT)

Para garantir precisão e confiabilidade nas datas, as durações foram estimadas utilizando o método **PERT de Três Pontos** (Estimativa Otimista $O$, Mais Provável $M$ e Pessimista $P$), calculando a Duração Esperada pela fórmula ponderada:
$$TE = \frac{O + 4M + P}{6}$$

### 📋 Tabela de Atividades, Dependências e Caminho Crítico

| ID | Pacote EAP | Descrição da Atividade | Pré-requisito (Dep.) | O (dias) | M (dias) | P (dias) | TE (dias úteis) | Responsável Principal | Caminho Crítico? |
|:---:|:---:|---|:---:|:---:|:---:|:---:|:---:|---|:---:|
| **A01** | 1.1 | Elaboração do TAP e Plano Integrado de Projeto | — | 7 | 10 | 19 | **11** | Gerente de Projetos (Giovani) | **SIM** |
| **A02** | 2.1 | Levantamento de Requisitos Técnicos de Automação e TI | A01 | 10 | 15 | 26 | **16** | Líder de Automação / TI | **SIM** |
| **A03** | 2.2 | Projeto Executivo Elétrico, Topologia de Rede e CAD | A02 | 10 | 14 | 24 | **15** | Eng. Automação | **SIM** |
| **A04** | 2.3 | Cotação, Homologação e Emissão de Ordens de Compra | A02 | 12 | 18 | 30 | **19** | Compras / GP | NÃO |
| **A05** | 3.1 | Instalação de Eletrocalhas e Anel de Fibra Óptica | A03, A04 | 15 | 20 | 31 | **21** | Infraestrutura / TI | **SIM** |
| **A06** | 3.2 | Montagem Física e Ligação dos Painéis Elétricos de Campo | A05 | 10 | 15 | 26 | **16** | Eng. Automação / Manutenção | **SIM** |
| **A07** | 3.3 | Instalação Física de Sensores e Câmeras DataMatrix | A06 | 8 | 12 | 22 | **13** | Manutenção / Automação | **SIM** |
| **A08** | 4.1 | Provisionamento de Servidores, Docker e Banco de Dados | A03 | 5 | 8 | 17 | **9** | Analista de TI | NÃO |
| **A09** | 4.2 | Desenvolvimento da Camada de Comunicação OPC UA | A07, A08 | 15 | 22 | 35 | **23** | Analista de TI / Automação | **SIM** |
| **A10** | 4.3 | Construção das Telas de IHM Touch de Chão de Fábrica | A02 | 14 | 20 | 32 | **21** | Analista de TI / Design | NÃO |
| **A11** | 4.4 | Desenvolvimento do Dashboard Web de OEE e Relatórios | A09, A10 | 18 | 25 | 38 | **26** | Analista de TI | **SIM** |
| **A12** | 5.1 | Testes de Bancada e Simulação Lógica (FAT) | A11 | 8 | 10 | 18 | **11** | Garantia da Qualidade / Automação | **SIM** |
| **A13** | 5.2 | Teste Integrado com Carga na Linha 1 (SAT) | A12 | 6 | 8 | 16 | **9** | Operações / Manutenção / TI | **SIM** |
| **A14** | 5.3 | Auditoria Metrológica e Confiabilidade dos Sensores | A13 | 5 | 7 | 15 | **8** | Garantia da Qualidade | **SIM** |
| **A15** | 6.1 | Homologação de Manuais Técnicos e POPs Operacionais | A11 | 6 | 8 | 16 | **9** | Qualidade / RH | NÃO |
| **A16** | 6.2 | Capacitação Prática das 4 Turmas de Operadores | A14, A15 | 8 | 10 | 18 | **11** | RH / Automação / Operações | **SIM** |
| **A17** | 6.3 | Operação Assistida em Tempo Real (60 Dias Corridos) | A16 | 38 | 42 | 52 | **43** | GP / TI / Manutenção | **SIM** |
| **A18** | 6.4 | Homologação de Encerramento e Termo de Aceite | A17 | 4 | 5 | 12 | **6** | Sponsor / GP | **SIM** |

---

## 2. Gráfico de Gantt do Projeto (Diagrama Visual Mermaid)

```mermaid
gantt
    title Cronograma Executivo do Projeto SIGAI - Linha de Base
    dateFormat  YYYY-MM-DD
    axisFormat  %b/%y

    section 1. Iniciação e Requisitos
    A01 Elaboração do TAP e Plano Integrado      :crit, a01, 2026-02-02, 2026-02-16
    A02 Requisitos Técnicos de Automação e TI   :crit, a02, after a01, 16d
    A03 Projeto Executivo Elétrico e Redes       :crit, a03, after a02, 15d
    A04 Compras de Sensores e Roteadores         :a04, after a02, 19d

    section 2. Infraestrutura e Campo
    A05 Instalação do Anel de Fibra Óptica      :crit, a05, after a03, 21d
    A06 Montagem dos Painéis Elétricos           :crit, a06, after a05, 16d
    A07 Fixação de Sensores e Leitores           :crit, a07, after a06, 13d

    section 3. Software e Integração
    A08 Servidores e Banco de Dados              :a08, after a03, 9d
    A09 Camada de Comunicação OPC UA             :crit, a09, after a07, 23d
    A10 Telas de IHM para Chão de Fábrica        :a10, after a02, 21d
    A11 Dashboard OEE e Rastreabilidade          :crit, a11, after a09, 26d

    section 4. Testes e Validação
    A12 Testes de Bancada FAT                    :crit, a12, after a11, 11d
    A13 Teste Integrado com Carga SAT            :crit, a13, after a12, 9d
    A14 Auditoria Metrológica de Qualidade       :crit, a14, after a13, 8d

    section 5. Transição e Aceite
    A15 Manuais e Procedimentos POP              :a15, after a11, 9d
    A16 Capacitação dos Operadores               :crit, a16, after a14, 11d
    A17 Operação Assistida (60 dias)             :crit, a17, after a16, 43d
    A18 Aceite Final e Encerramento              :crit, a18, after a17, 6d

    section Marcos Estratégicos
    Marco 1: Planejamento Aprovado               :milestone, m1, 2026-02-16, 0d
    Marco 2: Infraestrutura Física Pronta        :milestone, m2, 2026-05-15, 0d
    Marco 3: Software Homologado em Bancada      :milestone, m3, 2026-07-20, 0d
    Marco 4: Linha 1 Comissionada SAT            :milestone, m4, 2026-08-25, 0d
    Marco 5: Aceite Definitivo e Encerramento    :milestone, m5, 2026-11-30, 0d
```

---

## 3. Marcos Principais do Projeto (Milestones)

| Marco | Data Prevista | Critério Técnico de Validação |
|---|:---:|---|
| 🚩 **M1: Planejamento Consolidado** | 16/02/2026 | TAP e Planos de Gestão assinados pelo Sponsor e Comitê. |
| 🚩 **M2: Infraestrutura de Campo Pronta** | 15/05/2026 | Rede de fibra certificada e 100% dos painéis energizados e testados. |
| 🚩 **M3: Software e Telemetria Integrados** | 20/07/2026 | Coleta de dados via OPC UA operando continuamente em bancada FAT. |
| 🚩 **M4: Linha 1 Comissionada (SAT)** | 25/08/2026 | Operação de 8 horas consecutivas com apontamento automático e OEE em tempo real. |
| 🚩 **M5: Encerramento e Aceite Formal** | 30/11/2026 | 100% dos operadores aprovados, metas atingidas e termo de encerramento assinado. |

---

## 4. Matriz de Responsabilidades (RACI)

A Matriz RACI estabelece a governança de cada entrega:
- **R (Responsible):** Quem executa a atividade diretamente.
- **A (Accountable):** Quem responde pelo resultado final e tem autoridade de aprovação (apenas um "A" por atividade).
- **C (Consulted):** Quem deve ser consultado antes da tomada de decisão.
- **I (Informed):** Quem deve ser mantido informado sobre o andamento e conclusão.

### 📋 Mapeamento RACI por Pacote de Trabalho

| Pacote EAP / Atividade | Sponsor (Carlos) | Gerente Projetos (Giovani) | Eng. Automação (Roberto) | Analista TI (Luciana) | Esp. Qualidade (Fernando) | Manutenção (Marcos) | Operadores (Chão de Fábrica) |
|---|:---:|:---:|:---:|:---:|:---:|:---:|:---:|
| **1.1 TAP e Planejamento** | **A** | **R** | C | C | C | C | I |
| **2.1 Requisitos de Automação e TI** | I | **A** | **R** | **R** | C | C | C |
| **2.2 Projeto Executivo Elétrico/Redes** | I | **A** | **R** | C | I | C | I |
| **2.3 Aquisição de Equipamentos** | C | **A** | **R** | C | I | I | I |
| **3.1 Infraestrutura Fibra Óptica** | I | **A** | C | **R** | I | I | I |
| **3.2 Montagem Painéis Elétricos** | I | **A** | **R** | I | I | C | I |
| **3.3 Instalação de Sensores/Câmeras** | I | **A** | C | I | C | **R** | I |
| **4.1 Servidores e Banco de Dados** | I | **A** | I | **R** | I | I | I |
| **4.2 Camada OPC UA e Drivers CLP** | I | **A** | C | **R** | I | I | I |
| **4.3 Desenvolvimento da IHM** | I | **A** | C | **R** | C | I | C |
| **4.4 Dashboard OEE e Relatórios** | C | **A** | I | **R** | C | C | I |
| **5.1 Testes de Bancada (FAT)** | I | **A** | **R** | **R** | C | I | I |
| **5.2 Teste Integrado Linha 1 (SAT)** | C | **A** | **R** | **R** | C | **R** | C |
| **5.3 Auditoria Metrológica** | I | **A** | C | I | **R** | I | I |
| **6.1 Manuais e POPs** | I | **A** | C | C | **R** | C | I |
| **6.2 Treinamento Operacional** | I | **A** | C | C | I | I | **R** |
| **6.3 Operação Assistida (60 dias)** | C | **A** | **R** | **R** | C | **R** | C |
| **6.4 Termo de Aceite e Encerramento** | **A** | **R** | I | I | I | I | I |
