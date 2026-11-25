# Entrega 11 — Protótipo no Figma

**Data:** {{22/11/2026}}  
**Status:** 🟨 Em andamento
**Responsabilidade:** 1 protótipo integrado por equipe cobrindo os fluxos MoLIC. Se a turma exigir divisão individual, identifique o responsável por cada fluxo/tela.

## Objetivo da atividade

Materializar o modelo de interação em um protótipo navegável, preservando a lógica dos objetivos, tópicos, signos, feedbacks, alternativas e recuperações definidos anteriormente.

## Biblioteca de possibilidades para projetos técnicos

O protótipo deve materializar os fluxos definidos nas entregas anteriores. Dependendo do escopo, podem fazer sentido:

1. **Dashboard:** indicadores, alertas, estado, tendências e atalhos para tarefas frequentes.
2. **Configuração/parametrização:** escolhas, presets, validação e explicação de opções técnicas.
3. **Entrada de dados:** upload, conexão, seleção, pré-visualização e validação.
4. **Processamento:** fila, status, progresso, cancelamento, falha e reexecução.
5. **Relatório/resultados:** síntese, métricas, gráficos, explicação, exportação e compartilhamento.
6. **Histórico:** busca, filtros, ordenação, paginação, detalhes e repetição de execução.
7. **Comparação:** antes/depois, modelo A/B, execução A/B, baseline ou períodos.
8. **Explicabilidade:** confiança, fatores, evidências, limitações e correção/contestação.
9. **Administração:** usuários, grupos, perfis, permissões, integrações e políticas.
10. **CRUDs de domínio:** somente quando criar/consultar/editar/excluir representa tarefa real.
11. **Auditoria/logs:** histórico de alterações e eventos em linguagem adequada.
12. **Alertas/ocorrências:** severidade, impacto, ação, responsável e resolução.
13. **Ajuda/documentação:** apoio contextual a tarefas complexas.

### Estados que não podem ser esquecidos

Quando aplicável, considere: vazio/sem dados; carregamento/processamento; sucesso; erro de entrada; erro de processamento; filtro sem resultados; permissão insuficiente; confirmação de ação destrutiva; cancelamento/desfazer/recuperação; dados desatualizados/conflito.

> Esta lista é repertório de design, **não uma exigência de quantidade de telas**. A rastreabilidade deve explicar por que cada tela existe.

## Link do Figma
**Autor:** Guilherme Matias RA: 22.122.071-8 e Caio Arnoni 22.221.019-7 <br>
**Protótipo:** https://www.figma.com/design/McbDfvqqGuDnR9uDmBdJrp/Login-e-Cadastro-de-Colaboradores?node-id=0-1&t=KVpUb4PCjVZbOSQ0-1 <br>
**Arquivo editável:** https://www.figma.com/design/McbDfvqqGuDnR9uDmBdJrp/Login-e-Cadastro-de-Colaboradores?node-id=0-1&t=KVpUb4PCjVZbOSQ0-1  <br>
**Última verificação de permissão:** {{22/11/2026}}

> Teste o link em janela anônima. O avaliador deve conseguir abrir o protótipo sem solicitar permissão.

## Cobertura MoLIC → Figma

