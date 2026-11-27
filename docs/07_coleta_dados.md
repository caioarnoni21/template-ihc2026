# Entrega 7 — Coleta de dados, necessidades e aspectos éticos

**Data:** {{17/11/2026}}  
**Status:** 🟩 Concluida

## Objetivo da atividade

Planejar dados necessários para compreender usuários e requisitos de IHC, escolher técnicas adequadas e documentar instrumentos de modo que a aplicação possa ser reproduzida por pessoas diferentes.

## Para escopos de IHC derivados de TCC técnico

Quando o usuário e a interface foram propostos pela disciplina, uma prioridade da coleta é investigar se esse **cenário de uso realmente faz sentido**. Não trate o exercício de comercialização da Entrega 1 como validação de mercado.

Perguntas úteis incluem:

- esse perfil realmente realiza a atividade imaginada?
- quais ferramentas usa hoje?
- quais informações consulta?
- quais decisões toma?
- que vocabulário utiliza?
- quais parâmetros compreende e quais deveriam ser abstraídos?
- precisa de dashboard, histórico, filtros, relatórios ou comparação? Por quê?
- quais erros são frequentes e quais são críticos?
- existem papéis/permissões diferentes?
- que resultados do algoritmo/modelo seriam úteis ou difíceis de interpretar?

Quando o acesso ao perfil profissional for difícil, discuta com o docente alternativas metodológicas (especialistas próximos, dados secundários, literatura, participantes proxy) e registre as limitações. **Não esconda a limitação da amostra.**

## Hipóteses e lacunas prioritárias herdadas da Entrega 1

Antes de decidir “que dados coletar”, retome os itens `[H]` e `[?]` da Entrega 1 e o registro de hipóteses em [`../RASTREABILIDADE.md`](../RASTREABILIDADE.md). A coleta deve responder perguntas reais do projeto, e não apenas produzir um formulário porque a técnica foi solicitada.

| ID | Hipótese/lacuna | Evidência atual | Decisão que depende da resposta | Prioridade |
|---|---|---|---|---|
| H05 | O gestor será usuário direto da interface | Decisão inicial de escopo, sem validação com gestores | Manter ou rever Rafael como usuário direto de T01 | Alta |
| H15 / H18 | Gestores acompanham atividades usando diferentes fontes e contatos | Processo específico ainda não investigado | Integrar a consulta ao processo existente, evitando etapas sem necessidade | Alta |
| H19 / H24 | Histórico individual, indicadores, período e atualização apoiam a interpretação | Informações previstas no TCC, sem validação de utilidade com gestores | Selecionar conteúdo prioritário e detalhes da análise | Alta |
| H10 / H27 / ?03 | Familiaridade com indicadores e vocabulário pode afetar a compreensão | Não investigado com o público | Definir rótulos, explicações e nível inicial de detalhe | Alta |
| H17 / H25 | Interpretações incorretas podem levar a decisões sem contexto | Risco previsto no projeto; compreensão ainda não avaliada com gestores | Definir avisos de limites e tratamento de dados incompletos | Alta |
| H20 / H21 / H22 | Uso pode ocorrer em revisões, no computador e com interrupções | Contexto hipotético da equipe | Priorizar dispositivo, duração do fluxo e retomada | Média |
| H23 | Hierarquia, permissões e confiança influenciam o uso | Efeitos concretos ainda não investigados | Delimitar acesso, exposição de informações e responsabilidades | Alta |

## Parte A — necessidades e requisitos de IHC

> **Responsabilidade:** solução individual por integrante.

### A01 — Caio Arnoni

**Autor(a):** Caio Arnoni — 22.221.019-7

#### Que dados coletar?

| Dado/informação | Hipótese/lacuna relacionada | Por que é necessário | Qual decisão de design pode afetar |
|---|---|---|---|
 Perfil do usuário: responsabilidade de acompanhamento e experiência na função | H05 / H15 | Verificar se o perfil realmente realiza a atividade atribuída a Rafael | Público prioritário e limites de T01 |
