# Entrega 4 — Cenários de análise/problema

**Data:** {{dd/mm/aaaa}}  
**Status:** 🟨 em andamento
**Responsabilidade:** 1 solução completa por integrante

## Objetivo da atividade

Descrever situações atuais em que o usuário tenta alcançar um objetivo e encontra dificuldades. O cenário de análise/problema deve tornar visível **o contexto, os atores, as ações e as rupturas**, sem antecipar a interface que será projetada.

> **Regra central:** cenário de problema é a “história do problema”. Se o texto já diz “o sistema mostra”, “o aplicativo resolve” ou descreve botões/telas futuras, provavelmente está misturando problema com solução.

Sempre que possível, o cenário deve aprofundar uma **situação concreta já registrada na Entrega 1**.

### Quando o TCC não possuía interface

O cenário continua sendo uma história de **problema/atividade humana**, não uma história do futuro sistema. Descreva como o profissional realiza hoje uma atividade semelhante ou como lida atualmente com dados, resultados, configurações, logs, decisões e limitações que o tema do TCC pretende apoiar.

Exemplo: em vez de “o DBA abre o novo dashboard e executa o algoritmo”, descreva “o DBA precisa investigar uma consulta lenta, reúne informações em ferramentas distintas, compara planos manualmente e tem dificuldade para estimar o impacto de uma mudança”.

A interface da disciplina aparecerá somente depois, nos cenários de interação.

Se o integrante escolher um novo problema/situação, explique por que ele passou a ser relevante e indique a evidência que motivou sua inclusão.

## Cenário C01 — {{título}}

**Autor(a):** Caio Arnoni - 22.221.019-7  
**Persona(s) relacionada(s):** P01 - Rafael Costa, protagonista; P03 - Maria Fonseca, colaboradora envolvida.   
**Necessidade relacionada:** N01 - interpretar sem confundir eixos; N02 - reconhecer limites dos dados; N03 - considerar contexto humano; N06 - acompanhar retorno e ação. 
**Situação concreta da Entrega 1 relacionada:** seção 4.5, investigação manual de uma mudança; seções 3.1, 4.1-4.4; atividades A01, A03 e A04.  
**Hipóteses ainda presentes:** H01, H02, H05, H06, H07 e H08. 

### 1. Cenário inicial

Durante uma semana de trabalho híbrido, Rafael Costa, gestor de uma equipe de desenvolvimento, percebe que as mensagens de Maria Fonseca estão mais curtas e objetivas. Ele precisa entender se há alguma dificuldade de trabalho que justifique uma conversa de apoio. No computador, consulta as conversas profissionais às quais já tem acesso e o quadro de tarefas da equipe. Os cartões de Maria parecem seguir os prazos combinados, mas Rafael não consegue reconstruir com segurança se o padrão de comunicação realmente mudou ou se está se baseando apenas nas mensagens mais recentes. Ao alternar entre conversas e tarefas, encontra informações sem uma ligação clara entre si. Termina a consulta sem saber como abordar a situação sem transformar uma impressão em julgamento sobre a colaboradora.

### 2. Questões de refinamento

Use os tipos de questões/taxonomia definidos na aula. As perguntas devem revelar informações **ainda ausentes** do cenário, não repetir o que já foi respondido.

