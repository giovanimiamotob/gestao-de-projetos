# 📊 Etapa 1 — Análise e Seleção do Portfólio

**Empresa:** MetalTech S.A.  
**Unidade:** Escritório de Gerenciamento de Projetos (PMO)  
**Ciclo de Planejamento:** 12 Meses  

---

## 1. Avaliação dos 8 Projetos Candidatos

A equipe do PMO conduziu uma análise multicritério aprofundada dos 8 projetos estratégicos em avaliação na **MetalTech S.A.**, ponderando investimento financeiro, prazo de execução, nível de risco técnico-operacional, principais benefícios entregues e aderência direta aos 4 objetivos estratégicos da organização.

### 📋 Tabela Comparativa Geral

| ID | Nome do Projeto | Investimento | Prazo | Risco | Principal Benefício Declarado | Objetivos Estratégicos Impactados |
|:---:|---|:---:|:---:|:---:|---|---|
| **P1** | Automação da Linha 1 | R$ 900 mil | 6 meses | Alto | +12% na produtividade da linha principal | ⚙️ Produtividade (+15%) |
| **P2** | Sistema de Manutenção Preditiva | R$ 450 mil | 4 meses | Médio | -20% em paradas não planejadas de máquinas | 🛠️ Paradas (-20%) / 📉 Custos (-10%) |
| **P3** | Novo ERP Industrial | R$ 1,2 milhão | 10 meses | Alto | Integração dos processos corporativos | 📉 Custos operacionais / Integração |
| **P4** | Programa de Redução de Refugo | R$ 250 mil | 3 meses | Baixo | -25% de desperdício de matéria-prima | 📉 Custos (-10%) / 🎯 Qualidade |
| **P5** | Modernização do Controle de Qualidade | R$ 350 mil | 4 meses | Médio | -30% em retrabalho de componentes | 🎯 Qualidade (-30% retrabalho) |
| **P6** | Treinamento de Operadores | R$ 150 mil | 2 meses | Baixo | Aumento de produtividade e segurança operacional | ⚙️ Produtividade / Capacitação P1 |
| **P7** | Sistema de Monitoramento IoT | R$ 600 mil | 5 meses | Médio | Disponibilização de telemetria em tempo real | ⚙️ Produtividade / Infraestrutura P3 |
| **P8** | Expansão da Capacidade Produtiva | R$ 1,5 milhão | 12 meses | Alto | +20% na capacidade física instalada da fábrica | ⚙️ Volume Produtivo |

---

## 2. Mapeamento de Interdependências e Sinergias

Conforme levantado nas diretrizes técnicas, foram mapeadas as seguintes relações de precedência, complementaridade e sinergia operacional:

1. **P1 (Automação da Linha 1) ↔ P6 (Treinamento de Operadores):**
   - *Análise de Dependência:* A automação dos postos de trabalho exige capacitação prévia ou concomitante dos operadores para operação de novas IHM (Interfaces Homem-Máquina), robôs e sistemas de segurança. Sem o P6, o P1 sofrerá curva de aprendizado prolongada e risco de acidentes ou paradas não programadas.
   - *Decisão Técnica:* P6 deve ser iniciado no início do ciclo e finalizado antes do comissionamento completo de P1.

2. **P4 (Redução de Refugo) ↔ P5 (Modernização do Controle de Qualidade):**
   - *Análise de Sinergia:* Ambos atuam de forma simbiótica no chão de fábrica. P4 atua na causa raiz do desperdício de matéria-prima metálica e corte, enquanto P5 atua na detecção precoce e garantia dimensional dos produtos acabados.
   - *Decisão Técnica:* Integrar P4 e P5 em um único programa coordenado, gerando economia de escala e padronização rápida.

3. **P3 (Novo ERP Industrial) ↔ P7 (Sistema de Monitoramento IoT):**
   - *Análise de Dependência:* O ERP corporativo necessita de dados confiáveis de produção. A implantação prévia ou conjunta da telemetria IoT (P7) fornece os dados em tempo real necessários para a alimentação dos módulos de PCP do ERP.
   - *Restrição:* A soma de P3 + P7 totaliza R$ 1,8 milhão (72% do orçamento total) e consome 100% dos recursos de TI por até 10 meses. Executá-los agora inviabilizaria os ganhos imediatos na fábrica.

4. **P8 (Expansão de Capacidade) ↔ P1 (Automação da Linha 1):**
   - *Recomendação Corporativa:* A diretoria recomenda expressamente que a automação e otimização da Linha 1 (P1) ocorram **antes** da expansão física da fábrica. Expandir capacidade com processos manuais e ineficientes apenas multiplicaria o retrabalho e o refugo.

