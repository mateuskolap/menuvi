# 🎙️ Menuvi — Roteiro de Entrevista de Validação com Nutricionistas

> **Produto:** Menuvi (`menuvi.com.br`)  
> **Objetivo:** Validar se nutricionistas enxergam valor real na proposta do Menuvi, identificar deal-breakers, calibrar a aceitação da IA (geração + visão computacional) e testar a viabilidade do modelo financeiro híbrido (SaaS + split).
>
> **Regra de ouro:** Você está ali para **ouvir**, não para vender. Se o nutricionista não enxergar valor por conta própria na solução da dor dele, nenhuma funcionalidade extra vai resolver.

---

## ⚠️ Regras Para Não Fugir do Escopo

Antes de iniciar qualquer entrevista, tenha isso em mente:

> [!CAUTION]
> Durante as entrevistas, nutricionistas **vão sugerir dezenas de funcionalidades** (ex: módulo de exames laboratoriais complexos, teleconsulta com vídeo ao vivo, prescrição de manipulados/fitoterápicos, nutrição pediátrica). Anote tudo no feedback, mas **não prometa nada**. O escopo rígido do MVP do Menuvi é composto por:
>
> 1. **Cadastro com Validação de CRN:** Verificação automatizada na API do CFN (garantindo que apenas nutricionistas ativos acessem a plataforma).
> 2. **Gestão de Pacientes e Anamnese:** Paciente só entra no app mediante link exclusivo gerado pelo seu nutricionista, com onboarding via anamnese configurável pelo profissional (ou com template padrão pronto do sistema).
> 3. **Copiloto de IA com Tabelas Oficiais:** Geração de rascunhos de cardápios (1 a 30 dias) fundamentados exclusivamente nas tabelas TACO, TBCA e USDA, com cálculo nutricional 100% determinístico no banco de dados (IA nunca inventa calorias).
> 4. **Aprovação Obrigatória (Human-in-the-Loop):** Editor visual web onde o nutricionista ajusta e formalmente aprova/assina o plano antes que fique visível ao paciente.
> 5. **Diário Alimentar com Foto e Visão Computacional:** Paciente registra fotos das refeições e a IA apoia na pré-identificação dos alimentos para acelerar a conferência.
> 6. **Painel de Adesão:** Timeline diária para o nutricionista acompanhar refeições registradas e adesão do paciente.
> 7. **Módulo Financeiro Integrado:** Gestão de planos de atendimento (avulsos, assinaturas recorrentes ou pacotes parcelados) com cobrança automatizada (Pix, cartão, boleto via Asaas) sob modelo híbrido: mensalidade SaaS (~R$ 99/mês) + split retido por transação para custeio de IA e gateway.
>
> **Tudo o que não estiver nessa lista é backlog futuro, fora do MVP.**

---

## Como Conduzir a Entrevista

- **Duração:** 25 a 35 minutos no máximo.
- **Formato:** Conversa fluida e investigativa, não leitura de questionário. Use as perguntas como norte.
- **Gravação:** Grave o áudio com permissão prévia do profissional para não perder nuances e citações exatas.
- **Amostra recomendada:** 8 a 10 nutricionistas (mínimo absoluto de 5).
- **Diversidade de perfis:** Recém-formados (até 2 anos), profissionais consolidados (5+ anos), donos de consultório físico, autônomos que atendem 100% online e nutricionistas que trabalham com pacotes de acompanhamento recorrente.

---

## Bloco 1 — Rotina e Dores Atuais (Entender a realidade ANTES de falar da solução)

> **Objetivo:** Descobrir se as dores que o Menuvi se propõe a resolver são sentidas de forma intensa no cotidiano do profissional.

### Pergunta 1
**"Como funciona a sua rotina com seus pacientes hoje? Me conta o passo a passo desde a primeira consulta até o retorno e acompanhamento."**

> 🔍 *O que observar:* Em quais etapas ele gasta mais energia. Como ele realiza a anamnese inicial (se usa formulário próprio no Google Forms, papel, ou a anamnese engessada de outros softwares). Quais canais utiliza (WhatsApp pessoal, e-mail, planilhas). Onde ocorrem os maiores gargalos e atritos.

### Pergunta 2
**"Qual é a parte mais demorada, cansativa ou chata do seu trabalho como nutricionista hoje?"**