| Relação com tecnologia: ferramentas atuais, dispositivo e facilidade de interpretação de indicadores | H10 / H21 / H27 | Conhecer recursos disponíveis e dificuldades, sem presumir domínio técnico | Dispositivo prioritário, apresentação e detalhamento das informações |
| Conhecimento do domínio: entendimento de sinalização, padrão individual e análise incompleta | H17 / H24 / ?03 | Identificar vocabulário e interpretações possíveis | Rótulos, explicações e avisos de insuficiência |
| Conhecimento das tarefas: frequência, etapas de um caso recente, fontes consultadas, decisões e forma de registro | H15 / H18 / H19 / H20 | Verificar se o fluxo consultar–interpretar–registrar faz sentido na prática | Ordem das etapas, necessidade de registro e informações essenciais |
| Contexto: interrupções, tempo disponível, privacidade visual e barreiras de leitura ou interação | H20 / H21 / H22 | Compreender condições que dificultam realizar a tarefa | Retomada, densidade visual e requisitos de acessibilidade sem coleta de diagnósticos |
| Motivações e valores: critérios de confiança, limites de uso e preocupação com consequências sobre colaboradores | H23 / H25 | Entender o que torna o acompanhamento útil e aceitável | Permissões, transparência e limites da decisão apoiada pela interface |


#### De quem coletar?

| Perfil/stakeholder | Critério de inclusão | Relação com persona/público |
|---|---|---|
| Gestores, líderes ou coordenadores de equipes | Pessoas com 18 anos ou mais que acompanham ou acompanharam diretamente colaboradores nos últimos seis meses, independentemente da ferramenta utilizada | Público principal para investigar as hipóteses da persona Rafael Costa (P01) e a tarefa T01 |
| Profissionais de RH com responsabilidade direta pelo acompanhamento de uma equipe | Mesmo critério de experiência recente; responder sobre a própria atividade de acompanhamento, não sobre opiniões genéricas da área | Perspectiva complementar; identificar separadamente na análise para não confundir governança com a rotina de Rafael |

#### Aspectos éticos

Analise voluntariedade, consentimento, minimização de dados, privacidade, riscos, gravação, anonimização, armazenamento e descarte. Não responda apenas “sim, por causa da LGPD”: explique **quais dados e riscos existem neste projeto**.

### A03 — Tainá Cunha Bueno

**Autor(a):** Tainá Cunha Bueno — 22.119.025-9
**Foco:** perspectiva da pessoa afetada pela interpretação (P03 — Maria Fonseca; cenário C03; tarefa T03).

#### Que dados coletar?

| Dado/informação | Hipótese/lacuna relacionada | Por que é necessário | Qual decisão de design pode afetar |
|---|---|---|---|
| Perfil: função, tempo na equipe, modalidade de trabalho e ferramentas de comunicação e tarefas usadas | H06 / H11 / H16 | Verificar se o perfil corresponde à colaboradora representada em P03 | Público de T03 e linguagem do fluxo |
| Como recebe hoje comentários sobre sua comunicação ou participação e como responde | H06 / H23 / C03.Q1, Q7 | Conhecer o processo atual e suas rupturas antes de propor um fluxo | Necessidade (ou não) de um canal de esclarecimento na interface |
| O que gostaria de saber sobre uma análise que a envolve: fontes, finalidade, quem acessa, período | H11 / H28 / C03.Q3 / N07 | Identificar quais informações de transparência importam e em que ordem | Conteúdo de “Sobre minhas análises” (P12/F14) e da explicação (P13/F15) |
| Compreensão de termos como “sinalização”, “padrão individual” e “comunicação mudou” | ?03 / H25 | Verificar se o vocabulário causa leitura avaliativa ou diagnóstica | Rótulos e textos de “o que significa e o que não significa” |
| Preferências de forma e canal para contextualizar: escrita, conversa, com quem | C03.Q5 / H23 | Saber se a alternativa de conversa reservada é necessária | Opções de P14/F16 e regra SR2 do GOMS |
| Limites de privacidade: o que considera pessoal e não compartilharia | C03.Q5 / H28 | Evitar que o fluxo induza a expor dados sensíveis | Avisos preventivos e campos não obrigatórios |
| Critérios de um retorno satisfatório: prazo, conteúdo, registro | C03.Q7, Q8 / N06 | Definir o que conta como tarefa concluída | Estados da solicitação e ações “considero esclarecido” e “pedir nova revisão” |
| Atitude em relação ao uso de uma ferramenta desse tipo e condições de aceitação | H28 / H23 | Avaliar se o fluxo aumenta ou reduz a percepção de vigilância | Decisão de manter, reduzir ou retirar o fluxo da colaboradora |

#### De quem coletar?