| # | Questão | Por que precisa ser respondida | Fonte/forma de obter resposta |
|---|---|---|---|
| Q1 | Por que Rafael precisa decidir como abordar a situação naquele momento, e não em outra ocasião? | Identificar o gatilho e a consequência de adiar a análise | Entrevista com gestor sobre um episódio recente e sua agenda, sem coletar conteúdo privado |
| Q2 | Como o tempo disponível, o local e as interrupções condicionam essa consulta? | Delimitar restrições concretas de execução | Observação contextual consentida ou relato da rotina de revisão |
| Q3 | De quem depende a informação sobre a complexidade das tarefas e sobre acordos de comunicação da equipe? | Identificar conhecimento que não está nos registros consultados | Entrevistas com gestor e colaboradores sobre responsabilidades e acordos |
| Q4 | Como Rafael escolhe um período de comparação e organiza a busca para não depender só da memória? | Tornar explícita a estratégia de investigação | Reconstrução de uma tarefa real com materiais autorizados ou fictícios |
| Q5 | O que Rafael considera evidência de uma mudança de comunicação e quais atributos dos registros consegue conferir? | Distinguir impressão, frequência, conteúdo, data e situação da tarefa | Entrevista com exemplos fictícios de mensagens e cartões |
| Q6 | Conferir os cartões concluídos permite confirmar, sozinho, se houve mudança de comunicação? | Testar a relação entre fontes e impedir que uma dimensão substitua a outra | Discussão de casos contrastantes com gestores; sem avaliar colaboradores reais |
| Q7 | Como Rafael reage se uma mensagem posterior contradiz sua impressão inicial? | Compreender revisão da interpretação e continuidade da atividade | Entrevista por incidente crítico, incluindo evidências contraditórias |
| Q8 | Como Rafael reconhece que tem contexto suficiente para conversar e como retoma o que foi combinado? | Identificar critério de conclusão e risco de perda de acompanhamento | Relato de acompanhamentos anteriores e análise de registros autorizados |
### 3. Cenário refinado

Durante uma semana de trabalho híbrido, Rafael Costa percebe que as mensagens de Maria Fonseca estão mais curtas e objetivas. Ele precisa entender se há alguma dificuldade de trabalho que justifique uma conversa de apoio. **[NOVO - H; C01.Q1: A conversa individual já combinada com Maria acontecerá naquela tarde. Rafael quer chegar preparado para perguntar sobre o trabalho, sem levar uma avaliação previamente fechada.]** **[NOVO - H; C01.Q2: Ele está em casa, usando o notebook, e dispõe de vinte minutos antes de outra reunião. Uma solicitação de alinhamento interrompe a consulta e o obriga a retomar o ponto em que estava.]**

Rafael consulta as conversas profissionais às quais já tem acesso e o quadro de tarefas. **[NOVO - H; C01.Q3: Ele conhece os prazos, mas depende de Maria e do responsável pelo produto para compreender mudanças recentes na complexidade das demandas; os acordos sobre comunicação foram discutidos em reunião e não aparecem nos cartões.]** **[NOVO - H; C01.Q4: Decide comparar as conversas da última semana com as da semana anterior e anota referências em um arquivo de trabalho restrito, tentando relacioná-las às tarefas citadas.]**

Os cartões de Maria parecem seguir os prazos combinados. **[NOVO - H; C01.Q5: Nas conversas, Rafael confere datas e lê as mensagens anteriores às respostas curtas. Encontra trocas recentes mais frequentes, mas não tem uma contagem completa nem sabe se os trechos consultados representam toda a semana.]** **[NOVO - H; C01.Q6: A consulta aos cartões não confirma, por si só, uma mudança comunicacional: cumprir prazos informa sobre aquelas entregas, não sobre a causa ou o significado do modo de escrever.]**

**[NOVO - H; C01.Q7: Enquanto reúne as referências, Maria envia uma explicação técnica detalhada. Rafael percebe que esse exemplo contraria sua impressão de respostas sempre curtas e revê a anotação, mas continua sem saber a extensão da mudança.]** Ao alternar entre conversas, tarefas e anotações, não consegue estabelecer uma comparação segura dentro do tempo disponível.

**[NOVO - H; C01.Q8: Rafael considera necessário distinguir fatos de impressões e ouvir Maria antes de decidir um acompanhamento. Anota perguntas para a conversa e reserva um momento para retomar eventual acordo; não possui ainda uma explicação confirmada nem uma decisão sobre apoio.]** A preparação termina incompleta: ele identifica dúvidas pertinentes, mas permanece com o risco de dar peso excessivo a exemplos isolados ou perder informações ao retomar o assunto.

{{narrativa refinada}}

### 4. Elementos extraídos

