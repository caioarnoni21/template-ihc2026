# Entrega 9 — Modelo conceitual e design centrado na comunicação

**Data:** 18/11/2026  
**Status:** 🟨 Em andamento  
**Responsabilidade:** soluções individuais, com consolidação da equipe para mapa de objetivos e esquema de signos.

## Objetivo da atividade

Passar do cenário de problema para uma concepção da interação, explicitando objetivos, tópicos de conversa, falas e signos que a interface deverá comunicar/manipular.

## Transformando resultados técnicos em conceitos compreensíveis

Em TCCs algorítmicos ou orientados a dados, esta entrega deve evitar que a interface exponha apenas estruturas internas do código. Identifique os **conceitos e signos que fazem sentido para o usuário**.

Exemplos:

- `query plan`, custo estimado, recomendação e impacto para um DBA;
- modelo, dataset, versão, execução e métrica para engenheiro de IA;
- período, indicador, grupo, tendência e filtro para gestor/analista;
- alerta, severidade, evidência, responsável e status para analista de segurança.

Se um termo técnico for necessário, modele como será comunicado, explicado e relacionado à tarefa.

Dashboards, relatórios, filtros e CRUDs devem aparecer no modelo conceitual por meio dos **objetivos, signos e conversas** que justificam sua existência.

## 1. Cenários de interação

Para cada cenário de problema, produza uma versão em que a solução já pode ser descrita. **Destaque claramente o texto alterado** em relação ao cenário original.

### CI01 — Consultar uma análise e preparar o próximo passo de acompanhamento

**Autor(a):**  Caio Arnoni — 22.221.019-7
**Origem:** cenário problema C01, seção “Cenário refinado” da Entrega 4; também referenciado como E4-C01 nas entregas anteriores.

Durante uma semana de trabalho híbrido, Rafael Costa percebe que as mensagens de Maria Fonseca estão mais curtas e objetivas. Ele precisa entender se há alguma dificuldade de trabalho que justifique uma conversa de apoio. A conversa individual com Maria acontecerá naquela tarde, e Rafael quer se preparar sem levar uma avaliação previamente fechada. Está em casa, usando o notebook, e dispõe de vinte minutos antes de outra reunião.

**Em vez de reunir manualmente referências em diferentes ferramentas, Rafael solicita ao WorkSense a análise de Maria e informa qual período disponível deseja consultar. O sistema apresenta a identidade do caso, o período analisado, o histórico usado como referência, as fontes, a cobertura e a última atualização. Rafael confere se está consultando a pessoa e o ciclo pretendidos antes de interpretar os resultados.**

**Para o caso fictício desta narrativa, a análise tem dados suficientes e apresenta uma mudança na comunicação, enquanto os indicadores de tarefas permanecem próximos do histórico individual. O sistema mantém essas duas dimensões separadas e informa quais evidências sustentam a comparação e quais conclusões não são possíveis. Rafael reconhece que o andamento das entregas não explica, sozinho, o modo de escrever de Maria.**

Ele conhece os prazos, mas depende de Maria e do responsável pelo produto para compreender mudanças recentes na complexidade das demandas; os acordos de comunicação também dependem de contexto externo aos registros.

**Rafael pede esclarecimentos sobre o significado da sinalização. O sistema explica que ela representa uma alteração observada nos dados, não um diagnóstico ou uma explicação de sua causa. Uma mensagem técnica detalhada enviada por Maria contraria a impressão de respostas sempre curtas. Rafael considera esse exemplo na própria interpretação, sem presumir que ele já foi incorporado à análise: confere a atualização e reconhece a diferença entre o resultado disponível e o contexto posterior.**

Uma solicitação de alinhamento interrompe a consulta. **Ao retornar à atividade na mesma sessão, Rafael encontra preservados o caso e o período consultados e consegue retomar a análise sem reconstruir toda a sequência.**

**Rafael decide preparar uma conversa de apoio, sem concluir que Maria tenha um problema de saúde ou de desempenho. Informa esse encaminhamento, uma justificativa limitada ao contexto de trabalho, o responsável e uma data de retomada. O sistema apresenta o conteúdo a ser registrado, vinculado à colaboradora e ao período. Rafael confere e confirma o registro.**

