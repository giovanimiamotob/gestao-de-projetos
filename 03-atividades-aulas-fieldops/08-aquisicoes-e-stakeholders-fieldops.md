# Plano de Aquisições e Matriz de Poder × Interesse dos Stakeholders
## Projeto FieldOps — Plataforma de Inspeção Técnica em Campo

- **Disciplina:** Gestão de Projetos de TI (UniSENAI-SP)
- **Docente:** Prof. Me. Deivison S. Takatu
- **Autor / Gerente de Projetos:** Giovani Miamoto (`giovanimiamotob`)
- **Referência:** Aula 08 — Gerenciamento das Aquisições e das Partes Interessadas
- **Requisitos do Enunciado:**
  1. Tabela completa de Gerenciamento das Aquisições do Projeto FieldOps com item, urgência, motivo, fornecedores, quantidade, custo unitário e total.
  2. Matriz de Rede de Poder/Interesse classificando os stakeholders nos quadrantes: *Monitorar*, *Manter Informado*, *Manter Satisfeito* e *Gerenciar com Atenção*.
- **Versão:** 1.0 (Aprovada)

---

# PARTE 1: GERENCIAMENTO DAS AQUISIÇÕES DO PROJETO

## 1.1 Estratégia de Compras e Decisões "Fazer vs. Comprar" (*Make-or-Buy*)

O Projeto FieldOps adotou como diretriz focar o esforço interno de desenvolvimento no **core business** (regras de inspeção dinâmica, fluxo de aprovação e sincronização *offline-first*) e terceirizar infraestrutura, segurança de nuvem e insumos físicos por meio de contratações especializadas:
- **Make (Fazer internamente):** Código-fonte da API Node.js, aplicativo React Native, painel web Next.js e esquemas relacionais PostgreSQL.
- **Buy (Contratar/Adquirir externamente):** Armazenamento em nuvem elástica (AWS S3/RDS), smartphones robustos de teste com leitor biométrico, etiquetas físicas QR Code em alumínio anodizado e auditoria externa de segurança (Pentest).

---

## 1.2 Tabela de Gerenciamento das Aquisições do Projeto FieldOps

Abaixo apresenta-se a tabela de aquisições contendo todos os campos exigidos nos slides da Aula 08:

| ID | Cód. EAP | Item a Ser Adquirido | Urgência | Motivo da Decisão de Compra | Fornecedores Potenciais Qualificados | Qtd | Custo Unitário (R$) | Custo Total (R$) | Tipo de Contrato | Previsão de Entrega | Critérios de Seleção & Observações |
| :---: | :---: | :--- | :---: | :--- | :--- | :---: | :---: | :---: | :---: | :---: | :--- |
| **01** | 1.6.3 | Smartphones Android de Teste (Câmera 50MP, 128GB, GPS) | 5 - Muito Alta | Dispositivos dedicados para homologação e estresse de campo pelo time piloto | Motorola, Samsung, Xiaomi | 5 | R$ 1.450,00 | R$ 7.250,00 | Preço Fixo (PO) | Semana 2 | Câmera com autofoco rápido e certificação IP68 para poeira/água |
| **02** | 1.6.3 | Capas de Proteção Militar Anti-queda e Películas de Vidro | 4 - Alta | Proteção física dos aparelhos contra quedas frequentes em pisos de cimento | Spigen, Gorila Shield | 5 | R$ 120,00 | R$ 600,00 | Preço Fixo | Semana 2 | Compatibilidade exata e absorção de impacto de 2 metros |
| **03** | 1.6.3 | Baterias Portáteis (*Powerbanks*) 20.000mAh Homologadas | 4 - Alta | Garantir autonomia técnica durante turnos de 10h sem tomada em campo | Anker, Baseus, Geonav | 5 | R$ 180,00 | R$ 900,00 | Preço Fixo | Semana 3 | Certificação Anatel e suporte a carregamento rápido USB-C |
| **04** | 1.2.2 | Etiquetas Metálicas de QR Code em Alumínio Anodizado | 4 - Alta | Identificação física indelével dos ativos industriais nas plantas piloto | MetalPrint, 3M, Plastikote | 500 | R$ 4,50 | R$ 2.250,00 | Preço Fixo | Semana 4 | Resistência a solventes químicos, altas temperaturas e chuva |
| **05** | 1.2.2 | Banco de Dados Gerenciado AWS RDS PostgreSQL (Multi-AZ) | 5 - Muito Alta | Persistência central de alta disponibilidade e backups automatizados diários | Amazon Web Services (AWS) | 4 | R$ 1.300,00 | R$ 5.200,00 | Sob Demanda (Pay-as-you-go) | Semana 3 | SLA contratual de 99,95% e suporte a réplica de leitura |
| **06** | 1.2.2 | Armazenamento de Arquivos em Nuvem AWS S3 Standard | 5 - Muito Alta | Repositório em nuvem de fotos, laudos em PDF e logs de auditoria | Amazon Web Services (AWS) | 4 | R$ 450,00 | R$ 1.800,00 | Sob Demanda | Semana 3 | Durabilidade de 99,999999999% de objetos e URLs assinadas |
| **07** | 1.2.3 | Servidor de Execução em Contêiner AWS ECS/Fargate | 5 - Muito Alta | Hospedagem dos microsserviços Node.js sem sobrecarga de gestão de OS | Amazon Web Services (AWS) | 4 | R$ 1.450,00 | R$ 5.800,00 | Sob Demanda | Semana 3 | Escalabilidade automática elástica de CPU e memória |
| **08** | 1.1.3 | Assinatura GitHub Team (Controle de Versão e Actions CI/CD) | 5 - Muito Alta | Repositório central de código-fonte, automação de builds e testes | GitHub Inc. (Microsoft) | 4 | R$ 320,00 | R$ 1.280,00 | Assinatura Mensal | Semana 1 | Minutos incluídos de CI/CD em runners Linux e branch protection |
| **09** | 1.2.2 | Licença Figma Organization (Design System e Prototipação) | 4 - Alta | Criação colaborativa de interfaces, protótipos de alta fidelidade e Handoff | Figma Inc. | 4 | R$ 280,00 | R$ 1.120,00 | Assinatura Mensal | Semana 1 | Compartilhamento em tempo real com desenvolvedores e clientes |
| **10** | 1.4.1 | Assinatura Expo Application Services (EAS Build / Deploy) | 4 - Alta | Compilação remota de binários APK/AAB e envio de patches OTA | 650 Industries Inc. (Expo)| 4 | R$ 580,00 | R$ 2.320,00 | Assinatura Mensal | Semana 2 | Build concorrente de Android sem necessidade de máquina local pesada |
| **11** | 1.6.1 | Licença Sentry Performance Tracking & APM Cloud | 3 - Média | Monitoramento em tempo real de crashes do app mobile e erros da API | Functional Software (Sentry)| 4 | R$ 360,00 | R$ 1.440,00 | Assinatura Mensal | Semana 4 | Rastreamento de chamadas lentas e captura de stack traces nativos |
| **12** | 1.6.4 | Consultoria Jurídica Externa Especializada em LGPD | 3 - Média | Elaboração dos Termos de Uso, Política de Privacidade e consentimento | Escritório Silveira & Associados | 1 | R$ 5.500,00 | R$ 5.500,00 | Preço Fixo (Escopo Fechado) | Semana 8 | Especialização comprovada em direito digital e privacidade técnica |
| **13** | 1.6.1 | Teste de Intrusão Externo e Análise de Vulnerabilidade (Pentest)| 4 - Alta | Auditoria de segurança ofensiva antes da entrada em produção | HackerSec / Clavis Segurança | 1 | R$ 7.500,00 | R$ 7.500,00 | Preço Fixo | Semana 12 | Emissão de laudo formal de segurança com reteste gratuito incluído |
| **14** | 1.6.4 | Confecção de Apostilas e Manuais de Bolso Plastificados (A5)| 2 - Baixa | Suporte didático para os técnicos de campo consultarem rotinas offline | Gráfica Rápida Express | 50 | R$ 22,00 | R$ 1.100,00 | Preço Fixo | Semana 13 | Encadernação wire-o com laminação fosca à prova d'água |
| **15** | 1.6.5 | Conta de Desenvolvedor Google Play Console (Taxa Vitalícia)| 4 - Alta | Publicação oficial do app corporativo na Google Play Store interna | Google LLC | 1 | R$ 150,00 | R$ 150,00 | Taxa Única | Semana 6 | Requisito obrigatório para distribuição controlada do APK corporativo |
| **TOTAL** | - | **Total Consolidado das Aquisições do Projeto** | - | - | - | - | - | **R$ 44.460,00** | - | - | - |

---

# PARTE 2: GERENCIAMENTO DAS PARTES INTERESSADAS (STAKEHOLDERS)

## 2.1 Identificação e Postura Analítica das Partes Interessadas

Conforme metodologia apresentada na Aula 08, os stakeholders foram mapeados quanto ao seu nível de engajamento atual (**C** = Atual / *Current*) e desejado (**D** = Desejado / *Desired*):