| Elemento | Evidência no cenário |
|---|---|
| Ator(es) | Rafael investiga; Maria fornece seu contexto; o responsável pelo produto conhece mudanças nas demandas (C01.Q3) |
| Objetivo(s) | Preparar uma conversa de apoio sem pressupor uma avaliação negativa (C01.Q1) |
| Contexto | Trabalho híbrido; notebook em casa; vinte minutos e interrupção antes de outra reunião (C01.Q2) |
| Recursos/informações | Conversas autorizadas, datas, contexto das respostas, cartões e arquivo restrito de anotações (C01.Q4-Q5) |
| Ações | Consultar, ler trechos anteriores, anotar referências, conferir cartões e reformular uma anotação (C01.Q4-Q7) |
| Problemas/rupturas | Registros dispersos, amostra incompleta, dependência de memória e contexto não registrado |
| Consequências | Preparação incompleta, retrabalho e risco de abordagem injusta; nenhuma decisão punitiva ocorre na narrativa |

### 5. Implicações para as próximas entregas

- **Tarefa a analisar:** reunir evidências de um período, avaliar se são suficientes e preparar uma conversa de acompanhamento. O foco é a tarefa humana anterior à interpretação de qualquer sinal automatizado.
- **Informações a coletar:** estratégias reais de comparação, fontes autorizadas, tempo disponível, critérios para conversar e modo de retomar acordos.
- **Questão de investigação:** como o gestor diferencia mudança de comunicação, andamento das entregas e contexto não registrado?
- **Limite:** exemplos isolados não autorizam inferir causa, estado emocional ou desempenho global. As janelas de duas semanas da narrativa são escolhas fictícias de Rafael, não alteração dos períodos experimentais do TCC.

## Cenário C02 — Preparação de conversa de acompanhamento sob pressão de tempo

**Autor(a):** Guilherme Matias - 22.122.071-8  
**Persona(s) relacionada(s):** P02 - João Pedro, protagonista; {{P0X - nome}}, colaboradora envolvida.  
**Necessidade relacionada:** N02 - reconhecer limites dos dados; N03 - considerar contexto humano; N06 - acompanhar retorno e ação; {{N0X - obter leitura simples antes do detalhe}}.  
**Situação concreta da Entrega 1 relacionada:** {{seção 4.5, investigação manual de uma mudança; seções correspondentes}}.  
**Hipóteses ainda presentes:** {{H0X, H0Y}}.

### 1. Cenário inicial

Em uma semana de trabalho presencial e híbrido, João Pedro, gestor de operações de uma equipe de atendimento ao cliente, percebe que Camila Duarte, atendente da equipe, tem respondido de forma mais seca nos canais internos e passou a aparecer menos nas conversas informais. Ele precisa decidir se isso merece uma conversa de apoio ou se é só uma fase corrida. Entre duas reuniões, abre a planilha de escalas, o sistema de chamados e o canal de chat da equipe, aos quais já tem acesso. Os chamados de Camila parecem fechados dentro das metas, mas João não consegue saber se houve mudança real ou se está reagindo a poucas mensagens recentes. Como as informações estão em ferramentas separadas, ele não consegue ligá-las com segurança. Termina a consulta sem saber se "precisa se preocupar ou não" e com receio de tratar uma impressão como fato sobre a colaboradora.

### 2. Questões de refinamento

| # | Questão | Por que precisa ser respondida | Fonte/forma de obter resposta |
|---|---|---|---|
| Q1 | Por que João precisa decidir isso agora, e não na próxima reunião de acompanhamento? | Identificar o gatilho e a consequência de adiar a análise | Entrevista com gestor sobre um episódio recente, sem coletar conteúdo privado |
| Q2 | Quanto tempo João tem, onde faz a consulta e quais interrupções ocorrem? | Delimitar restrições de execução e de privacidade | Observação contextual consentida ou relato da rotina entre reuniões |
| Q3 | Que informação sobre a carga e a rotina da equipe não aparece nos registros e depende de outras pessoas? | Identificar conhecimento externo às ferramentas | Entrevistas com gestor, supervisores e atendentes sobre escalas, picos e acordos |
| Q4 | Como João escolhe o período de comparação e evita depender da memória? | Tornar explícita a estratégia de investigação | Reconstrução de uma tarefa real com materiais autorizados ou fictícios |
| Q5 | O que João considera sinal de mudança e quais atributos dos registros consegue conferir? | Distinguir impressão, frequência, conteúdo, data e situação do chamado | Entrevista com exemplos fictícios de mensagens, escalas e chamados |
| Q6 | Conferir as metas de atendimento permite concluir, sozinho, que não há problema (ou que há)? | Impedir que uma fonte substitua a outra | Discussão de casos contrastantes com gestores, sem avaliar colaboradores reais |
| Q7 | Como João reage se um dado novo contradiz a primeira impressão? | Compreender revisão da interpretação e continuidade da tarefa | Entrevista por incidente crítico, incluindo evidências contraditórias |
| Q8 | Como João decide que já sabe o suficiente para conversar e como registra e retoma o que foi combinado? | Identificar critério de conclusão e risco de perder o acompanhamento | Relato de acompanhamentos anteriores e análise de registros autorizados |