**Após concluir o registro, o sistema confirma o resultado e devolve o caso, o período e o encaminhamento registrado para conferência. Rafael encerra a preparação sabendo o que pretende conversar e como retomar o acompanhamento. A conversa com Maria e seus resultados permanecem fora de T01 e ainda não ocorreram nesta narrativa.**

**Se a análise não tiver dados suficientes, o sistema informa a fonte ou período com cobertura insuficiente e não apresenta uma conclusão sobre mudança. Rafael pode registrar a insuficiência, indicar quem retomará a consulta e quando, mantendo qualquer conversa humana independente de uma conclusão não sustentada pelos dados.**

**Se o registro não puder ser concluído, o sistema informa que ele não foi salvo e preserva o conteúdo durante a tentativa de recuperação. Rafael pode corrigir um dado inválido ou tentar novamente, conforme a causa informada. A atividade só é considerada concluída após a confirmação; persistindo a falha, permanece pendente.**


### Diferenças relevantes

| Alteração | Por que foi necessária | Evidência/artefato que justifica |
|---|---|---|
| Consulta identificada por colaborador, período, referência, cobertura e atualização | Reduzir ambiguidade e permitir verificar se os dados são pertinentes antes de interpretar | C01.Q4–Q5; HTA T01, etapas 1 e 2.1 |
| Comunicação e tarefas interpretadas separadamente | Evitar que cumprimento de prazos seja tratado como explicação da comunicação | C01.Q6; necessidade N01; HTA T01, etapa 2.2 |
| Explicação do significado e dos limites da sinalização | Distinguir resultado técnico, contexto externo e decisão humana | C01.Q3 e Q7; necessidades N02 e N03; metas qualitativas da Entrega 8 |
| Retomada do caso e período durante a sessão | Reduzir retrabalho após interrupção | C01.Q2; contexto proposto na Entrega 3 |
| Registro justificado e confirmação vinculados ao caso | Preservar o próximo passo sem confundir planejamento com conversa já realizada | C01.Q8; HTA T01, etapas 3.1 e 3.2; necessidade N06 |
| Caminhos de insuficiência e falha explícitos | Evitar conclusão sem evidências ou impressão de salvamento não ocorrido | HTA T01, planos condicionais e repetição; Entregas 6 e 8 |

## 2. Design centrado na comunicação

**Nome do cenário:** CI01 — Consultar uma análise e preparar o próximo passo de acompanhamento.

| Tópico > subtópico | Falas e signos envolvidos | Intenção/efeito esperado |
|---|---|---|
| Consultar uma análise e registrar o próximo passo humano | `U: Quero compreender este caso e preparar um acompanhamento.` / `D: Posso apresentar as evidências disponíveis e registrar sua decisão, sem determinar a causa da mudança.` Signos: análise, colaborador, encaminhamento | Comunicar a finalidade e o limite do apoio oferecido |
| > Localizar a análise | `U: Quero consultar Maria neste período.` / `D: Este é o caso, o período analisado e o padrão individual de referência.` Signos: colaborador, período analisado, período de referência | Estabelecer o contexto correto antes da interpretação |
| > Conferir suficiência e atualização | `U: Os dados permitem essa comparação?` / `D: Estas são as fontes, a cobertura, a atualização e as limitações.` Signos: fontes, cobertura, última atualização, estado da análise | Permitir avaliar a validade da consulta |
| > Interpretar evidências | `U: O que mudou em relação ao histórico da própria pessoa?` / `D: A comunicação apresentou mudança; os indicadores de tarefas permaneceram próximos do histórico neste exemplo.` Signos: padrão individual de referência, evidências de comunicação, evidências de tarefas | Evitar que um eixo substitua o outro |
| > Compreender o significado | `U: Essa mudança explica o que está acontecendo com Maria?` / `D: Não. A sinalização não determina causa; é necessário considerar o contexto e ouvir a colaboradora.` Signos: sinalização, limites da análise | Evitar interpretações diagnósticas ou punitivas |
| > Retomar a consulta | `U: Quero continuar de onde parei.` / `D: Você estava consultando este caso e este período nesta sessão.` Signos: colaborador, período analisado | Recuperar o contexto sem perder a identidade do caso |
| > Definir próximo passo | `U: Pretendo conversar para compreender o contexto de trabalho.` / `D: Qual encaminhamento deseja registrar, por qual motivo e com quem ficará a retomada?` Signos: encaminhamento, justificativa, responsável, data de retomada | Separar decisão humana de resultado técnico |
| > Registrar insuficiência | `U: Não há dados suficientes para concluir; quero registrar essa limitação.` / `D: Posso registrar a pendência e quem retomará a consulta, sem atribuir uma conclusão à pessoa.` Signos: estado da análise, limites da análise, encaminhamento, responsável | Tornar a insuficiência um resultado válido da tarefa |
| > Conferir e concluir o registro | `U: Os dados conferem; confirmo o registro.` / `D: O registro foi concluído para este colaborador e período, com este encaminhamento.` Signos: estado do registro e conteúdo do encaminhamento | Tornar a consequência da confirmação verificável |
| > Recuperar falha de registro | `D: Não foi possível salvar; o registro continua pendente e seu conteúdo foi preservado nesta tentativa.` / `U: Quero corrigir o problema ou tentar novamente.` Signos: estado do registro, motivo da falha, campos do encaminhamento | Evitar perda de conteúdo e falsa confirmação de sucesso |

