# 💰 Gerenciamento de Custos e Orçamento do Projeto

**Projeto:** Sistema Integrado de Automação e Gestão Industrial (SIGAI) — MetalTech S.A.  
**Área do Conhecimento:** Gerenciamento dos Custos (PMBOK / UniSENAI-SP)  
**Versão:** 1.0 | **Data de Elaboração:** Fevereiro de 2026  

---

## 1. Estrutura de Custos e Estimativas Orçamentárias

O orçamento do projeto foi estimado combinando a **técnica analítica *bottom-up*** (de baixo para cima, precificando pacote por pacote da EAP) com cotações de mercado e dados históricos de projetos industriais da MetalTech S.A.

Os custos dividem-se em despesas de capital (**CAPEX**) e custos operacionais de projeto (**OPEX**):

### 📋 Detalhamento Orçamentário por Categoria e Pacote da EAP

| Conta Contábil / Categoria | Pacote EAP | Descrição dos Itens de Custo | Qtd | Unid. | Valor Unitário | Custo Total (R$) | Tipo |
|---|:---:|---|:---:|:---:|---:|---:|:---:|
| **1. Recursos Humanos do Projeto** | | | | | | **R$ 480.000,00** | OPEX |
| • Gerente de Projeto (Giovani) | 1.0 | Coordenação, controle e governança (10 meses) | 10 | meses | R$ 14.000,00 | R$ 140.000,00 | |
| • Engenheiro de Automação Sênior | 2.0 / 3.0 / 5.0 | Projetos elétricos, redes e comissionamento | 10 | meses | R$ 12.000,00 | R$ 120.000,00 | |
| • Analista de Sistemas / Desenvolvedor TI | 4.0 | Backend OPC UA, banco de dados e dashboard web | 10 | meses | R$ 11.000,00 | R$ 110.000,00 | |
| • Especialista em Qualidade e Metrologia | 5.3 / 6.1 | Homologação de sensores, testes e manuais | 6 | meses | R$ 10.000,00 | R$ 60.000,00 | |
| • Técnico Especialista em Manutenção | 3.3 / 6.3 | Apoio mecânico em fixação e operação assistida | 5 | meses | R$ 10.000,00 | R$ 50.000,00 | |
| **2. Hardware e Infraestrutura Fabril** | | | | | | **R$ 460.000,00** | CAPEX |
| • Sensores de Vibração e Temperatura Preditivos | 3.3 | Acelerômetros piezoelétricos industriais blindados | 32 | un | R$ 4.500,00 | R$ 144.000,00 | |
| • Câmeras Industriais e Leitores DataMatrix | 3.3 | Leitores ópticos com iluminação integrada | 16 | un | R$ 6.500,00 | R$ 104.000,00 | |
| • Painéis Elétricos de Campo c/ Nobreak | 3.2 | Painéis Rittal com proteção IP66 e nobreaks senoidais | 4 | un | R$ 18.000,00 | R$ 72.000,00 | |
| • Switches Industriais Gerenciáveis e Gateways | 3.1 | Switches Gigabit com anel de redundância e gateways | 8 | un | R$ 8.500,00 | R$ 68.000,00 | |
| • Cabeamento de Fibra Óptica e Eletrocalhas | 3.1 | Cabos ópticos dielétricos, eletrocalhas perfuradas e conectores | 1 | pacote | R$ 72.000,00 | R$ 72.000,00 | |
| **3. Software, Servidores e Licenças** | | | | | | **R$ 180.000,00** | CAPEX |
| • Servidor de Aplicação Industrial em Rack | 4.1 | Servidor Dell PowerEdge c/ discos redundantes NVMe | 1 | un | R$ 65.000,00 | R$ 65.000,00 | |
| • Licenças de Servidor OPC UA Industrial | 4.2 | Licença Kepware Enterprise ilimitada para chão de fábrica | 1 | licença | R$ 45.000,00 | R$ 45.000,00 | |
| • Terminais Touchscreen Industriais (IHM) | 4.3 | Monitores industriais touch 21" com proteção IP65 | 8 | un | R$ 8.750,00 | R$ 70.000,00 | |
| **4. Serviços Terceirizados e Capacitação** | | | | | | **R$ 160.000,00** | OPEX |
| • Empresa de Instalação e Fusão de Fibra Óptica | 3.1 | Lançamento mecânico, fusão e certificação Fluke | 1 | serviço | R$ 60.000,00 | R$ 60.000,00 | |
| • Auditoria e Calibração Metrológica RBC | 5.3 | Aferição e emissão de laudo RBC para sensores a laser | 1 | serviço | R$ 40.000,00 | R$ 40.000,00 | |
| • Treinamento Externo e Certificação em CLP/OPC | 6.2 | Instrutoria técnica oficial e material didático | 4 | turmas | R$ 15.000,00 | R$ 60.000,00 | |
| — | — | **SUBTOTAL DO CUSTO BASE (Baseline)** | — | — | — | **R$ 1.280.000,00** | — |
| **5. Reservas Financeiras de Governança** | | | | | | **R$ 220.000,00** | — |
| • Reserva de Contingência (Riscos Conhecidos) | 1.1 | 10% do custo base para variações cambiais e retrabalhos | — | — | — | **R$ 128.000,00** | Contingência |
| • Reserva Gerencial (Imprevistos / Mudanças) | 1.1 | Verba estratégica administrada pelo Sponsor | — | — | — | **R$ 92.000,00** | Gerencial |
| 🏁 | — | **ORÇAMENTO TOTAL AUTORIZADO (BAC)** | — | — | — | **R$ 1.500.000,00** | — |