| ID | Parte Interessada | Papel no Contexto FieldOps | Desinformado | Resistente | Neutro | Dá Apoio | Lidera |
| :---: | :--- | :--- | :---: | :---: | :---: | :---: | :---: |
| **S1** | **Carlos Alberto Silveira** | Patrocinador Executivo (*Sponsor*) / Diretor de Operações | | | | C | **D** |
| **S2** | **Giovani Miamoto** | Gerente de Projetos de TI (Líder da Iniciativa) | | | | | **C, D** |
| **S3** | **Roberto Mendonça** | Gerente Geral de TI & Infraestrutura Corporativa | | | C | **D** | |
| **S4** | **Equipe de Supervisores** | Supervisores de Manutenção (Aprovadores de Laudo) | | C | | **D** | |
| **S5** | **Técnicos de Campo** | Usuários Finais Operacionais do Aplicativo Mobile | | C | | **D** | |
| **S6** | **Equipe de Desenvolvimento**| Arquitetos, Devs Backend/Mobile/Web, DevOps e QA | | | | C | **D** |
| **S7** | **Clientes Industriais** | Clientes Contratantes que recebem laudos de vistoria | | | C | **D** | |
| **S8** | **Diretoria Financeira** | Controladoria e Liberação Orçamentária (*CFO*) | | | C | **D** | |
| **S9** | **Jurídico / DPO** | Encarregado de Proteção de Dados (LGPD) | | | C | **D** | |
| **S10**| **Fornecedores Cloud (AWS/Expo)**| Provedores de Plataforma e Infraestrutura | | | **C, D**| | |

---

## 2.2 Matriz de Rede de Poder × Interesse (Mendelow Grid)

Mapeamento visual distribuindo as partes interessadas nos quatro quadrantes estratégicos:

```
PODER (Autoridade / Influência)
  Alto ^
       |  [ MANTER SATISFEITO ]             |  [ GERENCIAR COM ATENÇÃO ]
       |                                    |
       |  • S8: Diretoria Financeira (CFO)   |  • S1: Carlos Silveira (Sponsor Executivo)
       |  • S9: Jurídico & DPO (LGPD)       |  • S2: Giovani Miamoto (Gerente Projetos)
       |  • S7: Clientes Industriais Chave  |  • S3: Roberto Mendonça (Gerente TI)
       |                                    |
  -----+------------------------------------+------------------------------------>
       |  [ MONITORAR (Mínimo Esforço) ]   |  [ MANTER INFORMADO ]
       |                                    |
       |  • S10: Fornecedores Cloud (AWS)   |  • S4: Supervisores Técnicos de Campo
       |  • Comunidade Externa & Mercado    |  • S5: Técnicos Operacionais de Campo
       |                                    |  • S6: Equipe Técnica de Desenvolvimento
  Baixo|                                    |
       +------------------------------------+------------------------------------>
       Baixo                                Alto                   INTERESSE
```

---

## 2.3 Estratégia de Engajamento por Quadrante

### 1. Gerenciar com Atenção (Alto Poder / Alto Interesse)
- **Partes Interessadas:** Patrocinador Executivo (S1), Gerente de Projetos (S2), Gerente de TI (S3).
- **Abordagem Estratégica:** Envolvimento direto na governança executiva; reuniões mensais de progresso (*Status Report* executivo com Curva S e EVM); participação mandatória nas deliberações do Comitê de Mudanças (CCB).
- **Objetivo:** Garantir alinhamento estratégico ininterrupto, suporte corporativo e liberação ágil de impedimentos organizacionais.

### 2. Manter Satisfeito (Alto Poder / Baixo Interesse)
- **Partes Interessadas:** Diretoria Financeira (S8), Jurídico/DPO (S9), Clientes Industriais Chave (S7).
- **Abordagem Estratégica:** Comunicações pontuais e altamente objetivas; envio de demonstrativos consolidados de conformidade fiscal e legal; relatórios de conformidade com a LGPD e pentest; assegurar que o orçamento permaneça dentro dos limites sem surpresas financeiras.
- **Objetivo:** Prevenir bloqueios burocráticos ou vetos regulatórios que possam paralisar o projeto.

### 3. Manter Informado (Baixo Poder / Alto Interesse)
- **Partes Interessadas:** Supervisores de Manutenção (S4), Técnicos de Campo (S5), Equipe de Desenvolvimento (S6).
- **Abordagem Estratégica:** Comunicação contínua, aberta e consultiva; demonstrações quinzenais de software (*Sprint Review*); oficinas de cocriação de telas e rotinas; canal permanente de dúvidas e sugestões via Slack; programa de capacitação com material didático ilustrado.
- **Objetivo:** Mitigar a resistência à transição digital, transformando os operadores em defensores entusiasmados do novo sistema.

### 4. Monitorar (Baixo Poder / Baixo Interesse)
- **Partes Interessadas:** Fornecedores de Cloud e Ferramentas SaaS (S10), órgãos reguladores indiretos.
- **Abordagem Estratégica:** Acompanhamento passivo dos painéis de status de serviço (*Health Checks* da AWS/Expo) e renovação automática de faturas.
- **Objetivo:** Detectar tempestivamente eventuais descontinuações de bibliotecas ou alterações em tabelas de preços sem consumir esforço excessivo da gestão.