| MoLIC | Objetivo | Fluxo/telas no Figma | Estados de erro/recuperação | Responsável |
|---|---|---|---|---|
| M01, C1 | O02 — Localizar a análise pertinente | F06 apresenta equipe, ciclo e acesso à sinalização de M. F. | Seleção de outro período e consulta indisponível de C7 não demonstradas nas imagens | Caio Arnoni: documentação de T01; autoria visual a confirmar |
| M01, C3 | O03/O07 — Interpretar evidências e limites | F07 separa comunicação e atividades, com explicações do significado | Explicações presentes; interação dos controles ainda não percorrida integralmente | Caio Arnoni: documentação de T01 |
| M01, C2/C8 | O06/O08 — Conferir cobertura e reconhecer insuficiência | F08 mostra cobertura suficiente; F09 representa análise incompleta | Aviso de dados ausentes, retorno e encaminhamento para aguardar dados representados | Caio Arnoni: documentação de T01 |
| M01, C4/C5 | O04/O05 — Definir e revisar encaminhamento | F10, variante F12 e ações de confirmação | Justificativa e opções visíveis; validação, responsável, data de retomada e revisão anterior ao salvamento não demonstrados integralmente | Caio Arnoni: documentação de T01 |
| M01, C6 | O05 — Conferir registro concluído | F11 e F13; retorno de F13 a F06 verificado no navegador | Confirmações representadas; coerência entre seleção e resultado ainda requer correção/verificação | Caio Arnoni: documentação de T01 |
| M01, O09 | Retomar após interrupção | F06 tem aviso de rascunho; F10/F12 informam salvamento automático | Retomada entre sessões é prometida no texto, mas não verificada; ultrapassa a retomada na mesma sessão prevista no M01 | Caio Arnoni: documentação de T01 |
| M01, P2/P3/C9/C10 | O10 — Recuperar falha e abandonar com clareza | Não demonstrado nos oito prints | Faltam evidências de campo inválido, falha ao salvar, nova tentativa e confirmação de abandono | Caio Arnoni: documentação de T01 |
| M02b | O22 Acessar o sistema como gestor | `F01 → visão geral (M02, cena 1)` | `F01E` (e-mail ou senha incorretos; usuário sem perfil de gestor) | Guilherme Matias |
| M02b | O24 Recuperar acesso | `F01 → F02 → F02S` | `F02E` (e-mail inválido); retorno `F02 → F01` | Guilherme Matias |
| M02b | O23 Cadastrar e vincular colaborador | `F03 → F04` e `F04 → F03` (cadastrar outro) | `F03E1` (campo vazio ou formato inválido), `F03E2` (CPF, matrícula, Telegram ID ou Trello ID já vinculado), `F03E3` (falha ao salvar) | Guilherme Matias |
| M02b | O23 (saída sem salvar) | `F03 → F05` | `F05` (continuar editando ou sair sem salvar) | Guilherme Matias |
| M02 | O11 a O21 | {{telas da triagem, ainda a definir}} | {{...}} | Guilherme Matias |

## Catálogo de telas/estados

### F01 — Login do gestor

<img width="1025" height="667" alt="image" src="https://github.com/user-attachments/assets/8449b302-76fb-4e21-827c-ee29cefebf15" />

**Objetivo do usuário:** identificar-se como gestor para entrar no WorkSense (O22) e, se necessário, recuperar o acesso (O24).  
**Signos principais:** e-mail do gestor; senha; "lembrar de mim" (estado da sessão); "esqueci a senha"; aviso de acesso restrito a gestores; orientação "fale com o RH".  
**Origem no MoLIC:** M02b, cena 1 "Identificar-se como gestor", processamento "validar credenciais" e cena 2 "Recuperar acesso".

| Estado | O que o usuário vê | Origem no MoLIC |
|---|---|---|
| `F01-erro` | Mensagem "e-mail ou senha incorretos" ou "acesso permitido apenas a gestores", com os campos preservados | Retornos tracejados de "validar credenciais" à cena 1 (`RA`) |
| `F01-recuperar` | Painel ou janela "Recuperar acesso" sobre o login, com o campo de e-mail do gestor, ação "enviar" e "voltar ao login" | Cena 2 "Recuperar acesso" |
| `F01-recuperar-erro` | Mensagem junto ao campo de e-mail, que continua preenchido | Retorno tracejado de "validar e-mail e enviar instruções" à cena 2 (`RA`) |
| `F01-enviado` | Confirmação de que as instruções foram enviadas ao e-mail e ação de voltar ao login | Encerramento (`gcc`) do O24 |

### F02 — Cadastrar colaborador

<img width="1049" height="672" alt="image" src="https://github.com/user-attachments/assets/cc923bd6-ac7f-4c9c-b658-795cdf5f6228" />


