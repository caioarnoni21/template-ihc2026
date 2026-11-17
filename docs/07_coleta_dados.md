# Entrega 7 — Coleta de dados, necessidades e aspectos éticos

**Data:** {{dd/mm/aaaa}}  
**Status:** ⬜ Em andamento

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

> Repita A02, A03...

## Parte B — ferramentas de coleta

> Cada integrante deve preparar uma técnica/instrumento completo. As técnicas devem ser diferentes entre si e **questionário deve estar entre as técnicas escolhidas**, conforme o enunciado da disciplina.

### Instrumento I01 — Questionário sobre acompanhamento de equipes

**Autor(a):** Caio Arnoni — 22.221.019-7 <br> 
**Técnica:** questionário on-line com perguntas fechadas e abertas.
**Objetivo:** investigar a rotina de acompanhamento e as informações necessárias à interpretação e ao registro de um próximo passo, verificando as hipóteses relacionadas a T01.  
**Público:** gestores com responsabilidade direta de acompanhamento nos últimos seis meses. 

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
