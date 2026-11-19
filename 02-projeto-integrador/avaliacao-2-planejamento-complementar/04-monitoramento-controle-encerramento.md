# 📊 Monitoramento, Controle e Encerramento do Projeto

**Projeto:** Sistema Integrado de Automação e Gestão Industrial (SIGAI) — MetalTech S.A.  
**Área do Conhecimento:** Monitoramento, Controle e Encerramento (PMBOK / UniSENAI-SP)  
**Versão:** 1.0 | **Data de Elaboração:** Fevereiro de 2026  

---

## 1. Painel de Indicadores de Desempenho (KPIs do Projeto)

O acompanhamento da saúde do projeto é realizado através de um painel de indicadores balanceados (**Scorecard de Projeto**), avaliados quinzenalmente pelo PMO:

| Dimensão | Indicador-Chave (KPI) | Fórmula / Métrica | Meta Operacional | Faixa de Atenção | Faixa Crítica |
|---|---|---|:---:|:---:|:---:|
| **Tempo** | Índice de Desempenho de Prazos (SPI) | $SPI = \frac{EV}{PV}$ | $\ge 1,00$ | $0,90 \le SPI < 1,00$ | $< 0,90$ |
| **Custo** | Índice de Desempenho de Custos (CPI) | $CPI = \frac{EV}{AC}$ | $\ge 1,00$ | $0,90 \le CPI < 1,00$ | $< 0,90$ |
| **Escopo** | Taxa de Entregas Validadas na 1ª Tentativa | $\frac{\text{Entregas Aprovadas}}{\text{Entregas Submetidas}}$ | $\ge 90\%$ | $80\% - 89\%$ | $< 80\%$ |
| **Qualidade** | Não Conformidades Abertas (RNCs Ativas) | Total de RNCs sem resolução | $\le 2$ | $3 - 5$ | $> 5$ |
| **Operação** | OEE Médio da Linha 1 de Usinagem | $\text{Disp.} \times \text{Perf.} \times \text{Qual.}$ | $\ge 85\%$ | $75\% - 84\%$ | $< 75\%$ |
| **RH / Clima** | Engajamento nos Treinamentos | Presença e nota na prova teórica/prática | $\ge 90\%$ | $80\% - 89\%$ | $< 80\%$ |

---

## 2. Governança do Comitê de Controle de Mudanças (CCB)

O Comitê de Controle de Mudanças (**Change Control Board — CCB**) é o órgão colegiado responsável por analisar os impactos de qualquer proposta de modificação de escopo, prazo ou custo antes de sua autorização.

### Composição do CCB:
- **Carlos Eduardo Albuquerque** — Patrocinador Executivo (Sponsor / Diretor Industrial)
- **Giovani Miamoto** — Gerente de Projetos (Secretário e Relator Técnico do CCB)
- **Eng. Roberto Mendes** — Líder de Engenharia e Automação
- **Luciana Silveira** — Líder de Arquitetura de TI

### Modelo de Solicitação de Mudança (Change Request Template):

```text
┌────────────────────────────────────────────────────────────────────────────────────────┐
│                      FORMULÁRIO DE SOLICITAÇÃO DE MUDANÇA (CR)                         │
├───────────────────────────────────────┬────────────────────────────────────────────────┤
│ Código da Mudança: CR-2026-003        │ Data da Solicitação: 12/06/2026                │
│ Projeto: SIGAI — MetalTech S.A.       │ Solicitante: Gerente de Manutenção Industrial   │
├───────────────────────────────────────┴────────────────────────────────────────────────┤
│ 1. DESCRIÇÃO DA MUDANÇA PROPOSTA:                                                      │
│ Inclusão de 4 sensores adicionais de temperatura no óleo hidráulico da Prensa P-02.   │
├────────────────────────────────────────────────────────────────────────────────────────┤
│ 2. JUSTIFICATIVA TÉCNICA / BENEFÍCIO:                                                  │
│ A prensa P-02 apresentou sobreaquecimento em regime pesado; monitorar a temperatura    │
│ previne quebra de retentores e reduz paradas em cerca de 4 horas/mês adicionais.       │
├────────────────────────────────────────────────────────────────────────────────────────┤
│ 3. AVALIAÇÃO DE IMPACTO PELO PMO:                                                      │
│ • Impacto no Escopo: Inclusão de 4 pontos analógicos no CLP e 1 tela de alerta na IHM. │
│ • Impacto no Cronograma: +2 dias na atividade A07 (não afeta o caminho crítico global).│
│ • Impacto Financeiro: R$ 14.200,00 (coberto pela Reserva de Contingência).             │
│ • Impacto em Riscos: Risco insignificante; melhora o controle de quebras da prensa.   │
├────────────────────────────────────────────────────────────────────────────────────────┤
│ 4. PARECER DO COMITÊ (CCB):                                                            │
│ [X] APROVADA    [ ] REPROVADA    [ ] SOLICITADAS MAIS INFORMAÇÕES                      │
│                                                                                        │
│ Assinatura Sponsor: ________________________   Data: 14/06/2026                        │
│ Assinatura Gerente Projeto: ________________   Data: 14/06/2026                        │
└────────────────────────────────────────────────────────────────────────────────────────┘
```

