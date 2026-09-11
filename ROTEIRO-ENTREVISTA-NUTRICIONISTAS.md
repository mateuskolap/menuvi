# 🎙️ Menuvi — Roteiro de Entrevista de Validação com Nutricionistas

> **Produto:** Menuvi (`menuvi.com.br`)  
> **Objetivo:** Validar se nutricionistas enxergam valor real no Menuvi, identificar deal-breakers, e calibrar o escopo do MVP.
>
> **Regra de ouro:** Você está ali para **ouvir**, não para vender. Se o nutricionista não ver valor sozinho, nenhuma feature extra vai resolver.

---

## ⚠️ Regras Para Não Fugir do Escopo

Antes das perguntas, grave isso:

> [!CAUTION]
> Durante as entrevistas, nutricionistas **vão sugerir features**. Anote tudo, mas **não prometa nada**. O escopo do MVP é:
>
> 1. Nutricionista se cadastra (com validação de CRN)
> 2. Nutricionista convida seus clientes
> 3. IA gera rascunhos de planos alimentares que o nutricionista revisa e aprova
> 4. Cliente visualiza o plano e registra refeições (com foto)
> 5. Nutricionista acompanha a adesão do cliente
> 6. Pagamentos intermediados pelo app (com % retido)
>
> **Tudo que não estiver nessa lista é backlog, não é MVP.**

---

## Como Conduzir

- **Duração:** 25-35 minutos
- **Formato:** Conversa, não questionário. Use as perguntas como guia, não como checklist rígido
- **Grave (com permissão):** Você vai esquecer detalhes importantes
- **Entreviste no mínimo 5 nutricionistas**, idealmente 8-10
- **Misture perfis:** recém-formados, experientes, clínica própria, autônomos, que atendem online

---

## Bloco 1 — Dores Atuais (Entender o mundo dele ANTES de apresentar a solução)

> **Objetivo:** Descobrir se as dores que o app resolve são reais e sentidas no dia a dia.

### Pergunta 1
**"Como é o seu dia a dia com seus pacientes? Me conta o fluxo desde a primeira consulta até o acompanhamento."**

> 🔍 *O que observar:* Onde ele demonstra frustração. Ferramentas que ele menciona (planilhas, WhatsApp, apps genéricos). Processos manuais repetitivos.

### Pergunta 2
**"Qual a parte mais trabalhosa ou chata do seu trabalho hoje?"**

> 🔍 *O que observar:* Se ele menciona "montar plano alimentar", "acompanhar se o paciente seguiu", ou "cobrar pacientes". Se mencionar, o app resolve exatamente isso.

### Pergunta 3
**"Como você acompanha se o paciente está seguindo o plano entre uma consulta e outra?"**

> 🔍 *O que observar:* Se a resposta for "não acompanho" ou "peço para mandar foto no WhatsApp", é validação direta do problema.

### Pergunta 4
**"Você usa alguma ferramenta ou software hoje para montar planos alimentares? Qual? O que gosta e o que não gosta?"**

> 🔍 *O que observar:* Quem são os concorrentes reais (Dietbox? Nutrify? Planilhas Excel?). O que falta nessas ferramentas.

---

## Bloco 2 — Reação ao Conceito (Apresentar a ideia e observar a reação genuína)

> **Objetivo:** Medir o nível de interesse real — não o que ele diz, mas como reage.

### Pergunta 5
**"Imagina um app onde você convida seus pacientes, e dentro dele você tem uma IA que gera rascunhos de planos alimentares personalizados com base nas restrições e objetivos do paciente. Você revisa, ajusta o que quiser, e libera para ele. O paciente recebe o plano e tira foto de cada refeição para você acompanhar se está seguindo. O que você acha?"**