| Perfil/stakeholder | Critério de inclusão | Relação com persona/público |
|---|---|---|
| Colaboradores de equipes de tecnologia ou similares | 18 anos ou mais; trabalham em equipe com gestor direto e usam chat e ferramenta de tarefas no trabalho nos últimos seis meses | Público principal para investigar P03 e T03 |
| Colaboradores que já receberam comentário ou feedback sobre comunicação ou participação | Mesmo critério; experiência relatada voluntariamente, sem identificar pessoas envolvidas | Perspectiva mais próxima do C03 |
| **Exclusão** | Integrantes da equipe do projeto; pessoas subordinadas a quem conduz a entrevista; quem não consentir | Evitar viés e pressão hierárquica |

**Meta exploratória:** 3 a 5 entrevistas, por conveniência. Essa amostra não permite generalização; serve para revisar hipóteses e o fluxo.

#### Aspectos éticos

- **Voluntariedade e pressão hierárquica:** o convite é feito diretamente pela entrevistadora, nunca por gestores do participante. A recusa ou desistência não tem consequência e não precisa de justificativa.
- **Consentimento:** o termo (`instrumentos/termo_consentimento_modelo.md`, adaptado para entrevista) é lido antes de começar. O participante pode pular perguntas e retirar suas respostas até a consolidação.
- **Minimização:** não são coletados nome da empresa, nomes de colegas ou gestores, nem conteúdo de mensagens reais. Os exemplos são pedidos de forma genérica.
- **Dados sensíveis:** o roteiro não pergunta sobre saúde, vida familiar ou questões pessoais. Se o participante mencionar espontaneamente, a informação **não é anotada**. Esse risco é real neste projeto, porque o tema envolve mudanças de comportamento (C03.Q5).
- **Gravação:** somente áudio e somente com consentimento explícito e separado. Sem consentimento para gravar, são feitas apenas anotações. O áudio é apagado após a transcrição anonimizada.
- **Anonimização e armazenamento:** cada participante recebe um código (E01, E02…). As anotações ficam em pasta privada da autora durante o semestre 2026.2 e são descartadas ao final da disciplina. O termo assinado é guardado separado das anotações e **não** é publicado no GitHub.
- **Risco emocional:** falar sobre feedback pode gerar desconforto. A entrevistadora lembra que a pessoa pode pausar ou encerrar e não insiste em detalhes.
- **Relação com o TCC:** a entrevista não avalia o algoritmo nem a pessoa; o cenário apresentado é fictício.

## Parte B — ferramentas de coleta

> Cada integrante deve preparar uma técnica/instrumento completo. As técnicas devem ser diferentes entre si e **questionário deve estar entre as técnicas escolhidas**, conforme o enunciado da disciplina.

### Instrumento I01 — Questionário sobre acompanhamento de equipes

**Autor(a):** Caio Arnoni — 22.221.019-7 <br> 
**Técnica:** questionário on-line com perguntas fechadas e abertas.<br>
**Objetivo:** investigar a rotina de acompanhamento e as informações necessárias à interpretação e ao registro de um próximo passo, verificando as hipóteses relacionadas a T01.  <br>
**Público:** gestores com responsabilidade direta de acompanhamento nos últimos seis meses. <br>

#### Procedimento padronizado de aplicação

1. Transpor as perguntas abaixo para o formulário, preservando ordem, alternativas e desvios. Desativar coleta de e-mails e login obrigatório. Tornar obrigatórias somente Q01 e Q02, necessárias ao consentimento e à elegibilidade. Informar contato real e plataforma na apresentação antes de distribuir.
2. Fazer um piloto com uma pessoa elegível, verificando compreensão, tempo e funcionamento dos desvios. Se houver mudanças no instrumento, não misturar a resposta do piloto às da versão final. Registrar a versão aplicada e as alterações.
3. Convidar individualmente, sem pressão hierárquica, pessoas que atendam aos critérios. Enviar a mesma apresentação e informar que não se trata de avaliação profissional nem pesquisa diagnóstica.
4. Apresentar consentimento em Q01. Se a resposta for negativa, encerrar sem coletar conteúdo. Aplicar a elegibilidade em Q02; em caso negativo, agradecer e encerrar. Não usar essas submissões como dados da pesquisa.
5. Aplicar Q03–Q13 sobre práticas atuais antes de qualquer apresentação do WorkSense. Depois, mostrar o cenário fictício de Q14 e aplicar Q14–Q20. Não mostrar a avaliação da IA nem indicar respostas consideradas corretas.