**Objetivo do usuário:** cadastrar um novo colaborador e vinculá-lo às ferramentas da equipe (O23).  
**Signos principais:** nome completo; e-mail corporativo; CPF; telefone; cargo; departamento; data de admissão; matrícula; Telegram ID; Trello ID; exemplos de formato nos campos; lembrete "confira os dados antes de concluir o cadastro"; menu lateral (acesso ubíquo).  
**Origem no MoLIC:** M02b, cena 3 "Cadastrar colaborador", cena 4 "Colaborador cadastrado" e cena 5 "Alterações não gravadas".

| Estado | O que o usuário vê | Origem no MoLIC |
|---|---|---|
| `F02-erro-campo` | Mensagem junto ao campo vazio ou com formato inválido; os demais campos mantidos | Retorno tracejado de "validar dados" à cena 3 (`RA`) |
| `F02-erro-vinculo` | Mensagem indicando o dado já cadastrado ou vinculado (CPF, matrícula, Telegram ID ou Trello ID) | Retorno tracejado de "validar dados" à cena 3 (`RA`) |
| `F02-erro-salvar` | Mensagem de falha ao salvar, com os dados digitados mantidos | Retorno tracejado de "salvar cadastro" à cena 3 (`RA`) |
| `F02-cadastrado` | Confirmação com nome, matrícula e vínculos de Telegram e Trello; ações "cadastrar outro" e "concluir" | Cena 4 "Colaborador cadastrado" |
| `F02-alerta` | Janela "há alterações não gravadas" com "sair sem salvar" e "continuar editando", aberta por "Cancelar" ou por "Sair" no menu | Cena 5 (`AL`) |


### F06 — Visão geral da equipe

<img width="878" height="773" alt="image" src="https://github.com/user-attachments/assets/9aa8ff70-7077-4cea-9925-aec1d38bdfc7" />

**Objetivo do usuário:** localizar o caso que merece consulta e retomar uma atividade.  
**Signos principais:** ciclo, atualização, colaborador, situação no ciclo, último registro, sinalização, análise incompleta e rascunho.  
**Origem no MoLIC:** M01/C1 e O09.  

| Estado | O que o usuário vê | Origem no MoLIC |
|---|---|---|
| F06-equipe | Resumo do ciclo, seis pessoas dentro do padrão, uma sinalização, uma análise incompleta e lista de colaboradores com ações de consulta | M01, C1 — Localizar a análise pertinente |
| F06-retomada | Aviso de rascunho de C. M. e ação “Retomar”; funcionamento ainda não verificado | O09 — Retomar após interrupção; retomada entre sessões exige ampliar o modelo atual |
| F06-carregando (previsto) | Informação de consulta em andamento, antes de apresentar o resultado; não demonstrada nos prints | M01, P1 — Obter análise |
| F06-indisponivel (previsto) | Motivo da indisponibilidade e opção de rever caso/período ou tentar novamente; não demonstrado nos prints | M01, P1 → C7 → C1; recuperação apoiada (RA) |

### F07 — Significado da sinalização

<img width="1140" height="786" alt="image" src="https://github.com/user-attachments/assets/62392718-20e7-4320-97f9-ad3b01d1460f" />


**Objetivo do usuário:** compreender a alteração sem interpretar o resultado como diagnóstico ou punição.  
**Signos principais:** ciclo, padrão individual, comunicação, atividades, sinalização e limites.  
**Origem no MoLIC:** M01/C3.

| Estado | O que o usuário vê | Origem no MoLIC |
|---|---|---|
| F07-sinalizacao | Comparação entre comunicação e atividades de M. F., apresentadas separadamente em relação ao próprio padrão | M01, C3 — Interpretar evidências e limites |
| F07-explicacao | Blocos “O que este sinal significa” e “O que este sinal NÃO significa”, esclarecendo que não se trata de diagnóstico, avaliação de desempenho ou justificativa para punição | Diálogo de esclarecimento em C3; prevenção passiva (PP) |
| F07-prosseguir | Ações para consultar confiabilidade ou ir diretamente ao registro; ligações ainda não verificadas integralmente | Relação com C2 e C4; o atalho precisa ser reconciliado com a conferência prévia de suficiência no M01 |