> 🔍 *O que observar:*
> - 😍 **Olho brilhou, se inclinou para frente, fez perguntas** → Interesse genuíno
> - 😐 **"Legal, interessante"** (sem entusiasmo) → Educado, mas indiferente
> - 🤨 **Fez ressalvas imediatas** → Escute com atenção, são os deal-breakers reais

### Pergunta 6
**"O que mais te chamou atenção nisso? E o que te preocupa?"**

> 🔍 *O que observar:* O que ele destaca como valioso indica a feature mais importante. O que preocupa indica o que pode impedir a adoção.

### Pergunta 7
**"Se isso existisse hoje, você usaria? Por quê?"**

> 🔍 *O que observar:* "Sim" sem hesitação = validação forte. "Depende de..." = condições que precisam ser atendidas. "Acho que não" = entender por quê.

---

## Bloco 3 — IA Como Ferramenta (Testar aceitação e confiança na IA)

> **Objetivo:** Nutricionistas podem ter resistência à IA. Precisa medir isso.

### Pergunta 8
**"Como você se sentiria usando uma IA que gera um rascunho do plano alimentar para você revisar? Você confiaria nisso como ponto de partida?"**

> 🔍 *O que observar:*
> - 🟢 "Economizaria muito tempo" → Aceita IA como ferramenta
> - 🟡 "Depende da qualidade" → Precisa de demonstração
> - 🔴 "Prefiro fazer tudo eu mesmo" → Resistência. Entender se é medo ou orgulho profissional

### Pergunta 9
**"O que a IA NÃO deveria fazer, na sua opinião?"**

> 🔍 *O que observar:* Limites que o nutricionista considera inegociáveis. Isso define o que a IA pode e não pode no app.

### Pergunta 10
**"Você se sentiria confortável que o plano final — após a sua revisão — mostrasse que foi 'gerado com auxílio de IA'? Ou prefere que isso não apareça para o paciente?"**

> 🔍 *O que observar:* Se ele não quer que o paciente saiba da IA, pode indicar insegurança sobre a percepção de valor do seu próprio trabalho. Isso afeta como o app comunica a feature.

---

## Bloco 4 — Modelo Financeiro (Testar disposição para pagar e o modelo de %)

> **Objetivo:** Descobrir se o modelo de receita é aceitável. Este é o bloco mais sensível.

### Pergunta 11
**"Hoje, quanto você cobra por consulta ou por acompanhamento mensal?"**

> 🔍 *O que observar:* Faixa de preço real do mercado. Essencial para calcular se o % é viável para ambos os lados.

### Pergunta 12
**"Se o app processasse os pagamentos dos seus pacientes — tipo um Uber — e retivesse um percentual por transação, o que você acharia? Qual percentual te pareceria justo?"**

> 🔍 *O que observar:*
> - Se a reação for negativa → o modelo de % pode ser um deal-breaker. Considerar mensalidade fixa
> - Se aceitar → anotar o % que ele considera justo. Se vários disserem "até X%", é o teto do mercado
> - Comparativo: iFood cobra ~27%, Uber ~25%, Doctoralia cobra mensalidade fixa

### Pergunta 13
**"Você preferiria pagar uma mensalidade fixa pelo app ou um percentual sobre cada pagamento recebido?"**

> 🔍 *O que observar:* Nutricionistas com poucos clientes preferem %. Nutricionistas com muitos clientes preferem mensalidade fixa (o % ficaria caro demais). **Isso pode indicar que o modelo ideal é oferecer ambas as opções.**

### Pergunta 14
**"O que faria você parar de usar uma ferramenta assim depois de começar?"**

> 🔍 *O que observar:* Motivos de churn. Se "preço alto" aparecer repetidamente, o % precisa ser competitivo.

---

## Bloco 5 — Preocupações Éticas e Legais (Validar se os riscos que mapeamos são reais)

> **Objetivo:** Confirmar se os riscos que identificamos no brainstorming ressoam com profissionais reais.

### Pergunta 15
**"Você teria alguma preocupação ética ou profissional em usar um app assim? Alguma coisa que o CRN poderia questionar?"**