**Convenção:** `U` = usuário; `D` = preposto do designer/sistema, conforme a abordagem de Engenharia Semiótica adotada na disciplina.

## 3. Mapa de objetivos

Cada integrante apresenta seu mapa e a equipe cria um **mapa consolidado**, eliminando duplicidades e resolvendo conflitos de nomenclatura.

<img width="1818" height="571" alt="image" src="https://github.com/user-attachments/assets/83430598-09f6-41be-b215-41d1210be401" />


### Dicionário de objetivos

| ID | Objetivo | Persona(s) | Cenário(s) | Prioridade |
|---|---|---|---|---|
| O01 | Consultar uma análise e registrar o próximo passo humano | P01 — Rafael Costa | CI01 / T01 | Alta |
| O02 | Localizar a análise pertinente | P01 — Rafael Costa | CI01 | Alta |
| O03 | Avaliar as evidências e seus limites | P01 — Rafael Costa | CI01 | Alta |
| O04 | Definir o próximo passo humano | P01 — Rafael Costa | CI01 | Alta |
| O05 | Registrar e conferir o encaminhamento | P01 — Rafael Costa | CI01 | Alta |
| O06 | Conferir identidade, períodos, cobertura e atualização | P01 — Rafael Costa | CI01 | Alta |
| O07 | Interpretar comunicação e tarefas separadamente | P01 — Rafael Costa | CI01 | Alta |
| O08 | Reconhecer insuficiência de dados | P01 — Rafael Costa | CI01, alternativa de insuficiência | Alta |
| O09 | Retomar a consulta após interrupção | P01 — Rafael Costa | CI01 | Média |
| O10 | Recuperar uma falha de registro | P01 — Rafael Costa | CI01, alternativa de falha | Alta |

## 4. Esquema conceitual de signos

Consolide as informações em **uma tabela única**.

