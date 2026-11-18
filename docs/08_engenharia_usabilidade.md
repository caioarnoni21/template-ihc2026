# Entrega 8 — Ciclo de vida e engenharia de usabilidade

**Data:** 18/11/2026  
**Status:** 🟩 Concluida  
**Responsabilidade:** 1 solução por equipe

## Objetivo da atividade

Transformar o conhecimento acumulado sobre usuários, tarefas, plataforma e contexto em princípios e **metas de usabilidade verificáveis**, mantendo o caráter iterativo do projeto.

## Delimitação do sistema interativo

Antes das características da plataforma, separe:

| Camada | O que pertence ao projeto | O que será avaliado em IHC |
|---|---|---|
| contribuição técnica do TCC | Análise de alterações em padrões comunicacionais e indicadores profissionais em relação ao histórico individual, com resultados separados e informações explicativas | Se o gestor compreende a apresentação e os limites dos resultados. A qualidade dos modelos, cálculos e detecção exige avaliação técnica própria do TCC |
| camada de interação da disciplina | Visão da equipe, localização de colaborador e período, consulta de evidências, registro de encaminhamento e confirmação | Compreensão, conclusão da tarefa, tempo de interação, satisfação, erros e acesso aos controles necessários |
| integrações/dados simulados | Casos fictícios representando dados de comunicação e tarefas associados às fontes previstas, Telegram e Trello; estados completo, incompleto e falha de registro simulados | Navegação e interpretação desses estados. Não serão comprovados integração real, persistência em produção, segurança do servidor ou tempo real de processamento |

Em um protótipo de disciplina, é aceitável simular processamento ou resultados quando a implementação técnica não estiver integrada, desde que isso seja declarado e a simulação seja suficiente para avaliar a interação.

## 1. Características da plataforma

| Característica | Descrição | Consequência para IHC |
|---|---|---|
| Software | Interface web prevista para uso por gestores; versão atual em papel, seguida por protótipo navegável. Linguagens e infraestrutura de produção não estão definidas nesta entrega | Organizar navegação consistente entre equipe, análise e registro; não vincular metas de interação a uma implementação ainda inexistente |
| Hardware/dispositivos | Computador ou notebook como hipótese prioritária, com teclado e mouse. | Aproveitar espaço para comparação e leitura sem depender de uma resolução única; prever ampliação e navegação por teclado no protótipo implementado |
| Capacidades | Apresentar resumo da equipe, comparar dados com o histórico do próprio colaborador, mostrar limites e registrar uma decisão humana | Separar comunicação e tarefas; permitir conferir identidade, período e cobertura antes de registrar; priorizar informações da decisão, não todas as métricas disponíveis |
| Restrições | Dados incompletos, interpretações ambíguas e ausência de integração técnica no protótipo. O sistema não estabelece diagnóstico nem medida disciplinar | Diferenciar insuficiência de estabilidade; não transformar uma sinalização em veredito; manter o encaminhamento sob responsabilidade humana |
| Conectividade/latência | A versão web integrada dependerá de rede. A latência real ainda não foi medida; falhas podem ser simuladas | Exibir carregamento e falha; preservar campos na tentativa de recuperação e informar quando o registro não foi concluído |
| Segurança/privacidade | A interface trata informações potencialmente identificáveis sobre colaboradores; os testes usarão casos fictícios | Restringir visualização à equipe autorizada, evitar exposição desnecessária e permitir ocultar nomes. Iniciais não equivalem a anonimização nem substituem controle de acesso |
| Volume de dados/histórico |  Volume real ainda desconhecido. O projeto prevê comparação com histórico individual, com janelas de referência de 30 dias e análise de 15 dias | Tornar período e identidade visíveis. Investigar necessidade de busca, filtros e paginação conforme a escala real, sem incluí-los apenas por convenção |
| Tempo de processamento | Duração do cálculo técnico não estabelecida; resultados serão preparados para os testes de interação | Diferenciar processamento, indisponibilidade e resultado pronto; não usar a rapidez da simulação como evidência de desempenho do algoritmo |
| Papéis/permissões | Gestor como usuário direto; colaborador como pessoa afetada. RH e administração técnica têm responsabilidades a esclarecer | Limitar o gestor aos casos autorizados e separar decisões de acompanhamento das configurações técnicas. Permissões representadas no protótipo não comprovam proteção em produção |

## 2. Princípios gerais do projeto

Inclua apenas normas, leis, padrões e princípios realmente relevantes, explicando **como** afetam o projeto. Não transforme esta seção em lista de links.

