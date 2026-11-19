# ⚠️ Gerenciamento dos Riscos do Projeto

**Projeto:** Sistema Integrado de Automação e Gestão Industrial (SIGAI) — MetalTech S.A.  
**Área do Conhecimento:** Gerenciamento dos Riscos (PMBOK / UniSENAI-SP)  
**Versão:** 1.0 | **Data de Elaboração:** Fevereiro de 2026  

---

## 1. Estratégia de Gerenciamento de Riscos

O gerenciamento de riscos do projeto SIGAI segue o ciclo contínuo do PMBOK: **Identificação $\rightarrow$ Análise Qualitativa e Quantitativa $\rightarrow$ Planejamento de Respostas $\rightarrow$ Monitoramento e Controle**.

### Critérios de Classificação da Escala 5 × 5:

* **Probabilidade (P):**
  - `1 - Muito Baixa` ($< 10\%$)
  - `2 - Baixa` ($10\% - 30\%$)
  - `3 - Média` ($31\% - 50\%$)
  - `4 - Alta` ($51\% - 70\%$)
  - `5 - Muito Alta` ($> 70\%$)

* **Impacto (I):**
  - `1 - Insignificante` (desvio $< 2$ dias ou $< \text{R\$} \ 5\text{k}$)
  - `2 - Menor` (desvio de $3-7$ dias ou $\text{R\$} \ 5\text{k} - \text{R\$} \ 20\text{k}$)
  - `3 - Moderado` (desvio de $8-15$ dias ou $\text{R\$} \ 20\text{k} - \text{R\$} \ 50\text{k}$)
  - `4 - Maior` (desvio de $16-30$ dias ou $\text{R\$} \ 50\text{k} - \text{R\$} \ 100\text{k}$)
  - `5 - Crítico` (desvio $> 30$ dias, estouro orçamentário severo ou risco à segurança/NR-10/NR-12)

* **Grau de Severidade ($S = P \times I$):**
  - 🟢 **Baixo (1 a 5):** Aceitar o risco e monitorar periodicamente.
  - 🟡 **Médio (6 a 11):** Mitigação planejada e acompanhamento quinzenal.
  - 🟠 **Alto (12 a 19):** Plano de ação mandatória e monitoramento semanal.
  - 🔴 **Crítico (20 a 25):** Escalação imediata ao Sponsor e plano de contingência formal.

---

## 2. Registro e Detalhamento dos Riscos Identificados

Foram mapeados **10 riscos prioritários** cobrindo dimensões técnicas, operacionais, fornecedores, humanas e financeiras:

| ID | Descrição do Risco | Categoria / Causa Raiz | Impacto no Projeto | P | I | Severidade (P×I) | Nível | Estratégia de Resposta |
|:---:|---|---|---|:---:|:---:|:---:|:---:|:---:|
| **RSK-01** | Atraso na entrega de sensores importados e gateways IoT | Fornecedor / Gargalo logístico internacional na importação | Atraso nas atividades A05/A06 do caminho crítico e ociosidade de equipe | 3 | 4 | **12** | 🟠 Alto | **Mitigar / Prevenir** |
| **RSK-02** | Resistência cultural dos operadores ao novo sistema digital | Humana / Insegurança no emprego e aversão ao uso de tablets/IHM | Apontamentos incorretos, sabotagem de dados e perda de acurácia no OEE | 4 | 3 | **12** | 🟠 Alto | **Mitigar** |
| **RSK-03** | Incompatibilidade de protocolo em CLPs legados antigos da fábrica | Técnica / Máquinas de diferentes fabricantes sem suporte nativo OPC UA | Retrabalho de software, compra de gateways extras e atraso na telemetria | 3 | 4 | **12** | 🟠 Alto | **Prevenir / Mitigar** |
| **RSK-04** | Interferência eletromagnética (EMI) degradando sinal de dados | Técnica / Motores de alta potência e prensas gerando ruído elétrico | Queda intermitente na rede industrial e perda de pacotes de dados | 3 | 3 | **9** | 🟡 Médio | **Mitigar** |
| **RSK-05** | Flutuação cambial (Dólar) elevando custo de hardware importado | Financeira / Instabilidade macroeconômica e variação da moeda | Estouro da baseline de custos de equipamentos de automação | 3 | 3 | **9** | 🟡 Médio | **Transferir / Aceitar** |
| **RSK-06** | Acidente de trabalho durante passagem de cabeamento ou painéis | Segurança / Trabalho em altura e proximidade de barramentos elétricos | Paralisação da fábrica pelo MPT, multas pesadas e danos físicos | 1 | 5 | **5** | 🟢 Baixo | **Prevenir** |
| **RSK-07** | Indisponibilidade de parada de máquina para instalação física | Operacional / Demanda urgente de produção comercial impedindo parada | Reprogramação de montagem mecânica para fins de semana com hora extra | 4 | 2 | **8** | 🟡 Médio | **Mitigar** |
| **RSK-08** | Saída inesperada do Desenvolvedor de Software da equipe | Recursos Humanos / Rotatividade de profissionais no mercado de TI | Perda de produtividade no desenvolvimento do backend e dashboards | 2 | 4 | **8** | 🟡 Médio | **Mitigar** |
| **RSK-09** | Vulnerabilidade de segurança na rede OT permitindo ataque cibernético | Segurança da Informação / Rede de chão de fábrica exposta à internet | Parada maliciosa de maquinário ou sequestro de dados (Ransomware) | 2 | 5 | **10** | 🟡 Médio | **Prevenir** |
| **RSK-10** | Divergência metrológica entre sensor óptico e inspeção de bancada | Qualidade / Calibração inadequada ou vibração excessiva no suporte | Rejeição de lotes de peças pelo cliente automotivo (montadora) | 2 | 4 | **8** | 🟡 Médio | **Mitigar** |