#### Instrumento

Cole aqui o questionário/roteiro completo ou forneça link **mais uma cópia textual no repositório**.

```text
Questionário — Acompanhamento de equipes
Responsável: Caio Arnoni
Tempo estimado: 8 a 12 minutos
Escolha apenas uma alternativa nas perguntas fechadas.
Somente Q01 e Q02 são obrigatórias; as demais perguntas são opcionais.

Seção 1: Consentimento e perfil profissional

Q01. Você leu a apresentação e concorda em participar? Escolha única, obrigatória.
( ) Sim, concordo em participar.
( ) Não concordo. → Encerrar sem coletar respostas de conteúdo.

Q02. Você tem 18 anos ou mais e acompanha ou acompanhou diretamente colaboradores nos
últimos seis meses? Escolha única, obrigatória.
( ) Sim.
( ) Não. → Agradecer e encerrar por não atender ao recorte desta coleta.

Q03. Qual opção melhor descreve sua atuação nesse acompanhamento? Escolha única.
( ) Gestor ou gerente de equipe.
( ) Líder ou coordenador de equipe.
( ) Profissional de RH com acompanhamento direto de equipe.
( ) Outra função com responsabilidade direta de acompanhamento: ____________________ (opcional).
( ) Prefiro não responder.

Q04. Há quanto tempo você realiza atividades de acompanhamento de equipes, somando
suas experiências? Escolha única.
( ) Menos de um ano.
( ) De um a três anos.
( ) Mais de três anos.
( ) Prefiro não responder.

Seção 2: Rotina de acompanhamento e registro

Q05. Nos últimos seis meses, com que frequência você consultou informações para
decidir se deveria acompanhar mais de perto um colaborador? Escolha única.
( ) Diariamente ou quase diariamente.
( ) Semanalmente.
( ) Mensalmente.
( ) Menos de uma vez por mês.
( ) Somente quando ocorreu uma situação específica, sem frequência regular.
( ) Não realizei essa atividade nesse período.
( ) Não sei informar.

Q06. Pense na ocasião mais recente em que precisou decidir se faria algum
acompanhamento de um colaborador. O que motivou essa consulta e quais passos você
seguiu? Resposta aberta. Se não ocorreu, pode indicar isso. Não identifique pessoas
ou organizações.
Resposta: __________________________________________________________

Q07. Nessa ocasião, quais fontes ou ferramentas você consultou, se consultou alguma?
Resposta aberta. Pode informar categorias, como conversas, reuniões, documentos ou
ferramentas, e explicar para que serviram.
Resposta: __________________________________________________________

Q08. Quais informações pesaram na decisão e quais fizeram falta, se alguma? Resposta
aberta. Se não houve uma ocasião recente, pode responder sobre sua prática habitual
ou indicar que não se aplica.
Resposta: __________________________________________________________

Q09. Como você registrou a decisão e o acompanhamento combinado, se houve? Escolha
única.
( ) Não registrei.
( ) Anotei para uso pessoal.
( ) Registrei em documento ou planilha compartilhada.
( ) Registrei em ferramenta de gestão.
( ) Registrei por mensagem ou e-mail.
( ) Utilizei mais de uma dessas formas.
( ) Outra forma: ____________________ (opcional).
( ) Não se aplica / não lembro.

Q10. Que informações precisam constar nesse registro para que você ou outra pessoa
consiga retomar o caso? Se registrar não é necessário em sua rotina, explique por
quê. Resposta aberta.
Resposta: __________________________________________________________

Seção 3: Contexto de uso e familiaridade com indicadores

Q11. Qual dispositivo você mais utiliza para esse acompanhamento? Escolha única.
( ) Computador de mesa ou notebook.
( ) Celular.
( ) Tablet.
( ) Não utilizo dispositivo digital nessa atividade.
( ) Outro: ____________________ (opcional).
( ) Não se aplica.

Q12. Em quais momentos e condições você realiza essa atividade? Considere tempo
disponível, interrupções e possibilidade de outras pessoas visualizarem a consulta.
Há alguma barreira de leitura ou interação que dificulte a atividade? Resposta
aberta. Não informe diagnósticos ou dados de saúde.
Resposta: __________________________________________________________

Q13. Quando precisa interpretar indicadores sobre o trabalho da equipe, como descreve
essa atividade? Escolha única.
( ) Muito difícil.
( ) Difícil.
( ) Nem fácil nem difícil.
( ) Fácil.
( ) Muito fácil.
( ) Não utilizo indicadores / não se aplica.

Seção 4: Interpretação das informações

Cenário fictício para Q14–Q17: uma ferramenta apresenta uma mudança no padrão de
comunicação de um colaborador em relação ao próprio histórico. Os registros de
tarefas não mostram mudança no período. Em outro caso, faltam dados para concluir a
análise. Nenhum caso representa uma pessoa real. Responda com sua interpretação; não
é necessário conhecer o WorkSense.

Q14. Como você interpretaria o primeiro caso e qual seria seu próximo passo, se
algum? Resposta aberta.
Resposta: __________________________________________________________

Q15. No caso em que faltam dados, o que seria possível concluir e como você
procederia? Resposta aberta.
Resposta: __________________________________________________________

Q16. Quais informações adicionais você gostaria de conferir antes de tomar uma
decisão nesses casos, se alguma? Resposta aberta.
Resposta: __________________________________________________________

Q17. O que as expressões “padrão individual”, “sinalização” e “análise incompleta”
significam para você nesse contexto? Alguma deveria ser substituída? Resposta aberta;
permitir indicar que não conhece o termo.
Resposta: __________________________________________________________

Seção 5: Acesso e condições de uso

Q18. Quem deveria poder consultar e registrar informações desse tipo, e quais limites
de acesso ou uso seriam importantes? Resposta aberta.
Resposta: __________________________________________________________

Q19. Uma consulta desse tipo teria lugar na sua rotina? Escolha única.
( ) Sim.
( ) Talvez, dependendo das condições.
( ) Não.
( ) Não sei avaliar.

Q20. Explique sua resposta anterior. O que precisaria mudar no seu processo atual, se
algo, e o que faria você evitar uma ferramenta desse tipo? Resposta aberta.
Resposta: __________________________________________________________

```
**Mensagem final:** “Obrigado pela participação. Suas respostas contribuirão para revisar o cenário de uso e os requisitos do projeto acadêmico. Nenhuma conclusão será usada para avaliar pessoas ou equipes.”