### F08 — Confiabilidade: dados suficientes

<img width="1016" height="775" alt="image" src="https://github.com/user-attachments/assets/aaa531d4-3035-4f18-b9cd-17df143adcc4" />


**Objetivo do usuário:** conferir períodos, origem, cobertura e atualização antes de interpretar.  
**Signos principais:** estado da análise, referência, ciclo, dias com dados, fontes e atualização.  
**Origem no MoLIC:** M01/C2.  

| Estado | O que o usuário vê | Origem no MoLIC |
|---|---|---|
| F08-completa | Mensagem de análise completa, períodos de referência e comparação, cobertura e última atualização | M01, C2 — Conferir suficiência e atualização |
| F08-fontes | Trello e Telegram identificados como conectados, além da explicação de como a comparação é feita | Diálogo sobre fontes, cobertura e limites em C2; prevenção passiva (PP) |
| F08-detalhamento | Ações “Ver detalhes” e “O que significa?”; conteúdo de destino não apresentado nas imagens | Esclarecimento dos signos de C2; detalhamento ainda a verificar |
| F08-prosseguir | Ações para continuar ao registro ou voltar à sinalização | C4 e C3; no M01, a conferência de C2 antecede a interpretação em C3 |

### F09 — Confiabilidade: análise incompleta

<img width="1017" height="778" alt="image" src="https://github.com/user-attachments/assets/5ec34eb3-58c9-4c10-9218-563e8d00b9fe" />


**Objetivo do usuário:** reconhecer a limitação e evitar conclusão indevida.  
**Signos principais:** cobertura insuficiente, fonte ausente, período, estado incompleto e próximo passo.  
**Origem no MoLIC:** M01/C8.  

| Estado | O que o usuário vê | Origem no MoLIC |
|---|---|---|
| F09-incompleta | Aviso de falta de dados para comparação, distinto de ausência de alteração; cobertura de 6/15 dias no ciclo | M01, C2 → C8 — Reconhecer insuficiência de dados; prevenção passiva (PP) |
| F09-fonte-ausente | Telegram sem dados desde 28/10 e orientação para verificar o Telegram ID | Signos fontes, cobertura e limites em C8; captura de erro (CE) se a correção depender de responsável externo |
| F09-encaminhar | Ação para registrar “aguardar dados”, com possibilidade de voltar à visão geral | M01, C8 → C4; a volta à visão geral representa saída sem registro e requer verificar a ligação |

### F10 — Registrar encaminhamento

<img width="1216" height="776" alt="image" src="https://github.com/user-attachments/assets/b2ea2379-2c36-4086-87d2-45b28c053a3c" />


**Objetivo do usuário:** registrar sua decisão e justificativa vinculadas ao caso e ciclo.  
**Signos principais:** pessoa, período, encaminhamento, justificativa, limite de caracteres e rascunho.  
**Origem no MoLIC:** M01/C4; a revisão de C5 ainda precisa ser demonstrada.

| Estado | O que o usuário vê | Origem no MoLIC |
|---|---|---|
| F10-preenchimento | Opções de encaminhamento, justificativa, contador de caracteres e identificação do caso/ciclo; “Apoiar” selecionado no print | M01, C4 — Definir o próximo passo humano |
| F10-rascunho | Mensagem de salvamento automático e possibilidade de retomar; comportamento não verificado | O09; persistência entre sessões extrapola a conservação de contexto prevista no M01 |
| F10-erro-campo (previsto) | Mensagem no campo obrigatório ausente ou inválido, mantendo os demais dados; não demonstrada | Retorno de P2 — Validar dados para C4 (RA) |
| F10-revisao (previsto) | Resumo de caso, período e conteúdo ainda não salvo, permitindo corrigir ou confirmar; não demonstrado | M01, C5 — Conferir o encaminhamento |
| F10-salvando (previsto) | Informação de salvamento em andamento, sem afirmar sucesso antes da resposta; não demonstrada | M01, P3 — Salvar registro |
| F10-erro-salvar (previsto) | Aviso de registro não salvo, com dados preservados e ações de nova tentativa ou revisão; não demonstrado | P3 → C9, com retorno a P3 ou C5 (RA) |
| F10-abandono (previsto) | Alerta de conteúdo não salvo, com escolha entre continuar e abandonar; não demonstrado | M01, C10 — Decidir sobre abandono (AL) |

