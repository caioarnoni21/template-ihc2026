# Entrega 12 — Planejamento da avaliação de usabilidade (DECIDE)

**Data:** {{25/11/2026}}  
**Status:** 🟩 Concluida 
**Responsabilidade:** 1 solução por equipe

## Objetivo da atividade

Planejar a avaliação antes de executá-la, ligando perguntas de avaliação a métodos, participantes, tarefas, métricas, aspectos práticos, ética e forma de análise.

## O que está sendo avaliado

Em projetos cuja interface foi criada ou ampliada para a disciplina, o plano deve declarar explicitamente que a avaliação investiga **a qualidade da interação/protótipo**, não a validade científica ou o desempenho técnico do algoritmo/modelo do TCC.

Exemplos de perguntas:

- o DBA consegue localizar e comparar duas execuções?
- o analista entende o significado de um indicador?
- o administrador consegue alterar uma permissão sem risco de erro não percebido?
- o usuário compreende que o processamento está em andamento e consegue recuperar-se de uma falha?
- os filtros ajudam a localizar o histórico relevante?
- um relatório permite identificar a informação necessária para a decisão?

Se o protótipo utiliza dados ou resultados simulados, documente isso no plano.

## A. Método DECIDE

A avaliação do fluxo da colaboradora (T03) investiga a qualidade da interação com as telas F14–F18, considerando a compreensão das informações apresentadas, o envio de contexto ao gestor e o acompanhamento da solicitação.

Os indicadores, mensagens, períodos, respostas do gestor e estados das solicitações apresentados no protótipo são fictícios. A avaliação não pretende validar os algoritmos do WorkSense, a precisão dos indicadores ou a capacidade de identificar alterações comportamentais e profissionais.

| Etapa | Aplicação no projeto |
|---|---|
| D — Determine the goals | Verificar conclusão autônoma de T01 (MU01), tempo (MU02), satisfação (MU03), compreensão da insuficiência (MU04), recuperação de falha (MU05) e acesso por teclado quando tecnicamente avaliável (MU06). Para T03, verificar o envio de contexto ao destinatário correto e a conferência do recebimento sem ajuda (MU07), além da compreensão das dimensões e dos limites da análise (MU08). Priorizar interpretação responsável e registro correto sobre rapidez. |
| E — Explore the questions | Investigar se gestores localizam a pessoa e o período corretos, distinguem comunicação de tarefas, reconhecem limitações, registram um encaminhamento coerente e conferem o resultado. Investigar se colaboradores compreendem a própria explicação, identificam o destinatário, apresentam seu contexto e reconhecem o estado da solicitação. Examinar feedback, consistência, controle, prevenção e recuperação de erros. |
| C — Choose the evaluation paradigm and techniques | Avaliação formativa: inspeção heurística independente por avaliadores para a Entrega 13, seguida de teste observado com gestores e colaboradores para a Entrega 14, conforme o perfil de cada tarefa. Usar perguntas pós-tarefa para esclarecer interpretação e satisfação; opinião isolada não substitui observação. |
| I — Identify the practical issues | Planejar três avaliadores, uma pessoa elegível para o piloto e participantes externos ao grupo para o teste principal, conforme a disponibilidade e a orientação docente. Prever cinco gestores para a avaliação do fluxo T01 e pelo menos um colaborador para T03, registrando eventuais limitações de recrutamento. Usar notebook, navegador, Figma e cronômetro em ambiente tranquilo. Caio prepara e conduz a avaliação de T01; Tainá prepara e conduz a avaliação de T03. Inspecionar, corrigir bloqueios, realizar piloto, congelar a versão e então testar. |
| D — Decide how to deal with ethical issues | Explicar propósito acadêmico, voluntariedade, riscos e direito de interromper. Usar apenas casos fictícios, sem solicitar dados de colegas, empresas ou informações pessoais sensíveis. Registrar notas por códigos, sem gravação por padrão; guardar consentimento separado. Evitar relações de subordinação entre participantes e avaliadores. Não publicar dados brutos nem avaliar desempenho profissional dos participantes. |
| E — Evaluate, interpret and present the data | Consolidar contagens, tempos, satisfação e evidências qualitativas por tarefa e perfil. Comparar os resultados às metas originais, incluindo MU07 e MU08 para T03, e registrar omissões, ajuda e limitações. Priorizar problemas pela consequência, frequência observada e possibilidade de recuperação, mantendo inspeção heurística e teste humano separados. Não generalizar resultados obtidos com amostras pequenas. |

## B. Perguntas de avaliação