> 🔍 *O que observar:* Se o profissional cita espontaneamente: (a) o tempo excessivo montando cardápios manuais e calculando macros; (b) a dificuldade de saber se o paciente está cumprindo a dieta no dia a dia; ou (c) o estresse de fazer cobranças e lidar com pagamentos.

### Pergunta 3
**"Como você acompanha se o paciente realmente seguiu o plano entre uma consulta e outra?"**

> 🔍 *O que observar:* Se a resposta for "peço para mandar foto no WhatsApp e me perco nas mensagens" ou "só descubro no retorno que ele não seguiu", temos a validação exata do problema que o diário alimentar do Menuvi resolve.

### Pergunta 4
**"Você utiliza algum software ou ferramenta hoje para prescrever planos e gerenciar pacientes? O que mais gosta e o que mais te irrita nessas ferramentas?"**

> 🔍 *O que observar:* Concorrentes reais citados (ex: Dietbox, Webdiet, Nutrify, Avanutri, planilhas próprias). Falhas recorrentes: sistemas lentos, apps de pacientes confusos, falta de inteligência real, cálculo engessado ou custo elevado.

### Pergunta 5
**"Em relação à parte financeira do seu consultório: como você estrutura e cobra seus atendimentos hoje? Você vende mais consultas avulsas ou pacotes/acompanhamentos de vários meses? Costuma ter dor de cabeça com cobrança manual por Pix ou atrasos?"**

> 🔍 *O que observar:* Se o nutricionista trabalha com recorrência/pacotes (alinhado ao RF-022 do Menuvi). Se relata constrangimento ou perda de tempo cobrando pacientes no WhatsApp. Se sofre com cancelamentos e inadimplência.

---

## Bloco 2 — Reação ao Conceito do Menuvi (Apresentar a proposta e medir o interesse)

> **Objetivo:** Medir a tração inicial e a reação visceral à proposta de valor central da plataforma.

### Pergunta 6 (O Pitch do Menuvi)
**"Imagina uma plataforma web e app onde você convida seus próprios pacientes. Nela, você pode utilizar um modelo de anamnese padrão pronto para uso ou customizar 100% as perguntas para o paciente responder no app antes da consulta. A partir desses dados, você conta com um copiloto de Inteligência Artificial que monta rascunhos de cardápios completos baseados rigorosamente em tabelas oficiais (como TACO e TBCA) e nas metas do paciente, calculando calorias e macronutrientes de forma exata. Você edita o que quiser no painel e só libera após sua aprovação formal. No app do paciente, ele recebe o plano e registra fotos das refeições, onde a IA pré-identifica os alimentos do prato para você auditar a adesão numa linha do tempo diária. O que você acha dessa proposta?"**

> 🔍 *O que observar na reação:*
> - 😍 **Entusiasmo imediato** (olhos atentos, postura inclinada, começa a fazer perguntas sobre como usar) → Validação forte da proposta de valor.
> - 😐 **"Interessante, legal..."** (tom morno, sem empolgação) → Solução parece conveniente, mas talvez não resolva uma dor urgente para ele.
> - 🤨 **Ceticismo ou ressalvas técnicas** → Escute com muita atenção; aí estão os riscos de adoção e os deal-breakers reais.

### Pergunta 7
**"O que mais te chamou atenção positivamente nisso tudo? E, por outro lado, o que mais te deixou preocupado ou com o pé atrás?"**

> 🔍 *O que observar:* O ponto forte que ele destacar indica a funcionalidade âncora de marketing/vendas. A preocupação revela onde o produto precisa ser mais robusto (geralmente receio de alucinação da IA ou medo de os pacientes não usarem o app).

### Pergunta 8
**"Se essa plataforma existisse exatamente assim hoje, você começaria a usar com seus pacientes? Por quê?"**

> 🔍 *O que observar:* "Sim, com certeza" = forte tração. "Usaria se tivesse X" = identificar a condição essencial. "Acho que não" = aprofundar se o motivo é custo, desconfiança técnica ou hábito consolidado com outra ferramenta.

---

## Bloco 3 — Inteligência Artificial e Segurança Científica (Testar limites e confiança)

