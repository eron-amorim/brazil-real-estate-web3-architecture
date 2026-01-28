# Matriz de Risco — Estruturas Imobiliárias com Representação Digital (Brasil)

## Objetivo
Mapear os principais riscos que “matam” uma operação/empresa de estruturação e governança
para ativos imobiliários com representação digital no Brasil, e propor mitigadores práticos.

## Escopo
- Visão B2B / infraestrutura / governança (sem captação e sem promessa de retorno).
- Triagem de risco para conversar com advogado, gestor, compliance e dev.

## Escala
- **Probabilidade (P):** Baixa / Média / Alta
- **Impacto (I):** Baixo / Médio / Alto
- **Nível:** combinação qualitativa (ex.: Alto x Alto = Crítico)

---

## 1) Regulatório (CVM / BC / enquadramento)

### Risco
Estrutura ou comunicação ser interpretada como **valor mobiliário** (CVM) ou como atividade regulada
sem aderência (ex.: VASP/BC em cenário inadequado).

### Causas comuns
- linguagem de “rentabilidade”, “yield”, “renda garantida”
- “liquidez” prometida (marketplace, recompra, saída)
- distribuição ampla (público geral)
- pooling de investidores com esforço de terceiros (CIC na essência)
- operar fluxo de recursos de terceiros

### P/I
P: Média | I: Alto | Nível: **Crítico**

### Mitigadores (operacionais)
- **Radar de valor mobiliário** aplicado em todo projeto (documento de triagem)
- Revisão jurídica especializada (mercado de capitais) quando houver dúvida
- Política de comunicação: “sem promessa”, “sem liquidez”, “sem oferta”
- Escopo B2B: governança/relatórios/infra, não captação
- Registro de decisões e racional (trilha de auditoria)

---

## 2) Risco de promessa / marketing (reputacional + regulatório)

### Risco
O projeto ser vendido como “investimento” por linguagem comercial inadequada,
gerando risco legal e destruição de reputação.

### P/I
P: Alta | I: Alto | Nível: **Crítico**

### Mitigadores
- One-page comercial sóbrio com limites explícitos
- Checklist de “palavras proibidas” (rentabilidade garantida, liquidez etc.)
- Contrato com cláusulas claras: não aconselhamento, não oferta, não captação
- Aprovação de comunicação por alguém com noção regulatória (mesmo que seja você + advogado)

---

## 3) Jurídico do ativo (ônus, matrícula, contratos)

### Risco
Problemas no imóvel (ônus, penhoras, disputas, irregularidade documental) inviabilizarem a tese.

### P/I
P: Média | I: Alto | Nível: **Alto**

### Mitigadores
- Diligência documental mínima (matrícula, ônus, certidões, contratos)
- Data room com checklist obrigatório
- “Gates” (etapas) antes de avançar (ex.: sem matrícula limpa, não avança)

---

## 4) Fraude do originador / operador / prestador

### Risco
Dados falsos, contratos simulados, receitas inventadas, superfaturamento de CAPEX.

### P/I
P: Média | I: Alto | Nível: **Alto**

### Mitigadores
- Evidências: extratos, recibos, confirmação de pagamento/ocupação
- Auditoria amostral de contratos (ligação/validação independente)
- Separação de funções (quem origina não “auto-audita”)
- Registros e trilhas (quem subiu o documento, quando, qual versão)

---

## 5) Operacional (processos, controles, relatórios)

### Risco
Relatórios inconsistentes, falta de rotina, dados bagunçados → quebra de confiança.

### P/I
P: Alta | I: Médio/Alto | Nível: **Alto**

### Mitigadores
- Template de relatório mensal + checklist de fechamento
- Calendário de rotinas (D+5, D+10 etc.)
- “Fonte da verdade” definida (planilha/ERP/documento)
- Controle de versões no Git para templates e metodologias

---

## 6) PLD/FT (KYC/AML) inadequado ao risco

### Risco
Ausência de identificação e monitoramento mínimo, abrindo brecha para ilícitos e risco reputacional.

### P/I
P: Média | I: Alto | Nível: **Alto**

### Mitigadores
- Checklist KYC v1 (cadastro, validação, monitoramento)
- Política baseada em risco (perfil do cliente e origem de recursos)
- Registro de decisões (por que aprovou/reprovou)
- Mínimo de rastreabilidade interna (sem coletar dados desnecessários)

---

## 7) Tecnologia (segurança, integridade, disponibilidade)

### Risco
Vazamento de documentos, alteração de dados, indisponibilidade, acesso indevido ao data room.

### P/I
P: Média | I: Alto | Nível: **Alto**

### Mitigadores
- Controle de acesso por função (RBAC)
- Logs de acesso e auditoria
- Backups e retenção
- “Menos é mais”: MVP simples, sem inventar blockchain sem necessidade
- Proteção de dados sensíveis (LGPD como higiene)

---

## 8) Custódia / movimentação de dinheiro (evitar no começo)

### Risco
Você (ou sua empresa) virar ponto de custódia, recebimento ou repasse de recursos de terceiros.

### P/I
P: Baixa/Média | I: Alto | Nível: **Alto**

### Mitigadores
- Regra: **não tocar dinheiro de terceiros**
- Se surgir necessidade, estruturar com instituição/parceiro adequado (fora do escopo inicial)

---

## 9) Risco contratual (escopo mal definido)

### Risco
Cliente achar que você “garante resultado financeiro” ou que você é responsável por decisões de investimento.

### P/I
P: Média | I: Alto | Nível: **Alto**

### Mitigadores
- Contrato com limites (não oferta, não aconselhamento, não captação)
- Escopo detalhado + entregáveis + aceite
- Registro de reuniões e decisões

---

## 10) Risco estratégico (começar pela rota errada)

### Risco
Tentar começar por oferta/crowdfunding/fundo sem maturidade operacional → colapso.

### P/I
P: Média | I: Alto | Nível: **Alto**

### Mitigadores
- Começar por B2B Infra/Governança
- Pilotar com 1 caso completo (data room fake + memo)
- Só migrar para rota regulada com parceiro jurídico/operacional forte

---

## Saída prática
Esta matriz deve ser usada para:
- “go/no-go” de projetos
- pauta com advogado/gestor (o que realmente importa)
- definir MVP e controles mínimos

## Status
- [x] Versão 0.1 (operacional)
- [ ] Revisão após 1º estudo de caso
- [ ] Versão estável