| Princípio/norma | Aplicabilidade ao contexto | Decisão/requisito decorrente | Fonte |
|---|---|---|---|
| Contexto de uso | Rafael consulta informações da equipe para decidir e registrar um acompanhamento, possivelmente com pouco tempo e interrupções; contexto ainda a validar | Manter colaborador e período identificáveis; oferecer retorno sem perder o rascunho durante a navegação e organizar a tarefa em localizar, avaliar e registrar | Entregas 1, 3, 4 e 5; coleta planejada na Entrega 7 |
| LGPD: finalidade, necessidade, transparência e segurança | O eventual tratamento de dados reais de colaboradores exige delimitação de finalidade, acesso e proteção | Usar dados fictícios no protótipo; apresentar finalidade e limites; minimizar dados exibidos e coletados. Antes de integração real, definir base legal e governança com os responsáveis, sem presumir que consentimento isolado resolve o tratamento | [LGPD, arts. 6º e 46, texto da Câmara dos Deputados](https://www2.camara.leg.br/legin/fed/lei/2018/lei-13709-14-agosto-2018-787077-normaatualizada-pl.html) |
| Acessibilidade: WCAG 2.2, critérios aplicáveis dos níveis A e AA | Leitura dos indicadores, compreensão dos estados e preenchimento do registro não devem depender apenas de visão de cores ou uso do mouse | Usar texto além de cor; contraste de texto de pelo menos 4,5:1, ou 3:1 para texto grande; controles operáveis por teclado, foco visível, rótulos e erros identificáveis. Inspecionar critérios aplicáveis; não declarar conformidade completa a partir de uma tela em papel | [W3C: WCAG 2.2, 1.4.1, 1.4.3, 2.1.1, 2.4.7, 3.3.1 e 3.3.2](https://www.w3.org/TR/WCAG22/) |
| Visibilidade do estado e recuperação de erros | O gestor precisa diferenciar análise em andamento, incompleta e pronta, além de saber se registrou sua decisão | Apresentar estado, atualização e confirmação com caso e período; em falha, preservar o preenchimento e permitir tentar novamente | [Nielsen: heurísticas 1 e 9](https://www.nngroup.com/articles/ten-usability-heuristics/) |
| Correspondência com a linguagem do usuário, consistência e prevenção de erros | Termos técnicos e ações conclusivas podem prejudicar a interpretação | Testar rótulos como “padrão individual” e “análise incompleta”; manter termos consistentes; conferir caso e período antes do registro e evitar “Está tudo certo” como conclusão antecipada | [Nielsen: heurísticas 2, 4 e 5](https://www.nngroup.com/articles/ten-usability-heuristics/) |

## 3. Metas de usabilidade

Usabilidade deve ser discutida **no contexto de uso**. Metas quantitativas devem dizer o que será medido, em qual tarefa, com qual população e qual limite será considerado aceitável.

### 3.1 Metas qualitativas

| Meta | Para quem/tarefa | Evidência desejada | Justificativa |
|---|---|---|---|
| Compreender que sinalização não é diagnóstico | Rafael / avaliar evidências de T01 | Participante explica o resultado como alteração que exige contexto, sem concluir sobre saúde ou determinar punição | Evitar atribuir ao sistema uma autoridade que os dados não sustentam |
| Distinguir análise incompleta de ausência de alteração | Rafael / conferir suficiência dos dados | Participante reconhece a limitação e registra pendência, sem tratar falta de dados como estabilidade | Reduzir risco de decisão baseada em informação insuficiente |
| Interpretar comunicação e tarefas separadamente | Rafael / comparar resultados com o próprio histórico | Participante identifica que alteração comunicacional não implica necessariamente alteração nas entregas | Preservar o significado dos resultados separados do TCC |
| Localizar e manter o contexto do caso | Rafael / localizar análise e registrar próximo passo | Participante confere identidade e período e consegue voltar sem trocar de caso inadvertidamente | Evitar registro atribuído à pessoa ou ao ciclo errado |
| Reconhecer conclusão e recuperar falha | Rafael / registrar e conferir o resultado | Participante distingue tentativa de envio de confirmação e sabe como corrigir ou tentar novamente | Evitar falsa impressão de registro concluído |
| Perceber clareza e controle na decisão | Rafael / T01 completa | Participante relata com suas palavras o que decidiu, por quê e o que o sistema registrou | A interface deve apoiar a decisão humana e tornar sua consequência compreensível |

### 3.2 Metas quantitativas

| ID | Dimensão | Métrica | Tarefa/escopo | Meta | Como medir | Justificativa |
|---|---|---|---|---|---|---|
| MU01 | Eficácia | Percentual de participantes que concluem corretamente sem ajuda do moderador | T01, caso com dados suficientes | Pelo menos 80% | Número de conclusões sem ajuda dividido pelo total de tentativas válidas; verificar caso, período, justificativa, responsável e confirmação | Alvo inicial para conclusão autônoma do fluxo central |
| MU02 | Eficiência | Tempo mediano das conclusões corretas sem ajuda | Mesmo caso de MU01, em protótipo navegável | Até 5 minutos; considerar atendida somente se MU01 também for atingida | Cronometrar da apresentação da tela inicial, após leitura da tarefa, até conferência da confirmação. Relatar também duração e número de falhas e desistências | Alvo provisório de consulta breve; evita premiar rapidez obtida por desistência ou conclusão incorreta |
| MU03 | Satisfação | Mediana da resposta à pergunta pós-tarefa “Quão satisfeito você ficou com a experiência de realizar esta tarefa?” | T01, incluindo tentativas não concluídas | Pelo menos 4 em escala de 1 a 5 | Aplicar imediatamente após a tentativa: 1 muito insatisfeito, 2 insatisfeito, 3 nem satisfeito nem insatisfeito, 4 satisfeito, 5 muito satisfeito; registrar omissões e distribuição | Complementar desempenho observado com percepção do participante, sem confundir satisfação com eficácia |
| MU04 | Compreensão e prevenção de erro crítico | Percentual que identifica insuficiência e não faz conclusão sobre a pessoa a partir dos dados ausentes | T01, variante com análise incompleta | 100% no grupo avaliado | Perguntar de forma neutra “O que é possível concluir e qual seria seu próximo passo?”; conferir interpretação e registro, sem sugerir a resposta | A gravidade da interpretação equivocada justifica meta mais restritiva; não garante ausência de risco fora da amostra |
| MU05 | Recuperação de erro | Percentual que recupera uma falha de salvamento simulada sem ajuda e confere o registro | T01, variante com falha de registro | Pelo menos 80% | Apresentar a mesma falha após a primeira confirmação; observar nova tentativa e conferência do sucesso, com campos preservados | Verificar se o usuário distingue falha de persistência e consegue terminar |
| MU06 | Acessibilidade operacional | Proporção das etapas essenciais executáveis por teclado sem bloqueio e com foco visível | Localizar análise, abrir detalhes, preencher, confirmar e voltar em T01 | 100% das cinco etapas | Inspeção manual no protótipo web implementado, sem mouse; registrar resultado por etapa. No papel ou protótipo sem suporte a teclado, marcar não avaliável | Estabelecer um critério específico de acesso, sem substituir avaliação ampla de acessibilidade ou conformidade WCAG |

### 3.3 Priorização das metas (se exigida na disciplina)

Se o professor solicitar porcentagens que somem 100%, trate-as como **peso de prioridade**, não como métrica de usabilidade.

| Meta | Peso de prioridade | Justificativa |
|---|---:|---|
| MU01 — Conclusão correta | 25% | A interface precisa permitir completar a tarefa central |
| MU02 — Tempo de execução | 10% | Rapidez importa, mas não deve superar compreensão e segurança |
| MU03 — Satisfação | 10% | A percepção de uso complementa o desempenho observado |
| MU04 — Compreensão de insuficiência | 30% | Interpretação incorreta pode afetar decisões sobre colaboradores |
| MU05 — Recuperação de falha | 15% | Um registro não concluído precisa ser reconhecido e recuperável |
| MU06 — Acesso por teclado | 10% | O fluxo não deve excluir usuários dependentes de teclado |
| **Total** | **100%** | |

## 4. Como o ciclo será iterado

Explique que artefatos serão revisitados após protótipos e avaliações.

1. **Revisar requisitos:** aplicar o instrumento da Entrega 7 e confrontar resultados com personas, contexto, cenários e hipóteses da Entrega 1. Se os gestores não realizarem a atividade prevista, rever T01 e o escopo antes de aperfeiçoar telas sem utilidade demonstrada.
2. **Revisar o projeto essencial:** completar no papel a análise individual, o registro, a confirmação e os estados incompleto e de erro. Simular com alguém que não elaborou as telas; registrar observações reais, sem substituir participantes por respostas de IA.
3. **Consolidar padrões:** registrar no guia de estilo os termos escolhidos, estados, controles, hierarquia e regras de acesso. Aplicar as decisões de forma consistente à visão geral e às telas de detalhe e registro.
4. **Detalhar e inspecionar:** produzir o protótipo navegável com os caminhos necessários. Nas Entregas 12–14, conforme o roteiro da disciplina, realizar inspeções e testes compatíveis com sua fidelidade; corrigir bloqueios antes de medir as metas.
5. **Avaliar e revisar:** comparar cada medida com a meta registrada. Priorizar erros de interpretação, caso/período incorreto, falsa confirmação e bloqueios de acesso; depois, dificuldades de navegação, tempo e satisfação. Anotar o que mudou, por qual evidência e em qual versão.
6. **Reavaliar:** testar a versão revisada com casos equivalentes, identificando participantes novos e recorrentes. Atualizar as Entregas 3–6 e 8, o guia de estilo e `RASTREABILIDADE.md`. Preservar o histórico, inclusive quando uma hipótese for refutada ou uma meta não for atingida.

## Checklist

- [ ] Capacidades e restrições têm impacto de IHC explicitado.
- [ ] Está claro o limite entre contribuição técnica do TCC e camada interativa da disciplina.
- [ ] Resultados/processamento simulados no protótipo foram explicitados.
- [ ] Metas de usabilidade avaliam a interação, não substituem métricas técnicas do TCC.
- [ ] Normas/princípios estão contextualizados, não apenas copiados.
- [ ] Metas quantitativas são mensuráveis e associadas a tarefas/público.
- [ ] Eficácia, eficiência e satisfação são consideradas quando pertinentes.
- [ ] Metas poderão ser verificadas nas Entregas 12–14.