| ID | Pergunta | Método | Métrica/evidência | Critério esperado |
|---|---|---|---|---|
| QA01 | O gestor conclui a consulta e o registro para o caso correto sem ajuda? | Observação de UT01 | Sucesso, erros e ajuda | MU01: pelo menos 80% de conclusões corretas sem ajuda |
| QA02 | Quanto tempo exige a conclusão correta? | Cronometragem de UT01 | Tempo por tentativa e mediana das conclusões autônomas | MU02: mediana até 5 minutos, somente considerada atendida se MU01 também for |
| QA03 | Qual a satisfação com a experiência? | Pergunta após cada tarefa | Resposta ordinal de 1 a 5, inclusive após falha | MU03: mediana pelo menos 4 em UT01; demais tarefas relatadas separadamente |
| QA04 | O gestor distingue insuficiência de estabilidade e evita conclusão sobre a pessoa? | Observação e explicação após UT02 | Interpretação verbal e encaminhamento registrado | MU04: 100% do grupo reconhece a insuficiência sem conclusão indevida |
| QA05 | O gestor reconhece que o registro falhou e consegue recuperar a ação? | Observação de UT03, somente após implementar o caminho | Nova tentativa, ajuda e conferência do registro | MU05: pelo menos 80% recuperam e conferem sem ajuda |
| QA06 | Há problemas de feedback, consistência, prevenção ou recuperação? | Inspeção heurística | Evidência por tela, princípio relacionado e consequência provável | Nenhum bloqueio crítico conhecido nos caminhos liberados para teste; não equivale a ausência de problemas no produto |
| QA07 | As cinco etapas essenciais podem ser realizadas por teclado? | Inspeção técnica em implementação compatível | Localizar, abrir detalhes, preencher, confirmar e voltar, com foco visível | MU06: 5/5 etapas sem bloqueio. Não avaliável em protótipo sem suporte correspondente |
| QA08 | O gestor interpreta separadamente comunicação e tarefas? | Observação de UT01 e pergunta pós-tarefa | Explicação sobre cada dimensão e os limites da sinalização | Não confundir alteração comunicacional com piora nas entregas, diagnóstico ou justificativa automática para punição |
| QA09 | A colaboradora envia o contexto ao destinatário correto e confere o recebimento sem ajuda? | Observação de UT04 | Sucesso, ajudas, destinatário conferido e estado “Recebida” identificado | MU07: pelo menos 80% de conclusões sem ajuda |
| QA10 | A colaboradora interpreta a explicação separando comunicação e tarefas, sem tomá-la como avaliação pessoal? | Pergunta neutra após a leitura de F15 em UT04 | Explicação verbal sobre o que a análise diz e não diz | MU08: 100% do grupo separa as dimensões e não a interpreta como avaliação |

## C. Escopo e participantes

| Item | Planejamento |
|---|---|
| Perfis | Gestores, líderes ou coordenadores com experiência recente em acompanhamento direto de colaboradores (T01); colaboradores adultos com gestor direto que utilizam ferramentas de comunicação e gerenciamento de tarefas no trabalho (T03). Rafael e Maria representam os perfis de interesse e não são participantes reais. |
| Critérios de inclusão/exclusão | Para T01, incluir adultos que acompanharam diretamente uma equipe nos últimos seis meses. Para T03, incluir adultos com gestor direto que utilizaram chat e ferramentas de tarefas no trabalho nos últimos seis meses. Todos devem consentir com a participação. Excluir integrantes do projeto no teste principal e pessoas subordinadas a quem conduz a avaliação. Não exigir uso específico de Telegram ou Trello, nem excluir participantes por necessidades de acessibilidade; providenciar condições de participação e registrar os limites do protótipo. |
| Nº de participantes | Meta exploratória: cinco gestores para o fluxo T01 e pelo menos um colaborador para T03 no teste principal, além de uma pessoa elegível para o piloto, analisada separadamente. Três avaliadores na inspeção heurística, preferencialmente não autores dos fluxos inspecionados. A quantidade final dependerá da disponibilidade e da orientação docente, considerando a participação de pelo menos um usuário por integrante da equipe. Os números são planejados e não representam recrutamento realizado ou amostra estatística da população. |
| Ambiente | Preferencialmente presencial em sala tranquila, sem supervisores do participante. Se remoto, registrar a mudança, condições de conexão e dispositivo; não misturar diferenças de ambiente sem relatá-las. |
| Dispositivo | Notebook/computador com teclado e mouse ou dispositivo de entrada habitual do participante. Registrar resolução, navegador e zoom efetivos; não impor barreira de acesso para uniformizar condições. |
| Protótipo/versão | Arquivo Figma da Entrega 11. Para T01, telas F06–F13 e estados complementares de M01. Para T03, telas F14–F18, incluindo F15-vazio, F16-conversa, F16-E1, F16-E2, F16-sair, F18-aguardando e F18-esclarecida. Congelar uma cópia identificada como versão de teste com data e link após corrigir bloqueios. Verificar as interações antes de liberar cada tarefa para avaliação. |
| Teste piloto | Uma pessoa elegível antes do teste principal; participante e data a confirmar. Validar enunciados, duração, dados fictícios, links, registro de observações e recuperação simulada. Conferir se o fluxo da colaboradora permite consultar a explicação, enviar contexto e verificar o recebimento. Se o instrumento mudar, versionar; não somar os resultados do piloto aos principais. |