---

## 2. Linha de Base dos Custos (Cost Baseline) e Desembolso Mensal

O fluxo financeiro foi distribuído mensalmente ao longo dos 10 meses de execução, resultando na **Curva S** de desembolso acumulado:

| Mês | Período | Principais Entregas Financeiras do Mês | Desembolso Mensal (R$) | Custo Acumulado (R$) | % Acumulado (PV) |
|:---:|---|---|---:|---:|:---:|
| **M1** | Fev/26 | Iniciação, levantamento de requisitos e contratação de RH | R$ 60.000,00 | R$ 60.000,00 | 4,7% |
| **M2** | Mar/26 | Projeto executivo e emissão das ordens de compra de hardware | R$ 240.000,00 | R$ 300.000,00 | 23,4% |
| **M3** | Abr/26 | Chegada de hardware e instalação do anel de fibra óptica | R$ 260.000,00 | R$ 560.000,00 | 43,8% |
| **M4** | Mai/26 | Montagem de painéis elétricos e servidores industriais | R$ 190.000,00 | R$ 750.000,00 | 58,6% |
| **M5** | Jun/26 | Fixação física dos sensores nas máquinas e desenvolvimento OPC | R$ 150.000,00 | R$ 900.000,00 | 70,3% |
| **M6** | Jul/26 | Finalização das IHMs e testes lógicos em bancada (FAT) | R$ 110.000,00 | R$ 1.010.000,00 | 78,9% |
| **M7** | Ago/26 | Testes com carga na fábrica (SAT) e auditoria metrológica | R$ 90.000,00 | R$ 1.100.000,00 | 85,9% |
| **M8** | Set/26 | Treinamento de operadores e início da operação assistida | R$ 80.000,00 | R$ 1.180.000,00 | 92,2% |
| **M9** | Out/26 | Operação assistida plena e estabilização de relatórios | R$ 50.000,00 | R$ 1.230.000,00 | 96,1% |
| **M10** | Nov/26 | Conclusão da operação assistida e encerramento formal | R$ 50.000,00 | R$ 1.280.000,00 | 100,0% |

---

## 3. Metodologia de Monitoramento e Controle por Valor Agregado (EVM)

O controle econômico do projeto será executado por meio da técnica de **Gerenciamento do Valor Agregado (Earned Value Management — EVM)**, confrontando periodicamente o planejamento físico com os gastos reais.

### Fórmulas e Indicadores Adotados:
1. **Valor Planejado (PV — Planned Value):** Custo orçado do trabalho programado até a data de corte.
2. **Valor Agregado (EV — Earned Value):** Custo orçado do trabalho efetivamente realizado até a data de corte.
3. **Custo Real (AC — Actual Cost):** Custo total incorrido para realizar o trabalho entregue.
4. **Variação de Custos (CV):** $CV = EV - AC$ *(Se $> 0$, o projeto está abaixo do orçamento).*
5. **Variação de Prazos (SV):** $SV = EV - PV$ *(Se $> 0$, o projeto está adiantado).*
6. **Índice de Desempenho de Custos (CPI):** $CPI = \frac{EV}{AC}$ *(Se $\ge 1,0$, custo eficiente).*
7. **Índice de Desempenho de Prazos (SPI):** $SPI = \frac{EV}{PV}$ *(Se $\ge 1,0$, cronograma eficiente).*

### Gatilhos de Ação Corretiva:
- **Faixa Verde ($0,95 \le CPI, SPI \le 1,05$):** Operação sob controle; nenhuma intervenção extraordinária necessária.
- **Faixa Amarela ($0,85 \le CPI < 0,95$ ou $0,85 \le SPI < 0,95$):** Emissão de alerta gerencial e revisão técnica de atividades não críticas.
- **Faixa Vermelha ($CPI < 0,85$ ou $SPI < 0,85$):** Convocação imediata do Sponsor, paralisação de despesas discricionárias e aplicação de plano de recuperação (crashing ou fast-tracking).