> **Objetivo:** Entender a relação do profissional com IA, identificar medos éticos e validar a arquitetura técnica do Menuvi (IA como orquestrador + tabelas oficiais como fonte da verdade).

### Pergunta 9
**"Como você se sentiria ao usar uma IA para gerar o primeiro rascunho de um plano alimentar para você revisar e ajustar? Você confiaria nisso como ponto de partida da sua prescrição?"**

> 🔍 *O que observar:*
> - 🟢 "Economizaria metade do meu tempo" → Pronto para o copiloto.
> - 🟡 "Depende muito da precisão dos alimentos e quantidades" → Exigência de qualidade e rigor técnico.
> - 🔴 "Nutrição é individual, máquina não sabe fazer dieta" → Resistência profunda. Sondar se é preconceito com IA genérica (tipo ChatGPT comum) ou princípio inegociável.

### Pergunta 10 (Validação da Arquitetura Anti-Alucinação)
**"Uma grande preocupação de muitos profissionais é a IA 'alucinar' ou inventar calorias. No Menuvi, a IA nunca calcula nada de cabeça: ela apenas combina alimentos a partir das tabelas oficiais brasileiras (TACO e TBCA), e todo cálculo de calorias e macros é feito de forma matemática e exata pelo sistema. Saber disso mudaria a sua segurança para utilizar a ferramenta?"**

> 🔍 *O que observar:* Se a menção explícita às tabelas TACO/TBCA traz alívio e credibilidade técnica imediata ao nutricionista.

### Pergunta 11 (Validação da Visão Computacional)
**"E no diário alimentar do paciente: se a IA analisar a foto do prato enviada por ele e já sugerir os alimentos identificados para facilitar sua visualização rápida na timeline, você acharia isso útil ou preferiria olhar apenas a foto pura?"**

> 🔍 *O que observar:* Se ele enxerga economia de tempo em ter os alimentos pré-rotulados na foto ou se teme falsos positivos da IA na identificação de alimentos misturados.

### Pergunta 12
**"Você prefere que o paciente saiba que o plano contou com auxílio de tecnologia de IA na montagem preliminar (com sua revisão e aprovação), ou prefere que a presença da IA seja 100% de bastidor (invisível para o paciente)?"**

> 🔍 *O que observar:* Sensibilidade sobre a percepção de valor do próprio trabalho clínico. Define as diretrizes visuais do app do paciente e relatórios.

### Pergunta 13
**"O que você considera que a IA JAMAIS deveria fazer em uma plataforma para nutricionistas?"**

> 🔍 *O que observar:* Limites éticos e clínicos considerados inegociáveis pela classe (ex: jamais prescrever direto ao paciente, jamais sugerir condutas patológicas sem intervenção médica, jamais alterar calorias sem aval).

---

## Bloco 4 — Modelo Financeiro e Cobranças (Testar modelo híbrido e disposição a pagar)

> **Objetivo:** Validar a monetização híbrida do Menuvi: mensalidade SaaS fixa (~R$ 99/mês) + split sobre transações para cobrir custos de IA e gateway.

### Pergunta 14
**"Quanto você cobra em média hoje por uma consulta avulsa e quanto cobra por um acompanhamento continuado (ex: plano trimestral ou semestral)?"**

> 🔍 *O que observar:* Faixa de preços praticada no mercado real. Permite calcular o impacto exato do modelo de split e o retorno financeiro que o sistema proporciona ao profissional.

### Pergunta 15 (Validação da Automação de Cobranças)
**"Se o sistema oferecesse cobrança automatizada para seus pacientes — permitindo gerar links de pagamento, Pix automático com QR code, cartão de crédito com cobrança recorrente mensal ou parcelamento em até 12x — o quanto isso resolveria problemas de tempo ou inadimplência no seu consultório?"**

> 🔍 *O que observar:* Se a intermediação de cobrança é vista como um grande diferencial agregador de valor ou se o profissional é indiferente porque já possui máquina de cartão própria ou cobra em dinheiro.