## D. Lista de tarefas de avaliação

| ID | Cenário neutro entregue ao usuário | Objetivo oculto da avaliação | Critério de sucesso | Tempo-limite (se houver) |
|---|---|---|---|---|
| UT01 | Você é responsável por esta equipe e está preparando uma conversa com M. F. Consulte as informações do ciclo 22/10 a 05/11 e deixe registrado o próximo passo que considera adequado, explicando o motivo. Confira o resultado antes de terminar | T01/O01; localizar, conferir suficiência, interpretar e registrar sem diagnóstico; MU01–MU03 e QA08 | Caso e período corretos, interpretação sem confundir eixos, encaminhamento justificado, responsável e retomada quando aplicável, com confirmação conferida. Aceitar decisões diferentes se coerentes, sem exigir uma opção específica | 10 minutos |
| UT02 | Em outro caso fictício de acompanhamento, você precisa decidir o próximo passo para este colaborador e ciclo. Examine as informações disponíveis, registre o que considera adequado e confira o resultado | T01/O08; reconhecer insuficiência sem induzir “aguardar dados”; MU04 | Identifica falta de dados, não conclui estabilidade nem problema da pessoa, registra a limitação e um responsável pela retomada e confere a confirmação | 10 minutos |
| UT03 | Você precisa concluir o registro deste acompanhamento para que ele possa ser retomado depois. Faça o registro e confira se a tarefa foi concluída | T01/O10; sistema apresenta falha simulada na primeira tentativa de salvar, sem anunciar a resposta correta ao participante; MU05 | Reconhece que não salvou, recupera sem ajuda, preserva/corrige conteúdo e confere sucesso. A falha provocada não conta como erro do participante | 10 minutos; executar somente após preparar e verificar o estado de falha |
| UT04 | Você é colaboradora de uma equipe de desenvolvimento. Seu gestor comentou que suas mensagens parecem mais curtas e você recebeu um aviso de que uma explicação do seu ciclo foi compartilhada. Entenda o que foi observado, explique o seu contexto para o gestor e confira se ele recebeu | T03/O25–O30; separar comunicação e tarefas; perceber o destinatário; distinguir “Recebida” de “Respondida”; MU07 e MU08 | Abrir a explicação, enviar mensagem ao destinatário correto e apontar o estado “Recebida” sem ajuda; explicar que a análise não é uma avaliação pessoal | 8 minutos |

> Uma boa instrução descreve o objetivo do participante sem dizer **onde clicar** ou usar o rótulo exato do controle que está sendo testado.

## E. Instrumentos

- [Modelo de termo de consentimento](../instrumentos/termo_consentimento_modelo.md)
- [Roteiro de teste](../instrumentos/roteiro_teste_usabilidade.md)
- [Planilha de observação](../instrumentos/planilha_observacao_modelo.md)
- [Formulário de avaliação heurística](../instrumentos/formulario_heuristica_modelo.md)
- - Perguntas pós-tarefa da UT04:
  - O que essa explicação diz sobre você e o que ela não diz?
  - Para quem foi a sua mensagem?
  - Como você sabe se ela foi recebida?
  - Qual foi a principal dificuldade durante a tarefa?
  - O que você manteria ou mudaria na interface?
  - Qual foi seu nível de satisfação com a experiência, em uma escala de 1 (muito insatisfeito) a 5 (muito satisfeito)?
    
### Procedimento de aplicação — UT04

**Responsável:** Tainá Cunha Bueno — 22.119.025-9

