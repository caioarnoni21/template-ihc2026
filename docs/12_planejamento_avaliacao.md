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

| Etapa | Aplicação no projeto |
|---|---|
| D — Determine the goals | Verificar conclusão autônoma de T01 (MU01), tempo (MU02), satisfação (MU03), compreensão da insuficiência (MU04), recuperação de falha (MU05) e acesso por teclado quando tecnicamente avaliável (MU06). Priorizar interpretação responsável e registro correto sobre rapidez |
| E — Explore the questions | Investigar se gestores localizam a pessoa e o período corretos, distinguem comunicação de tarefas, reconhecem limitações, registram um encaminhamento coerente e conferem o resultado. Examinar feedback, consistência, controle e recuperação |
| C — Choose the evaluation paradigm and techniques | Avaliação formativa: inspeção heurística independente por avaliadores para a Entrega 13, seguida de teste observado com gestores para a Entrega 14. Usar perguntas pós-tarefa para esclarecer interpretação e satisfação; opinião isolada não substitui observação |
| I — Identify the practical issues | Planejar três avaliadores, um participante de piloto e cinco gestores no teste principal, sujeitos à disponibilidade e orientação docente. Usar notebook, navegador, Figma e cronômetro em ambiente tranquilo. Caio prepara materiais e modera; observador e avaliadores serão definidos pela equipe. Inspecionar, corrigir bloqueios, realizar piloto, congelar versão e então testar |
| D — Decide how to deal with ethical issues | Explicar propósito acadêmico, voluntariedade, riscos e direito de interromper. Usar apenas casos fictícios, sem solicitar dados de colegas ou empresas. Registrar notas por códigos, sem gravação por padrão; guardar consentimento separado. Não publicar dados brutos nem avaliar desempenho profissional dos participantes |
| E — Evaluate, interpret and present the data | Consolidar contagens, tempos, satisfação e evidências qualitativas por tarefa. Comparar às metas originais, registrar omissões, ajuda e limitações. Priorizar problemas pela consequência, frequência observada e possibilidade de recuperação, mantendo inspeção e teste humano separados |

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

## C. Escopo e participantes

| Item | Planejamento |
|---|---|
| Perfis | Gestores, líderes ou coordenadores com experiência recente em acompanhamento direto de colaboradores; Rafael representa o perfil, não um participante real |
| Critérios de inclusão/exclusão | Incluir adultos que acompanharam diretamente uma equipe nos últimos seis meses e consentiram. Excluir autores das telas do teste principal. Não exigir uso de Telegram/Trello nem excluir por necessidade de acessibilidade; providenciar condições de participação e registrar limites do protótipo |
| Nº de participantes | Meta exploratória: cinco gestores no teste principal e uma pessoa elegível no piloto, analisada separadamente; três avaliadores na inspeção, preferencialmente não autores dos fluxos. Números planejados, não recrutamento realizado. Não representam amostra estatística da população |
| Ambiente | Preferencialmente presencial em sala tranquila, sem supervisores do participante. Se remoto, registrar a mudança, condições de conexão e dispositivo; não misturar diferenças de ambiente sem relatá-las |
| Dispositivo | Notebook/computador com teclado e mouse ou dispositivo de entrada habitual do participante. Registrar resolução, navegador e zoom efetivos; não impor barreira de acesso para uniformizar condições |
| Protótipo/versão | Arquivo Figma da Entrega 11, telas F06–F13 e estados complementares de M01. Congelar uma cópia identificada como versão de teste com data e link após corrigir bloqueios. A versão atualmente documentada ainda não está liberada para todas as tarefas |
| Teste piloto | Uma pessoa elegível antes do teste principal; nome e data a confirmar. Validar enunciados, duração, dados fictícios, links, registro de observações e recuperação simulada. Se o instrumento mudar, versionar; não somar os resultados do piloto aos principais |

## D. Lista de tarefas de avaliação

| ID | Cenário neutro entregue ao usuário | Objetivo oculto da avaliação | Critério de sucesso | Tempo-limite (se houver) |
|---|---|---|---|---|
| UT01 | Você é responsável por esta equipe e está preparando uma conversa com M. F. Consulte as informações do ciclo 22/10 a 05/11 e deixe registrado o próximo passo que considera adequado, explicando o motivo. Confira o resultado antes de terminar | T01/O01; localizar, conferir suficiência, interpretar e registrar sem diagnóstico; MU01–MU03 e QA08 | Caso e período corretos, interpretação sem confundir eixos, encaminhamento justificado, responsável e retomada quando aplicável, com confirmação conferida. Aceitar decisões diferentes se coerentes, sem exigir uma opção específica | 10 minutos |
| UT02 | Em outro caso fictício de acompanhamento, você precisa decidir o próximo passo para este colaborador e ciclo. Examine as informações disponíveis, registre o que considera adequado e confira o resultado | T01/O08; reconhecer insuficiência sem induzir “aguardar dados”; MU04 | Identifica falta de dados, não conclui estabilidade nem problema da pessoa, registra a limitação e um responsável pela retomada e confere a confirmação | 10 minutos |
| UT03 | Você precisa concluir o registro deste acompanhamento para que ele possa ser retomado depois. Faça o registro e confira se a tarefa foi concluída | T01/O10; sistema apresenta falha simulada na primeira tentativa de salvar, sem anunciar a resposta correta ao participante; MU05 | Reconhece que não salvou, recupera sem ajuda, preserva/corrige conteúdo e confere sucesso. A falha provocada não conta como erro do participante | 10 minutos; executar somente após preparar e verificar o estado de falha |

> Uma boa instrução descreve o objetivo do participante sem dizer **onde clicar** ou usar o rótulo exato do controle que está sendo testado.

## E. Instrumentos

- [Modelo de termo de consentimento](../instrumentos/termo_consentimento_modelo.md)
- [Roteiro de teste](../instrumentos/roteiro_teste_usabilidade.md)
- [Planilha de observação](../instrumentos/planilha_observacao_modelo.md)
- [Formulário de avaliação heurística](../instrumentos/formulario_heuristica_modelo.md)
- {{questionário pré/pós-teste}}

## F. Plano de análise

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