### Pergunta 16 (Validação do Modelo Híbrido: SaaS R$ 99 + Split de Transação)
**"Nosso modelo para o Menuvi foi desenhado para ser muito acessível: um plano de assinatura padrão de R$ 99,00/mês para uso ilimitado da plataforma web e do app pelos seus pacientes (com condições promocionais de entrada para os primeiros meses, por exemplo R$ 49,90/mês nos primeiros 3 meses), combinada a uma pequena taxa percentual retida sobre os pagamentos que seus pacientes fizerem pelo app (apenas para cobrir o processamento bancário e os custos dos servidores de IA). O que você acha desse formato? Você acharia justo ou preferiria pagar uma mensalidade fixa mais alta sem nenhuma taxa sobre suas consultas?"**

> 🔍 *O que observar:*
> - Se a condição de entrada (ex: R$ 49,90) e o valor regular de **R$ 99,00** soam atrativos perante softwares consolidados do mercado (que cobram entre R$ 80 e R$ 180 sem IA avançada).
> - Se a taxa percentual do split gera objeção ("não gosto que mexam no valor da minha consulta") ou se é vista com naturalidade ("já pago taxa na maquininha de cartão mesmo, então tudo bem se substituir").
> - Qual modelo ele defenderia como ideal para o seu perfil.

### Pergunta 17
**"Depois de começar a usar um software como esse, o que faria você cancelar a assinatura e abandonar a plataforma?"**

> 🔍 *O que observar:* Principais gatilhos de churn: pacientes com dificuldade de usar o app, bugs no gerador de dietas, lentidão, lentidão no repasse do dinheiro ou preço incompatível com o volume de pacientes.

---

## Bloco 5 — Ética, Legislação e Segurança (Validar blindagem regulatória e LGPD)

> **Objetivo:** Confirmar se as proteções regulatórias do Menuvi (CFN, LGPD e validação de registro) estão alinhadas às exigências da categoria.

### Pergunta 18
**"Você teria algum receio ético ou medo de questionamento por parte do CRN/CFN ao utilizar uma ferramenta com IA que atua como copiloto nas suas prescrições?"**

> 🔍 *O que observar:* Grau de conhecimento das resoluções do CFN (Resolução CFN nº 599/2018). Confirmação de que a presença obrigatória do nutricionista revisando e assinando o plano neutraliza o risco de infração ética.

### Pergunta 19 (Validação da Barreira de Entrada via CRN Ativo)
**"O Menuvi faz uma verificação ativa na base do Conselho Federal de Nutricionistas para liberar o cadastro apenas de profissionais com registro ATIVO no CRN, bloqueando coaches, personals ou leigos. Essa barreira de entrada faz diferença para você na hora de escolher um software?"**

> 🔍 *O que observar:* Senso de valorização e proteção da categoria contra a atuação ilegal de falsos profissionais na internet.

### Pergunta 20
**"Sobre dados clínicos de saúde dos seus pacientes e fotos de refeições ficarem armazenados em nuvem: qual o seu nível de preocupação com a LGPD e sigilo profissional? Você exige algo específico de segurança?"**

> 🔍 *O que observar:* Preocupação real com vazamento de dados de saúde (dados sensíveis). Se a conformidade com criptografia e política de privacidade transparente serve como argumento forte de contratação.

### Pergunta 21
**"Se um paciente tivesse qualquer reação adversa ou dúvida sobre a alimentação — mesmo tendo seguido o plano gerado com auxílio da IA — de quem você considera que é a responsabilidade técnica e civil? Do profissional, do software, ou de ambos?"**

> 🔍 *O que observar:* Alinhamento sobre a responsabilidade clínica. Se o nutricionista assume com naturalidade que a responsabilidade é 100% dele (pois ele é quem revisa e prescreve), o modelo do Menuvi opera em segurança jurídica. Se ele esperar que a IA assuma a culpa médica, há um desalinhamento sério.

---

## Bloco 6 — Fechamento e Próximos Passos (Medir intenção real de adoção)

> **Objetivo:** Separar elogios cordiais de intenção genuína de uso imediato.

### Pergunta 22
**"Se o Menuvi estivesse disponível no próximo mês com essas funcionalidades (gerador com IA e tabelas TACO/TBCA, diário por fotos, cobrança integrada e valor promocional de entrada de R$ 49,90/mês), você toparia ser um dos nossos primeiros usuários beta para testar com alguns pacientes?"**

> 🔍 *O que observar:* "Sim, pode me colocar na lista" e pedir prazo = intenção de compra altíssima. "Me avisa quando tiver mais coisas" = ainda não enxergou benefício suficiente no MVP.