1. Apresentar o objetivo acadêmico da avaliação e obter o consentimento do participante.
2. Explicar que a avaliação se refere à interface, e não ao desempenho da pessoa.
3. Abrir o protótipo na tela F14 — Sobre minhas análises, sem apresentar previamente as demais telas.
4. Ler o cenário da tarefa UT04 e iniciar a cronometragem.
5. Solicitar que o participante pense em voz alta durante a interação, sem indicar onde clicar.
6. Registrar ações, dúvidas, erros, pedidos de ajuda e dificuldades de interpretação.
7. Encerrar a cronometragem quando o participante concluir a tarefa, desistir ou atingir o tempo-limite.
8. Aplicar as perguntas pós-tarefa e registrar a satisfação.
9. Agradecer a participação e armazenar as observações de forma anonimizada.

Os dados utilizados durante a tarefa são fictícios. O participante não deverá fornecer informações profissionais ou pessoais reais para preencher a mensagem de contexto.

## F. Plano de análise

### Plano de análise — UT04

| Critério | Forma de análise |
|---|---|
| Sucesso total | O participante consulta a explicação, envia a mensagem ao destinatário correto e identifica o estado “Recebida”, sem ajuda. |
| Sucesso parcial | O participante realiza parte das etapas ou conclui o fluxo com ajuda da avaliadora. |
| Falha | O participante não consegue enviar a mensagem, identifica incorretamente o destinatário, não reconhece o recebimento ou abandona a tarefa sem concluí-la. |
| Erros | Registrar ações incorretas, seleção de opções inadequadas, tentativas de envio inválidas e interpretações equivocadas que afetem a execução. |
| Dúvidas | Registrar hesitações, perguntas e dificuldades de compreensão, mesmo quando não resultarem em erro. |
| Ajudas | Contabilizar cada intervenção da avaliadora que forneça orientação necessária à continuidade da tarefa. |
| Tempo | Medir desde o término da leitura do enunciado até a conclusão, desistência ou tempo-limite de 8 minutos. |
| Satisfação | Registrar a resposta individual em escala de 1 a 5. |
| Observações qualitativas | Organizar falas e comportamentos por tela, etapa da tarefa e problema identificado, distinguindo observação de interpretação da avaliadora. |
| Priorização | Considerar o impacto sobre a compreensão, a conclusão da tarefa, a privacidade e a possibilidade de recuperação. |

#### Comparação com as metas de usabilidade

| Meta | Forma de cálculo | Critério de atendimento |
|---|---|---|
| MU07 — Eficácia | Número de participantes que enviaram o contexto ao destinatário correto e conferiram o recebimento sem ajuda, dividido pelo total de tentativas válidas de UT04, multiplicado por 100 | Pelo menos 80% |
| MU08 — Compreensão | Número de participantes que distinguiram corretamente comunicação e tarefas e reconheceram que a análise não representa uma avaliação pessoal, dividido pelo total de participantes avaliados em UT04, multiplicado por 100 | 100% |

A compreensão será avaliada separadamente do sucesso operacional, utilizando as respostas pós-tarefa. Um participante pode concluir a navegação corretamente e ainda apresentar uma interpretação equivocada da análise.

Os resultados serão apresentados por meio de contagens, tempos, satisfação e observações qualitativas. Caso apenas um participante realize UT04, os resultados serão registrados como 0/1 ou 1/1, com indicação explícita da limitação da amostra.

Os problemas identificados serão relacionados às telas F14–F18, ao MoLIC M03 e à tarefa T03, permitindo a comparação com os achados da avaliação heurística da Entrega 13.

As metas de usabilidade serão consideradas atendidas ou não atendidas apenas após a realização do teste com participantes reais.

Defina antes dos testes:

- sucesso total / parcial / falha;
- o que conta como erro, dúvida, ajuda e abandono;
- como tempo será medido;
- escala de satisfação pós-tarefa;
- como observações/falas serão codificadas;
- como problemas serão priorizados;
- como comparar resultados às metas de usabilidade.

## Checklist

- [ ] As seis etapas DECIDE foram contextualizadas, não apenas expandidas por sigla.
- [ ] Perguntas de avaliação têm método e evidência correspondentes.
- [ ] O plano distingue avaliação de IHC de avaliação técnica/científica do TCC.
- [ ] Dados ou processamentos simulados no protótipo estão declarados.
- [ ] Tarefas vêm de objetivos/cenários relevantes.
- [ ] Critérios de sucesso foram definidos antes da coleta.
- [ ] Questões práticas e éticas estão resolvidas.
- [ ] Instrumentos estão prontos antes da Entrega 13/14.
- [ ] Plano diz como dados serão analisados e apresentados.