---

## 3. Procedimento Formal de Encerramento e Aceite

O encerramento do projeto SIGAI segue um protocolo estruturado em 4 etapas:

1. **Aceite Provisório (Marco M4 — Mês 8):**
   - Conclusão dos testes integrados com carga (SAT).
   - Início do período de 60 dias de **Operação Assistida**, com acompanhamento diário pela equipe técnica e registro de chamados residuais.
2. **Aceite Definitivo (Marco M5 — Mês 10):**
   - Atingimento comprovado das metas de desempenho (disponibilidade $\ge 85\%$, aumento de $15\%$ na produtividade da Linha 1 e redução de retrabalho).
   - Encerramento formal de 100% dos relatórios de não conformidade (RNCs).
   - Assinatura do **Termo de Aceite Definitivo** pelo Diretor Industrial.
3. **Desmobilização e Encerramento Financeiro/Contratual:**
   - Quitação final de notas fiscais de fornecedores terceirizados de fibra óptica e sensores.
   - Liberação de garantias contratuais e arquivamento de ARTs de engenharia elétrica.
   - Realocação dos recursos humanos internos de volta às suas funções ordinárias de operação e manutenção.
4. **Transição para a Operação e Manutenção (Sustentação):**
   - Entrega formal das senhas administrativas, documentação técnica *as-built*, manuais e código-fonte documentado para a Gerência de TI e Manutenção da MetalTech S.A.

---

## 4. Reunião de Post-Mortem e Registro de Lições Aprendidas

Ao término do projeto, realizou-se uma oficina formal de avaliação para documentar boas práticas e oportunidades de melhoria para os futuros projetos da empresa (como a Fase 2 de IoT e ERP):

### 📋 Registro de Lições Aprendidas (Lessons Learned Repository)

| Domínio de Gestão | O que aconteceu? (Situação / Desafio) | O que deu certo? (Ponto Forte) | O que pode ser melhorado? (Oportunidade) | Ação Recomendada para Próximos Projetos |
|---|---|---|---|---|
| **Engenharia de Campo** | Vibração mecânica inicial causou ruído nos sensores piezoelétricos na Prensa P-01. | Rápida atuação com coxins antivibração e suportes magnéticos de teste. | Estudo preliminar de vibração da carcaça antes da fixação definitiva. | Realizar ensaios de vibração prévios antes de adquirir suportes mecânicos. |
| **Comunicação / Pessoas** | Operadores mais antigos demonstraram receio de serem substituídos pela automação. | O programa "Operador 4.0" com capacitação prática e certificação desfez o medo. | Comunicação iniciada apenas no Mês 2 gerou ruídos nas primeiras semanas. | Iniciar o plano de comunicação com o chão de fábrica desde o Kick-off do projeto. |
| **Fornecedores / Compras** | O prazo de nacionalização dos gateways industriais demorou 12 dias a mais que o previsto. | A existência de 15 dias de folga na atividade A04 evitou atraso no caminho crítico. | Confiança inicial em cotações verbais de prazo sem cláusula contratual de SLA. | Incluir cláusulas contratuais de multa diária por atraso na entrega de hardware. |
| **Arquitetura de TI** | O tráfego de dados na rede fabril gerou picos que sobrecarregaram o switch legado. | A decisão de implantar anel redundante exclusivo de fibra óptica isolou o problema. | Não subestimar a volumetria de dados de telemetria contínua de alta frequência. | Projetar a infraestrutura de rede considerando 3 vezes a vazão estimada de dados. |
| **Gestão Orçamentária** | A cotação de serviços de calibração metrológica foi 10% maior devido à urgência de laudo. | A Reserva de Contingência absorveu a despesa sem necessidade de verba suplementar. | Cotações de auditoria metrológica feitas muito perto da data de execução. | Fechar contratos de auditoria e calibração com 60 dias de antecedência. |