---

## 3. Matriz de Decisão Multicritério (Ponderação Estratégica)

Cada projeto foi avaliado em uma escala de 1 a 5 nos seguintes fatores:
- **Alinhamento Estratégico (Peso 30%):** Contribuição direta para as 4 metas corporativas.
- **Relação Custo-Benefício / ROI (Peso 25%):** Ganhos proporcionais ao capital investido.
- **Exequibilidade e Riscos (Peso 25%):** Prazo curto, baixo risco e disponibilidade de recursos humanos.
- **Urgência Operacional (Peso 20%):** Necessidade de intervenção rápida no parque industrial.

| Projeto | Alinhamento (30%) | Custo-Benefício (25%) | Exequibilidade (25%) | Urgência (20%) | Pontuação Ponderada | Classificação Final |
|:---:|:---:|:---:|:---:|:---:|:---:|:---:|
| **P1** | 5 (1,50) | 4 (1,00) | 3 (0,75) | 5 (1,00) | **4,25** | 🟢 **Prioridade** |
| **P2** | 5 (1,50) | 5 (1,25) | 4 (1,00) | 5 (1,00) | **4,75** | 🟢 **Prioridade** |
| **P4** | 4 (1,20) | 5 (1,25) | 5 (1,25) | 4 (0,80) | **4,50** | 🟢 **Prioridade** |
| **P5** | 5 (1,50) | 4 (1,00) | 4 (1,00) | 4 (0,80) | **4,30** | 🟢 **Prioridade** |
| **P6** | 4 (1,20) | 5 (1,25) | 5 (1,25) | 5 (1,00) | **4,70** | 🟢 **Prioridade** |
| **P7** | 3 (0,90) | 3 (0,75) | 3 (0,75) | 3 (0,60) | **3,00** | 🟡 **Posterior** |
| **P3** | 3 (0,90) | 2 (0,50) | 2 (0,50) | 2 (0,40) | **2,30** | 🟡 **Posterior** |
| **P8** | 3 (0,90) | 2 (0,50) | 2 (0,50) | 2 (0,40) | **2,30** | 🔴 **Adiado** |

---

## 4. Classificação Final do Portfólio

Com base nas evidências quantitativas e qualitativas, a classificação oficial aprovada pelo PMO é:

### 🟢 Grupo 1: Prioridade (Execução nos Próximos 12 Meses)
1. **P1 — Automação da Linha 1 (R$ 900 mil):** Garante salto tecnológico imediato e entrega +12% de produtividade.
2. **P2 — Sistema de Manutenção Preditiva (R$ 450 mil):** Atende integralmente à meta de -20% de paradas de máquinas, protegendo a produção da Linha 1.
3. **P4 — Programa de Redução de Refugo (R$ 250 mil):** Retorno rápido (3 meses), ataca diretamente o desperdício financeiro de matéria-prima.
4. **P5 — Modernização do Controle de Qualidade (R$ 350 mil):** Atende diretamente a meta de -30% em retrabalho e protege a imagem da marca junto aos clientes automotivos.
5. **P6 — Treinamento de Operadores (R$ 150 mil):** Habilita as equipes para as novas tecnologias de P1 e garante produtividade sustentável.

*Subtotal Aprovado:* **R$ 2.100.000,00** *(dentro do teto de R$ 2,5M, restando R$ 400 mil de reserva gerencial).*

---

### 🟡 Grupo 2: Posterior (Fase 2 — Planejamento para o Ano 2)
1. **P7 — Sistema de Monitoramento IoT (R$ 600 mil):** Relevante para telemetria em nuvem, mas as máquinas da Linha 1 e a manutenção preditiva (P1 e P2) precisam estar implantadas e estabilizadas primeiro.
2. **P3 — Novo ERP Industrial (R$ 1,2 milhão):** Projeto de altíssimo risco e longo prazo (10 meses). Depende da maturidade dos processos de chão de fábrica que serão otimizados no Ano 1. Deve ser o carro-chefe da Transformação Digital no Ano 2.

---

### 🔴 Grupo 3: Adiado (Sem Previsão Imediata)
1. **P8 — Expansão da Capacidade Produtiva (R$ 1,5 milhão):** Excede a capacidade financeira restante do ciclo atual e violaria a diretriz de otimizar a planta existente antes de investir em obras civis e novas instalações. Será reavaliado no planejamento estratégico do Ano 3.