### Pergunta 23
**"Você tem 1 ou 2 colegas nutricionistas que também sentem essas mesmas dores no consultório e que você poderia me indicar para eu conversar?"**

> 🔍 *O que observar:* Pessoas só indicam colegas de profissão para iniciativas que consideram sérias e relevantes. Conseguir indicações é um dos melhores sinais de tração antecipada.

### Pergunta 24
**"Se você pudesse nos dar UM único conselho sobre o que não podemos errar de jeito nenhum nesse produto, qual seria?"**

> 🔍 *O que observar:* O valor mais profundo do profissional sintetizado em uma única resposta.

---

## 📋 Ficha de Consolidação Pós-Entrevista

Preencha imediatamente após o término de cada conversa (enquanto a memória está fresca):

| Critério Avaliado | Registro / Anotação |
|:---|:---|
| **Nome do Profissional / Código** | |
| **Tempo de Formatura / Perfil** | (Recém-formado / 2-5 anos / 5+ anos / Clínica / Autônomo 100% online) |
| **Volume de Pacientes Ativos** | (< 10 / 10 a 30 / 30 a 60 / 60+) |
| **Ticket Médio Praticado** | Consulta avulsa: R$ ______ \| Pacote/Mês: R$ ______ |
| **Ferramenta Principal Atual** | (Dietbox / Webdiet / Nutrify / Excel / Outro) |
| **Nível de Interesse Geral no Menuvi** | 1 (Nenhum) \| 2 (Baixo) \| 3 (Neutro) \| 4 (Alto) \| 5 (Entusiasta) |
| **Maior Dor Validada** | (Tempo de cálculo / Acompanhamento de fotos / Cobrança manual) |
| **Aceitação do Copiloto de IA** | Aceita plenamente \| Aceita com TACO/TBCA \| Resistente |
| **Reação à Visão Computacional (Fotos)** | Muito útil \| Neutro \| Cético |
| **Reação ao Modelo Financeiro** | Aprovou R$ 99 + split \| Prefere só mensalidade fixa \| Rejeitou |
| **Top 1 Preocupação / Objeção** | |
| **Aceitou ser Usuário Beta?** | (Sim / Talvez / Não) |
| **Indicou Colegas?** | (Sim: quantos? / Não) |

---

## 🚩 Sinais de Alerta (Red Flags) — Quando Reavaliar o Produto

Se **3 ou mais** entrevistados manifestarem qualquer uma destas objeções de forma enfática, pare e reavalie o direcionamento:

1. **"Eu jamais confiaria num rascunho de IA, mesmo usando tabelas oficiais"** → A proposta de valor de produtividade não atinge o público-alvo prioritário.
2. **"Meus pacientes não têm paciência de tirar foto de comida no app"** → Risco alto de desengajamento no lado B2C do produto.
3. **"Eu não aceito que o software retenha qualquer porcentagem sobre o que meu paciente me paga"** → O split financeiro pode ser um deal-breaker; o modelo precisaria migrar para mensalidade SaaS pura.
4. **"Já uso [Ferramenta X], ela faz tudo o que preciso e não vejo motivo para trocar"** → O diferencial de IA e fotos não está soando forte o suficiente para superar a inércia de migração.
5. **"O CRN da minha região já notificou profissionais por usarem apps similares"** → Risco regulatório imprevisto que exige consulta jurídica imediata.

---

## ✅ Sinais Verdes (Green Flags) — Sinais de Validação Forte

1. O nutricionista **descreve espontaneamente o cansaço de calcular dietas e macros** antes de você citar o gerador de IA.
2. O nutricionista **desabafa sobre o caos de receber fotos de pratos pelo WhatsApp pessoal**.
3. O nutricionista **elogia o fato de o Menuvi usar as tabelas TACO e TBCA** em vez de cálculos arbitrários de modelos estrangeiros.
4. O nutricionista **pergunta quando o sistema vai ser lançado** e pede para ser avisado primeiro.
5. O nutricionista considera a mensalidade de **R$ 99,00 justa ou barata** em comparação com o tempo que vai economizar.
6. O nutricionista **indica outros profissionais espontaneamente** durante a conversa.