> 🔍 *O que observar:* Se ele mencionar algo que não mapeamos, é um risco novo. Se não tiver preocupação nenhuma, pode indicar falta de conhecimento sobre as regras do CFN.

### Pergunta 16
**"Sobre os dados dos seus pacientes ficarem na nuvem — isso te preocupa? Você precisaria de algo específico para se sentir confortável?"**

> 🔍 *O que observar:* Nível de preocupação com privacidade. Se for alto, o app precisa de funcionalidades de segurança visíveis (não só internas).

### Pergunta 17
**"Se um paciente tivesse uma reação adversa seguindo um plano gerado com auxílio da IA — mesmo após sua revisão — como você veria a responsabilidade? Do profissional, do app, ou de ambos?"**

> 🔍 *O que observar:* Se o nutricionista entende que a responsabilidade clínica é dele (porque ele revisou e aprovou), o modelo funciona. Se ele esperar que o app assuma a responsabilidade, há um desalinhamento perigoso.

---

## Bloco 6 — Decisão Final (Medir intenção real de uso)

> **Objetivo:** Separar interesse polido de intenção real.

### Pergunta 18
**"Se esse app existisse hoje e custasse [X% ou R$Y/mês], você assinaria agora?"**

> 🔍 *O que observar:* "Sim, agora" = validação forte. "Quando tiver mais features" = não resolveu a dor principal ainda. "Vou pensar" = provavelmente não.

### Pergunta 19
**"Você conhece outros nutricionistas que teriam interesse? Me indicaria alguém para conversar?"**

> 🔍 *O que observar:* Se ele indica, o interesse é real. Pessoas não indicam coisas que não acreditam para colegas.

### Pergunta 20
**"Se você pudesse mudar ou adicionar UMA COISA nessa ideia, o que seria?"**

> 🔍 *O que observar:* A resposta mais repetida entre os entrevistados é a feature mais importante que pode estar faltando. **Anote, mas não prometa.**

---

## 📋 Checklist Pós-Entrevista

Após cada entrevista, preencha imediatamente (antes de esquecer):

| Item | Resposta |
|:-----|:---------|
| **Nome (ou código)** | |
| **Perfil** (recém-formado / experiente / clínica / autônomo) | |
| **Nível de interesse** (1-5) | |
| **Dor principal que o app resolve** | |
| **Maior preocupação / objeção** | |
| **Aceitação da IA** (aceita / com ressalvas / rejeita) | |
| **Modelo financeiro preferido** (% / mensalidade / ambos) | |
| **% máximo aceitável** | |
| **Usaria hoje?** (sim / com condições / não) | |
| **Indicou colegas?** (sim / não) | |
| **Feature mais pedida** | |
| **Red flag identificada** | |

---

## 🚩 Red Flags — Se Aparecerem, Pare e Reavalie

Se **3 ou mais** nutricionistas mencionarem qualquer um destes, é sinal de alerta sério:

1. **"Eu não confiaria numa IA para gerar planos"** → A proposta de valor central não funciona para o público
2. **"Meus pacientes não usariam app"** → O cliente final pode não adotar
3. **"Eu jamais pagaria % sobre minhas consultas"** → O modelo de receita precisa mudar
4. **"O CRN não permitiria isso"** → Risco regulatório que não mapeamos
5. **"Já uso [ferramenta X] e estou satisfeito"** → Concorrente forte, precisa oferecer muito mais

---

## ✅ Sinais Positivos — Se Aparecerem, Você Está no Caminho Certo

1. **Nutricionista pede para ser avisado quando lançar**
2. **Nutricionista indica colegas espontaneamente**
3. **Nutricionista descreve exatamente o problema que o app resolve ANTES de você apresentar**
4. **Nutricionista pergunta preço antes de você falar**
5. **Nutricionista reclama das ferramentas atuais**