#### Como os dados serão analisados

As respostas fechadas serão resumidas por contagem de alternativas, sempre informando o número de respostas válidas por pergunta e as omissões. A amostra pequena e por conveniência não permite generalização estatística. Perfis de RH serão identificados separadamente na análise; não publicar cruzamentos que favoreçam reidentificação.

As respostas abertas serão organizadas por temas: processo atual; informações utilizadas; registro e retomada; contexto e acessibilidade; compreensão de resultados; confiança e limites de uso. Registrar também necessidades inesperadas e respostas que contrariem o cenário proposto. Associar cada interpretação a uma resposta desidentificada, distinguindo fala do participante de inferência do pesquisador.

Q03–Q10 investigarão H05, H15, H18 e H19; Q11–Q13 investigarão H10, H20, H21, H22 e H27; Q14–Q17 investigarão H17, H19, H24, H25 e ?03; Q18–Q20 investigarão H05 e H23 e as condições de utilidade da proposta. O questionário pode revelar dificuldades relatadas, mas não comprova desempenho na interface, causalidade de sobrecarga por métricas ou precisão técnica do TCC.

Para cada hipótese, reunir evidências favoráveis e contrárias antes de decidir: sustentada no recorte quando houver relatos concretos convergentes; refutada no recorte quando os relatos contradisserem a formulação; refinada quando depender de contexto ou perfil. Respostas insuficientes ou genéricas mantêm a hipótese aberta. Registrar quantidade de respostas, limitações e fundamento da decisão; não converter aprovação da ideia em comprovação de necessidade de dashboard.

Os resultados poderão alterar persona, contexto, etapas de T01, informações mostradas e vocabulário. Por exemplo, ausência de necessidade de registro exige rever essa etapa; dificuldade em distinguir insuficiência de estabilidade exige revisar explicações e testar sua compreensão posteriormente. Essas são possibilidades de revisão, não resultados já obtidos.

### Instrumento I03 — Entrevista semiestruturada com colaboradores

**Autor(a):** Tainá Cunha Bueno — 22.119.025-9 <br>
**Técnica:** entrevista semiestruturada individual, presencial ou por videochamada, de 25 a 35 minutos. <br>
**Objetivo:** compreender como colaboradores recebem e respondem a interpretações sobre sua comunicação, o que precisam saber sobre análises que os envolvem e o que caracteriza um retorno satisfatório, verificando as hipóteses ligadas a P03, C03 e T03. <br>
**Público:** colaboradores com gestor direto que usaram chat e ferramenta de tarefas no trabalho nos últimos seis meses. <br>

