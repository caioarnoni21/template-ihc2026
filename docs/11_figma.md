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
**Autor:** Guilherme Matias RA: 22.122.071-8 <br>
**Protótipo:** https://www.figma.com/design/McbDfvqqGuDnR9uDmBdJrp/Login-e-Cadastro-de-Colaboradores?node-id=0-1&t=KVpUb4PCjVZbOSQ0-1 <br>
**Arquivo editável:** https://www.figma.com/design/McbDfvqqGuDnR9uDmBdJrp/Login-e-Cadastro-de-Colaboradores?node-id=0-1&t=KVpUb4PCjVZbOSQ0-1  <br>
**Última verificação de permissão:** {{22/11/2026}}

> Teste o link em janela anônima. O avaliador deve conseguir abrir o protótipo sem solicitar permissão.

## Cobertura MoLIC → Figma

| MoLIC | Objetivo | Fluxo/telas no Figma | Estados de erro/recuperação | Responsável |
|---|---|---|---|---|
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