---

## 3. Matriz de Probabilidade × Impacto (Diagrama Visual)

```text
IMPACTO
  ▲
5 │           [RSK-06]      [RSK-09] 
4 │                         [RSK-08,10]   [RSK-01,02,03]
3 │                                       [RSK-04,05]
2 │                         [RSK-07]
1 │
  └────────────────────────────────────────────────────────► PROBABILIDADE
       1 (M.Baixa)   2 (Baixa)     3 (Média)    4 (Alta)     5 (M.Alta)
```

---

## 4. Planos de Ação, Contingência e Donos de Risco

### RSK-01: Atraso na Entrega de Sensores
- **Ação Preventiva/Mitigadora:** Realizar compras nas primeiras duas semanas de projeto; homologar dois distribuidores nacionais que possuam estoque regulador no Brasil.
- **Plano de Contingência:** Caso o atraso exceda 10 dias, acionar fornecedor nacional reserva mediante pagamento de frete expresso pago pela Reserva de Contingência.
- **Gatilho:** Pedido não despachado em até 20 dias da emissão da Ordem de Compra.
- **Dono do Risco:** Comprador Industrial / Gerente de Projetos (Giovani Miamoto).

### RSK-02: Resistência Operacional dos Colaboradores
- **Ação Preventiva/Mitigadora:** Promover reuniões de conscientização antes da montagem física; criar o programa "Operador 4.0"; envolver operadores líderes no design da IHM para que seja intuitiva.
- **Plano de Contingência:** Reforçar a presença do instrutor técnico em campo no primeiro mês de operação assistida e instituir bônus de engajamento por equipe com 100% de apontamento correto.
- **Gatilho:** Taxa de rejeição ou apontamento manual acima de 15% nas primeiras duas semanas de testes.
- **Dono do Risco:** Especialista de RH / Gerente de Produção.

### RSK-03: Incompatibilidade em CLPs Legados
- **Ação Preventiva/Mitigadora:** Realizar auditoria técnica física (varredura de firmwares) em 100% das 16 máquinas nos primeiros 15 dias de projeto.
- **Plano de Contingência:** Instalar módulos remotos de I/O distribuído (Fieldbus) com ligação direta aos sensores físicos, sem depender da CPU do CLP antigo.
- **Gatilho:** CLP não responder às requisições do driver OPC UA nos testes de bancada.
- **Dono do Risco:** Eng. de Automação (Roberto Mendes).

### RSK-05: Flutuação Cambial
- **Ação Preventiva/Mitigadora:** Negociação de contratos de fornecimento em moeda nacional (Reais) com preço fixo travado (*hedge* comercial com o distribuidor).
- **Plano de Contingência:** Absorção do diferencial de custo através dos R$ 128.000,00 da Reserva de Contingência aprovada.
- **Gatilho:** Variação cambial superior a 8% na data do faturamento do hardware.
- **Dono do Risco:** Gerente de Projetos / Controladoria Financeira.

### RSK-09: Cibersegurança e Vulnerabilidade em Redes Industriais
- **Ação Preventiva/Mitigadora:** Implementação de arquitetura de rede segmentada conforme norma ISA/IEC 62443, com Firewall Industrial e DMZ exclusiva entre a rede corporativa e o chão de fábrica.
- **Plano de Contingência:** Isolamento físico imediato do switch industrial via VLAN de contingência e restauração do backup estático offline dos servidores.
- **Gatilho:** Detecção de tráfego anômalo ou tentativa de acesso não autenticado pelo IDS/IPS.
- **Dono do Risco:** Analista de TI / Segurança da Informação (Luciana Silveira).