### F11 — Confirmação de encaminhamento

<img width="1241" height="776" alt="image" src="https://github.com/user-attachments/assets/5608a875-dd2d-4594-b796-7e0b5f42fdc5" />


**Objetivo do usuário:** conferir o que foi registrado e retornar à equipe.  
**Signos principais:** autor, data/hora, pessoa, ciclo, encaminhamento, justificativa e próxima revisão.  
**Origem no MoLIC:** M01/C6. 

| Estado | O que o usuário vê | Origem no MoLIC |
|---|---|---|
| F11-confirmado | Confirmação de registro, autor, data/hora, pessoa, ciclo, encaminhamento “Acompanhar”, justificativa e próxima revisão | M01, P3 → C6 — Conferir o registro concluído |
| F11-retornar | Ação “Voltar à visão geral”; destino ainda não verificado nesta variante | Encerramento de O01 após conferência em C6 e possível início de nova consulta em C1 |
| F11-historico | Ação “Ver histórico de registros”; tela de destino não apresentada | Consulta de histórico não detalhada no M01; modelar antes de afirmar cobertura |

### F12 — Registrar insuficiência

<img width="1115" height="781" alt="image" src="https://github.com/user-attachments/assets/7e5186b9-9d5e-472c-bd89-1e4c151313c1" />


**Objetivo do usuário:** registrar a pendência causada pela insuficiência.  
**Signos principais:** estado incompleto, encaminhamento, justificativa e rascunho.  
**Origem no MoLIC:** M01/C8 → C4.

| Estado | O que o usuário vê | Origem no MoLIC |
|---|---|---|
| F12-insuficiencia | Aviso de análise incompleta e orientação de que o encaminhamento disponível é aguardar dados | M01, C8 → C4; regra restritiva do protótipo a reconciliar com o modelo |
| F12-selecao | “Apoiar” e “Aguardar dados” aparecem selecionados simultaneamente; inconsistência a corrigir, não um comportamento esperado | Signo encaminhamento em C4; corrigir escolha única antes de validar em P2 |
| F12-justificativa | Texto sobre ausência de dados, limite de caracteres e ação de confirmar “aguardar dados” | Diálogo de justificativa em C4 |
| F12-erro-campo (previsto) | Orientação para corrigir informação obrigatória, preservando o conteúdo; não demonstrada | P2 → C4 (RA) |
| F12-erro-salvar (previsto) | Aviso de pendência não registrada, com possibilidade de tentar novamente; não demonstrado | P3 → C9 (RA) |
| F12-abandono (previsto) | Alerta antes de descartar o preenchimento, com opção de continuar; não demonstrado | M01, C10 (AL) |

### F13 — Confirmação de pendência

<img width="1115" height="781" alt="image" src="https://github.com/user-attachments/assets/68da7072-3f30-4fda-b60c-830fcda8c0f4" />


**Objetivo do usuário:** confirmar o registro da insuficiência e compreender como será retomado.  
**Signos principais:** estado salvo, pessoa, ciclo, justificativa, encaminhamento e próxima revisão.  
**Origem no MoLIC:** M01/C6, após a alternativa de insuficiência. 