### 3. Cenário refinado

Em uma semana de trabalho presencial e híbrido, João Pedro percebe que as mensagens de Camila Duarte estão mais secas e que ela participa menos das conversas informais. Ele precisa decidir se isso merece uma conversa de apoio. **[NOVO - H; C02.Q1: A reunião individual mensal já está marcada para o dia seguinte. João quer chegar com uma ideia clara do que perguntar, sem uma conclusão fechada e com algo que possa justificar depois, se a conversa for difícil.]** **[NOVO - H; C02.Q2: Ele está em uma sala compartilhada, com quinze minutos entre duas reuniões. Um supervisor o chama para resolver uma escala e ele precisa recomeçar a consulta, sem lembrar onde parou. Há outras pessoas por perto, o que o faz evitar deixar nomes e mensagens abertos na tela.]**

João abre a planilha de escalas, o sistema de chamados e o canal de chat da equipe. **[NOVO - H; C02.Q3: Ele conhece as metas, mas depende do supervisor para saber que as últimas duas semanas tiveram pico de demanda e troca de turnos, informação que não consta nas ferramentas. Os combinados sobre como a equipe se comunica no chat foram feitos em reunião e não estão registrados.]** **[NOVO - H; C02.Q4: Decide comparar as duas últimas semanas com as duas anteriores e anota o que encontra em um arquivo restrito, sem saber ao certo como relacionar chat, escalas e chamados.]**

Os chamados de Camila parecem fechados dentro das metas. **[NOVO - H; C02.Q5: No chat, João confere datas e lê as mensagens anteriores às respostas secas. Nota trocas mais curtas nos últimos dias, mas não tem uma contagem completa nem sabe se os trechos que leu representam toda a semana.]** **[NOVO - H; C02.Q6: Os chamados dentro da meta informam sobre aquelas entregas, mas não confirmam nem descartam mudança no modo de se comunicar, nem explicam a causa. João percebe que "meta cumprida" não responde à sua pergunta.]**

**[NOVO - H; C02.Q7: Enquanto anota, vê que Camila escreveu uma explicação longa e cuidadosa para um colega de outro turno. Isso contraria sua impressão de respostas sempre secas, e ele corrige a anotação, mas continua sem saber a extensão da mudança.]** Ao alternar entre planilha, chamados, chat e anotações, não consegue chegar a uma resposta simples dentro do tempo disponível.

**[NOVO - H; C02.Q8: João conclui que não deve agir só com o que viu e que precisa ouvir Camila antes de qualquer decisão. Anota duas perguntas abertas para a conversa e combina consigo mesmo registrar, logo depois, o que ouviu e o que ficou combinado; não possui ainda uma explicação confirmada nem uma decisão sobre apoio.]** A preparação termina incompleta: ele sabe que precisa conversar, mas permanece inseguro sobre o peso de poucos exemplos e com receio de perder o que foi combinado se não registrar.

### 4. Elementos extraídos