#### Procedimento padronizado de aplicação

1. **Piloto:** aplicar o roteiro com uma pessoa elegível, verificando duração, clareza e o cartão do cenário. Se o roteiro mudar, registrar a versão e não misturar o piloto aos resultados.
2. **Convite:** individual, pela entrevistadora, com a mesma mensagem para todos. Informar duração, finalidade acadêmica e que não se trata de avaliação profissional.
3. **Abertura:** ler a apresentação e o termo; obter o consentimento para participar e, separadamente, para gravar áudio.
4. **Ordem fixa dos blocos:** primeiro a experiência atual (blocos 1 e 2) e só depois o cenário fictício e a ideia de interface (blocos 3 e 4), para não induzir respostas.
5. **Condução:** fazer as perguntas principais na ordem; usar as perguntas de aprofundamento apenas quando necessário. Não sugerir respostas, não defender a ideia do WorkSense e não pedir exemplos reais com nomes.
6. **Registro:** anotar falas-chave entre aspas (curtas), sem dados identificáveis; marcar o tempo aproximado de cada bloco.
7. **Encerramento:** perguntar se a pessoa quer acrescentar ou retirar algo; agradecer; registrar o código do participante.

#### Instrumento

```text
Roteiro de entrevista — Esclarecimento de interpretações no trabalho
Responsável: Tainá Cunha Bueno
Duração estimada: 25 a 35 minutos
Código do participante: E__        Data: __/__/____     Gravação de áudio autorizada? ( ) Sim ( ) Não

ABERTURA (ler)
"Obrigada por participar. Esta entrevista faz parte de um trabalho da disciplina
de Interação Humano-Computador. Quero entender como as pessoas recebem e respondem
a comentários sobre a forma como se comunicam no trabalho. Não existe resposta
certa ou errada e não estou avaliando você. Não cite nomes de colegas, gestores
ou empresas. Você pode pular qualquer pergunta, pedir pausa ou encerrar quando
quiser. Não vou perguntar sobre saúde ou vida pessoal; se algo assim surgir,
não será anotado."
→ Ler o termo de consentimento e confirmar o aceite antes de continuar.

BLOCO 0 — Perfil (sem identificação)
0.1 Qual é a sua função e há quanto tempo você trabalha nessa equipe?
0.2 Você trabalha de forma presencial, remota ou híbrida?
0.3 Quais ferramentas a equipe usa para conversar e para organizar tarefas?

BLOCO 1 — Feedback sobre comunicação hoje
1.1 Você já recebeu algum comentário sobre a forma como se comunica ou participa
    nas conversas da equipe? Como foi, sem citar nomes?
    ↳ Aprofundar: Em que momento isso aconteceu? Por qual canal?
1.2 Você soube em que a pessoa se baseou para fazer o comentário?
    ↳ Aprofundar: O que teria ajudado você a entender?
1.3 Como você respondeu ou explicou o seu lado?
    ↳ Aprofundar: Você preparou algo antes? Reuniu exemplos? Quanto tempo levou?
1.4 Existem informações que você preferiria não compartilhar ao explicar uma
    situação de trabalho? Sem mencionar informações pessoais, como você lida
    com esses limites?

BLOCO 2 — Retorno e conclusão
2.1 Depois que você explicou o seu lado, o que aconteceu?
2.2 Como você soube se a sua explicação foi considerada?
    ↳ Aprofundar: Quanto tempo de espera é aceitável? O que o silêncio significa para você?
2.3 O que precisaria acontecer para você considerar o assunto encerrado?

BLOCO 3 — Cenário fictício (mostrar o cartão abaixo e ler em voz alta)
   CARTÃO: "Uma ferramenta compara as mensagens de trabalho e as tarefas de cada
   pessoa com o seu próprio histórico. Neste ciclo, ela indicou que as mensagens de
   uma colaboradora ficaram mais frequentes e mais curtas. As tarefas continuaram
   como antes. O gestor recebeu essa informação."
3.1 Se você fosse essa colaboradora, o que gostaria de saber sobre essa análise?
    ↳ Aprofundar: o que é analisado? Por quem? Para quê? Por quanto tempo?
3.2 Como você entende a frase "as mensagens mudaram em relação ao seu histórico"?
    ↳ Aprofundar: Isso parece uma avaliação sobre você? Por quê?
3.3 Você gostaria de ver a mesma explicação que o gestor viu? Por quê?
3.4 Se quisesse dar o seu contexto, como preferiria fazer: por escrito, em conversa,
    com outra pessoa presente, ou de outro modo?

BLOCO 4 — Limites e aceitação
4.1 O que tornaria uma ferramenta como essa aceitável ou inaceitável para você?
4.2 Quem não deveria ter acesso a essas informações?
4.3 Se você enviasse uma explicação por uma ferramenta, o que esperaria ver depois
    de enviar?

ENCERRAMENTO
5.1 Há algo que não perguntei e que você considera importante?
5.2 Você quer retirar ou corrigir algo do que disse?
"Obrigada! As respostas serão usadas de forma anônima, apenas para a disciplina."

ANOTAÇÕES DA ENTREVISTADORA
Duração por bloco: B0 __ B1 __ B2 __ B3 __ B4 __
Falas-chave (curtas, sem identificação):
Observações sobre compreensão do cartão:
Perguntas puladas:
```