| Grupo | Signo | Origem | Observações/semântica | Tipo de conteúdo | Restrição | Valor padrão | Prevenção | Recuperação |
|---|---|---|---|---|---|---|---|---|
| Contexto | Colaborador | Domínio | Pessoa acompanhada; usuário seleciona entre identidades disponibilizadas pelo sistema | Identificador e nome de exibição | Deve pertencer ao conjunto autorizado; manter vínculo inequívoco mesmo com iniciais | Nenhum caso selecionado | PP: apresentar identidade junto ao período; PA: impedir acesso não autorizado | RA: permitir corrigir a seleção; CE: orientar contato com responsável quando faltar autorização legítima |
| Contexto | Período analisado | Domínio | Intervalo de registros sobre o qual o sistema apresenta a análise, escolhido entre os disponíveis | Intervalo de datas | Início não posterior ao fim; vinculado ao caso e à análise disponível | Nenhum até selecionar a análise | PP: explicitar datas; PA: não aceitar intervalo inexistente como análise pronta | RA: indicar períodos disponíveis e permitir nova escolha |
| Contexto | Período de referência | Aplicação | Intervalo histórico usado pelo sistema para estabelecer o padrão individual | Intervalo de datas | Corresponder à comparação efetivamente realizada; não confundir com período analisado | O da análise selecionada | PP: distinguir referência de período analisado | RA: informar ausência de referência válida e impedir conclusão indevida |
| Evidências | Padrão individual de referência | Aplicação | Síntese calculada do histórico do próprio colaborador; não representa padrão ideal nem média da equipe | Conjunto de medidas com unidades e explicação | Depende de histórico suficiente; não comparar pessoas como equivalentes | Não disponível até haver referência válida | PP: explicar comparação consigo mesmo | RA: informar insuficiência e permitir registrar pendência |
| Evidências | Fontes | Domínio | Origem dos registros profissionais ou comunicacionais apresentada pelo sistema | Conjunto de nomes de fontes | Indicar apenas fontes realmente consideradas na análise | Fontes da análise selecionada | PP: explicar o que cada fonte representa | CE: se uma integração exigir reparo externo, indicar responsável técnico sem atribuir a falha ao colaborador |
| Evidências | Cobertura | Aplicação | Disponibilidade dos dados por fonte e período, produzida pelo sistema | Estado por fonte e intervalo; contagem quando conhecida | Não apresentar percentual sem denominador; desconhecido não equivale a completo | Não verificada | PP: informar lacunas e alcance da comparação | RA: permitir registrar insuficiência; CE: indicar reparo externo quando necessário |
| Evidências | Última atualização | Aplicação | Momento da atualização dos dados considerados na análise | Data e hora com referência de fuso | Não apresentar horário de consulta como se fosse atualização dos dados | Não disponível até conhecer a atualização | PP: identificar a que atualização o horário se refere | RA: sinalizar indisponibilidade ou desatualização sem inventar horário |
| Evidências | Estado da análise | Aplicação | Situação da produção ou disponibilidade da análise, não avaliação da pessoa | Categoria: em processamento, disponível, incompleta ou indisponível | Usar conforme a cobertura e o processamento; não equivale a sinalização | Indisponível até confirmação | PP: explicar cada estado; PA: não emitir conclusão para dados insuficientes | RA: aguardar ou registrar pendência; CE: orientar suporte em falha não recuperável pelo gestor |
| Evidências | Evidências de comunicação | Aplicação | Indicadores derivados de registros comunicacionais, apresentados pelo sistema em relação à referência | Medidas e comparação explicadas | Exibir unidades e período; sem inferir diagnóstico ou causa; limitar dados identificáveis | Não disponíveis sem dados suficientes | PP: explicar limites e manter separado das tarefas | RA: indicar insuficiência ou informação divergente a conferir |
| Evidências | Evidências de tarefas | Aplicação | Indicadores derivados dos registros de trabalho, separados dos comunicacionais | Medidas e comparação explicadas | Não equivalem a desempenho global; dependem de cobertura suficiente | Não disponíveis sem dados suficientes | PP: explicitar alcance das medidas | RA: indicar limitações e permitir manter pendência |
| Interpretação | Sinalização | Aplicação | Resultado derivado de alteração em uma dimensão; não decisão sobre a pessoa | Classificação por dimensão e explicação | Só concluir com dados suficientes; ausência de sinalização não significa ausência de dificuldade humana | Sem conclusão até verificar suficiência | PP: distinguir alteração, causa e decisão | RA: consultar evidências e limites antes de registrar |
| Interpretação | Limites da análise | Aplicação | Explicação do que os resultados permitem ou não concluir, produzida pelo sistema | Texto contextual | Vinculado ao caso e às limitações reais; não esconder ausência de dados | Explicação geral, acrescida das limitações do caso | PP: tornar explícitas as restrições de interpretação | RA: oferecer explicação complementar; sem prometer esclarecer a causa humana |
| Encaminhamento | Encaminhamento | Domínio | Próximo passo escolhido por Rafael, independente de automatismos do modelo | Categoria: conversar, acompanhar, não intervir neste ciclo ou aguardar dados | Seleção explícita; insuficiência não fundamenta uma conclusão sobre a pessoa | Nenhum | PP: explicar opções; PA: exigir escolha; AL: pedir revisão se houver insuficiência e conclusão incompatível | RA: permitir revisar antes de confirmar |
| Encaminhamento | Justificativa | Domínio | Motivo informado por Rafael; distinguir evidência, hipótese e informação a confirmar | Texto | Obrigatória para registrar; sem diagnósticos ou conteúdo pessoal desnecessário | Vazia | PP: orientar conteúdo mínimo; PA: impedir confirmação vazia | RA: identificar ausência e preservar os demais dados |
| Encaminhamento | Responsável pela retomada | Domínio | Pessoa autorizada indicada para dar continuidade | Referência a pessoa autorizada | Obrigatória para registro; não escolher terceiro sem responsabilidade definida | Nenhum | PP: explicar responsabilidade; PA: exigir indicação válida | RA: corrigir responsável sem perder justificativa |
| Encaminhamento | Data de retomada | Domínio | Data proposta pelo usuário para reavaliar o encaminhamento | Data | Obrigatória para acompanhar ou aguardar dados; não anterior à data do registro | Não definida | PP: explicar formato e quando é necessária; PA: validar condição e data | RA: indicar o problema e permitir corrigir |
| Registro | Estado do registro | Aplicação | Situação do encaminhamento durante a interação | Categoria: rascunho, salvando, salvo ou falha | Informar salvo somente após conclusão confirmada; simulação declarada no protótipo | Rascunho | PP: distinguir rascunho de salvo; AL: avisar antes de descartar conteúdo | RA: preservar conteúdo e tentar novamente; manter pendência se não salvar |
| Registro | Motivo da falha | Aplicação | Explicação produzida pelo sistema sobre o impedimento e a ação possível | Texto contextual | Não expor detalhes técnicos ou credenciais; não afirmar causa desconhecida | Não se aplica sem falha | PP: explicar restrições conhecidas antes da confirmação | RA: orientar correção ou nova tentativa; CE: indicar suporte se a recuperação estiver fora da interface |