| Elemento | Evidência no cenário |
|---|---|
| Ator(es) | João investiga; Camila fornece seu contexto; o supervisor conhece picos de demanda e trocas de turno (C02.Q3) |
| Objetivo(s) | Chegar à conversa de apoio com uma leitura simples da situação e sem avaliação fechada (C02.Q1) |
| Contexto | Trabalho presencial/híbrido; sala compartilhada; quinze minutos e interrupção entre reuniões (C02.Q2) |
| Recursos/informações | Planilha de escalas, sistema de chamados, canal de chat, datas, contexto das respostas e arquivo restrito de anotações (C02.Q4-Q5) |
| Ações | Consultar, ler trechos anteriores, anotar, conferir chamados, corrigir uma anotação e preparar perguntas (C02.Q4-Q8) |
| Problemas/rupturas | Ferramentas separadas, amostra incompleta, dependência de memória, interrupções e contexto não registrado |
| Consequências | Preparação incompleta, retrabalho e risco de abordagem injusta; nenhuma decisão punitiva ocorre na narrativa |

### 5. Implicações para as próximas entregas

- **Tarefa a analisar:** reunir evidências de um período, avaliar se são suficientes, chegar a uma leitura simples e registrar o encaminhamento após a conversa. O foco é a tarefa humana anterior à interpretação de qualquer sinal automatizado.
- **Informações a coletar:** como gestores com pouca familiaridade com dados decidem se "há algo a observar", o que consideram suficiente para conversar, o tempo real disponível e como registram e retomam acordos.
- **Questão de investigação:** como o gestor operacional diferencia mudança de comunicação, cumprimento de metas e contexto não registrado, quando tem pouco tempo e pouca familiaridade com métricas?
- **Limite:** exemplos isolados não autorizam inferir causa, estado emocional ou desempenho global. As janelas de duas semanas da narrativa são escolhas fictícias de João, não alteração dos períodos experimentais do TCC.

## Cenário C03 — {{título}}

**Autor(a):** Taina - RA:  
**Persona(s) relacionada(s):** {{P01}}  
**Necessidade relacionada:** {{R01}}  
**Situação concreta da Entrega 1 relacionada:** {{seção 4.4 / H01 / outra ou “nova situação justificada”}}  
**Hipóteses ainda presentes:** {{H01, H02 ou —}}

### 1. Cenário inicial

{{narrativa}}

### 2. Questões de refinamento

Use os tipos de questões/taxonomia definidos na aula. As perguntas devem revelar informações **ainda ausentes** do cenário, não repetir o que já foi respondido.

| # | Questão | Por que precisa ser respondida | Fonte/forma de obter resposta |
|---|---|---|---|
| Q1 | {{...}} | {{...}} | {{...}} |

### 3. Cenário refinado

Reescreva o cenário incorporando as respostas. Marque o conteúdo novo de forma consistente (por exemplo, `**[NOVO: ...]**`).

{{narrativa refinada}}

### 4. Elementos extraídos

| Elemento | Evidência no cenário |
|---|---|
| Ator(es) | {{...}} |
| Objetivo(s) | {{...}} |
| Contexto | {{...}} |
| Recursos/informações | {{...}} |
| Ações | {{...}} |
| Problemas/rupturas | {{...}} |
| Consequências | {{...}} |

### 5. Implicações para as próximas entregas

Quais tarefas merecem análise? Quais informações precisam ser coletadas? **Não desenhe a solução ainda.**

> Repita para C02, C03... com autoria individual.

## Checklist

- [ ] Há um cenário completo por integrante.
- [ ] Cada cenário tem título, ator, objetivo, contexto e problema.
- [ ] O cenário possui origem rastreável na Entrega 1 ou justifica claramente a inclusão de uma nova situação.
- [ ] O texto descreve a situação atual, sem antecipar a solução.
- [ ] Para TCC sem interface original, o cenário descreve uma prática humana plausível relacionada à contribuição técnica, e não “a falta de uma tela”.
- [ ] Questões de refinamento acrescentam informação nova.
- [ ] O refinamento mostra claramente o que foi adicionado/alterado.
- [ ] Cenários são diferentes o suficiente para cobrir objetivos/problemas relevantes.
- [ ] Cada cenário está ligado a persona/necessidade na matriz de rastreabilidade.