#### Como os dados serão analisados

As anotações e transcrições anonimizadas serão organizadas por **análise temática** com um **diagrama de afinidade**. Cada fala-chave vira uma nota, e as notas serão agrupadas nos temas: (1) como o feedback chega; (2) assimetria de informação; (3) esforço de reconstrução; (4) privacidade e o que não se compartilha; (5) expectativa de retorno e critério de conclusão; (6) transparência desejada; (7) aceitação e percepção de vigilância. Temas não previstos serão registrados em um grupo próprio, e não forçados nos existentes.

Relação entre blocos e hipóteses: o **bloco 1** investiga H06, H23 e C03.Q1–Q5; o **bloco 2**, C03.Q7–Q8 e N06; o **bloco 3**, H11, H25, ?03 e N07; o **bloco 4**, H23 e H28.

Para cada hipótese, as evidências favoráveis e contrárias serão listadas antes da decisão: **sustentada no recorte** quando houver relatos concretos convergentes; **refutada no recorte** quando os relatos a contradisserem; **refinada** quando depender de contexto; **inconclusiva** quando faltarem dados. A quantidade de participantes que mencionaram cada tema será informada, sem percentuais, por causa da amostra pequena.

Os resultados podem alterar P03, C03, T03 e o fluxo PF07. Por exemplo: se os participantes não quiserem acessar a própria explicação, o fluxo passa a se limitar à transparência (P12/F14) e ao pedido de conversa; se o silêncio após o envio for a maior dor, a confirmação e os estados da solicitação ganham prioridade; se “comunicação mudou” for lido como avaliação, os rótulos precisam ser revistos antes do Figma. Essas são possibilidades de revisão, não resultados obtidos.

## Síntese

O questionário pretende reduzir lacunas sobre a existência da tarefa de Rafael, as fontes utilizadas, as decisões realizadas e os critérios para registrar um acompanhamento. Também investiga compreensão dos termos, condições de consulta e limites de acesso. Após a coleta, H05, H10, H15, H17, H18, H19, H20, H21, H22, H23, H24, H25, H27 e ?03 serão reavaliadas como sustentadas, refutadas, refinadas ou ainda abertas, conforme as evidências e o alcance de cada pergunta.

## Checklist

- [ ] Hipóteses/lacunas prioritárias da Entrega 1 foram revisitadas.
- [ ] Se o escopo de IHC foi derivado de TCC técnico, a coleta investiga a plausibilidade do usuário, tarefa e contexto adotados.
- [ ] Perguntas não pressupõem que dashboard, CRUD, filtros ou relatórios sejam necessários; investigam a necessidade.
- [ ] Cada dado a coletar responde uma dúvida concreta do projeto ou justifica outra necessidade de informação.
- [ ] Parte A identifica dados e perfis de coleta de forma específica.
- [ ] Aspectos éticos são contextualizados para o projeto.
- [ ] Há uma técnica completa por integrante e técnicas distintas.
- [ ] Questionário está incluído entre as técnicas.
- [ ] Cada instrumento possui objetivo, público, procedimento e conteúdo integral.
- [ ] Perguntas evitam indução e coletam apenas dados necessários.
- [ ] Está claro como os dados serão analisados e usados no design.