### Regras para os signos

- Use o vocabulário do domínio do usuário.
- Evite duplicar o mesmo conceito com nomes diferentes.
- Diferencie informação fornecida pelo usuário, produzida pelo sistema e derivada do domínio.
- Registre prevenção e recuperação apenas quando fizer sentido; explique as siglas usadas.

## Síntese

Quais objetivos/tópicos/signos deverão necessariamente aparecer nos diagramas MoLIC?

Na Entrega 10, os diagramas MoLIC de T01 deverão representar as conversas para localizar a análise (O02), conferir suficiência e contexto (O06), interpretar as dimensões e seus limites (O03/O07/O08), definir o próximo passo (O04) e registrar e conferir o resultado (O05). Também deverão explicitar retomada (O09) e recuperação de falha (O10), sem transformar insuficiência em conclusão sobre a pessoa.

Os signos obrigatórios são colaborador, períodos analisado e de referência, padrão individual de referência, fontes, cobertura, última atualização, estado da análise, evidências de comunicação e de tarefas, sinalização, limites da análise, encaminhamento, justificativa, responsável, data de retomada quando aplicável, estado do registro e motivo da falha quando houver.

## Checklist

- [ ] Cenários de interação mostram alterações em relação aos cenários de problema.
- [ ] Cada solução individual identifica autor e cenário de origem.
- [ ] Tópicos/falas/signos são coerentes com objetivos do usuário.
- [ ] Mapas individuais foram consolidados.
- [ ] O esquema de signos está em uma tabela única e sem duplicações conceituais.
- [ ] Nomes de objetivos/signos serão reutilizados na Entrega 10.
- [ ] Em TCC técnico, signos representam conceitos do domínio compreensíveis ao usuário, não apenas variáveis/estruturas internas.
- [ ] Padrões como dashboard, relatório, filtros, administração e CRUD possuem objetivos e signos correspondentes.
- [ ] A interface comunica não só o resultado técnico, mas também seu significado para a tarefa.