| Estado | O que o usuário vê | Origem no MoLIC |
|---|---|---|
| F13-confirmado | Confirmação de “Aguardar dados”, pessoa, período, justificativa e autoria do registro | M01, C6, após o caminho de insuficiência C8 → C4 |
| F13-retornar | Ação “Voltar à visão geral”; retorno a F06 verificado na sessão consultada | Encerramento de O01 após C6; visão geral disponível para nova consulta |
| F13-revisao-futura | Texto “Quando o ciclo tiver dados suficientes. Você será avisado”; aviso futuro não verificado | Signos responsável e data de retomada de C4/C6 precisam ser explicitados; notificação futura não modelada em M01 |
| F13-historico | Ação “Ver histórico de registros”; destino não demonstrado | Consulta de histórico fora do detalhamento atual de M01 |

> Documente também estados que muitas equipes esquecem: carregamento, vazio, confirmação, sucesso, erro, permissão negada, cancelamento, desfazer/voltar quando aplicável.

## Sistema visual e consistência

| Elemento | Regra adotada | Justificativa |
|---|---|---|
| Tipografia | Uma única família sem serifa (Inter), com títulos em peso semibold e rótulos e apoio em peso regular ou medium | Legibilidade em formulários e hierarquia clara entre título, rótulo e texto de apoio |
| Cores | Verde-escuro para identidade e painel lateral, verde de ação para botões primários e links, fundo cinza claro e cartões brancos; mensagens de erro em cor distinta do verde, sempre acompanhadas de texto | Hierarquia entre ação principal e secundária; o erro não depende só da cor |
| Componentes | Campo de texto (rótulo acima, campo, exemplo de formato), botão primário e secundário, cartão, menu lateral, selo "Novo colaborador", mensagens de erro e confirmação | Os mesmos componentes se repetem no login e no cadastro, mantendo o comportamento previsível |
| Feedback | Erros junto ao campo ou ao topo do formulário, em linguagem simples, mantendo o que o usuário digitou; confirmação explícita ao salvar; alerta antes de descartar dados | Visibilidade do estado do sistema e recuperação sem perda de trabalho (`RA` e `AL` do M02b) |

## Verificação de acessibilidade básica

Critérios da WCAG aplicados ao protótipo Web:

| Critério | Situação | Observação |
|---|---|---|
| Rótulos visíveis | Atende | Todos os campos têm rótulo fixo acima; o exemplo de formato não substitui o rótulo |
| Tamanho de alvo | Atende | Campos e botões têm altura próxima de 44 px |
| Contraste de texto | {{verificar}} | Conferir com um plugin de contraste (texto branco sobre o verde de ação; texto de apoio em cinza). Os exemplos de formato nos campos aparecem em cinza claro e podem ficar abaixo de 4,5:1 |
| Erro não depende só da cor | {{verificar}} | Garantir ícone e texto nas mensagens de erro dos estados `E` |
| Foco visível | {{a prototipar}} | Definir contorno de foco nos campos e botões |
| Navegação por teclado | {{a documentar}} | Ordem prevista: e-mail, senha, lembrar de mim, esqueci a senha, entrar |

Para produto Web, considere critérios pertinentes da WCAG vigente (por exemplo, contraste, foco, tamanho de alvo, texto alternativo e navegação por teclado quando aplicáveis). Para outras plataformas, use as recomendações adequadas ao contexto.

## Checklist

- [ ] Link do Figma está acessível.
- [ ] Há screenshots representativos no repositório.
- [ ] Todos os MoLIC relevantes estão cobertos.
- [ ] Estados de erro, feedback e recuperação foram prototipados.
- [ ] Terminologia/signos são consistentes com Entrega 9.
- [ ] Componentes equivalentes se comportam de forma consistente.
- [ ] Fluxos críticos são clicáveis do início ao fim.
- [ ] O protótipo está pronto para inspeção e testes, sem “links mortos” nas tarefas avaliadas.
- [ ] Dashboards, relatórios, históricos, filtros, administração e CRUDs presentes possuem justificativa rastreável.
- [ ] Estados de vazio, processamento, erro e recuperação foram considerados quando pertinentes.
- [ ] Resultados técnicos são apresentados de forma interpretável para o perfil de usuário.
- [ ] A equipe distingue no protótipo o que é interação simulada e o que é funcionalidade técnica realmente integrada, quando necessário.
