# Entrega 10 — MoLIC

**Data:** {{22/11/2026}}  
**Status:** 🟨 Em andamento
**Responsabilidade:** 1 solução completa por integrante

## Objetivo da atividade

Modelar a interação como uma **conversa entre usuário e preposto do designer**, oferecendo visão global dos caminhos que permitem ao usuário atingir seus objetivos — incluindo alternativas e rupturas relevantes. MoLIC não deve ser reduzida a um fluxograma de telas.

> Use a **notação MoLIC ensinada na disciplina**. Este template foca critérios de qualidade e não substitui a legenda/notação apresentada em aula.

## Atenção a TCCs sem interface original

O MoLIC não modela o algoritmo por dentro. Ele modela a **conversa de interação necessária para que uma pessoa use a contribuição**.

Exemplos de conversas:

- usuário escolhe dados/parâmetros → sistema valida → usuário inicia análise → sistema comunica processamento → usuário interpreta resultado;
- usuário consulta histórico → refina filtros → abre execução → compara com outra;
- administrador seleciona perfil → altera permissão → sistema comunica consequências → administrador confirma/cancela;
- analista recebe alerta → examina evidências → classifica ocorrência → registra decisão.

Modele também rupturas plausíveis: entrada inválida, falha de processamento, ausência de resultado, permissão insuficiente, filtro sem resultados, conflito de alteração, cancelamento ou necessidade de recuperação.

## M01 — {{nome do cenário/objetivo}}

**Autor(a):** Caio Arnoni - 22.221.019-7  
**Cenário de interação de origem:** CI01, derivado de C01/E4-C01.  
**Objetivo(s):** O01 e seus desdobramentos O02–O10, conforme a Entrega 9. 
**Tarefa(s) relacionada(s):** T01 — Consultar uma análise e registrar o próximo passo humano.
**Signos relevantes:** colaborador; período analisado; período de referência; padrão individual de referência; fontes; cobertura; última atualização; estado da análise; evidências de comunicação e de tarefas; sinalização; limites da análise; encaminhamento; justificativa; responsável pela retomada; data de retomada; estado do registro; motivo da falha.

### Diagrama

![MoLIC M01](../assets/10_molic/molic_m01.svg)

**Fonte editável:** {{adicione aqui o link para o arquivo `.drawio`, `.svg` editável ou outro formato utilizado pela equipe}}

### Leitura do diagrama

Explique em texto o caminho principal e pelo menos os caminhos alternativos/rupturas mais importantes.

cenas têm tópico no cabeçalho e diálogos/signos no corpo; `u:` identifica a fala do usuário, `d:` a do preposto e `d+u:` o diálogo. Quadrados pretos representam processamento do sistema; o círculo cheio indica abertura e o círculo duplo, encerramento. `gco` abre a conversa sobre o objetivo e `gcc` a fecha. Linhas tracejadas indicam retornos/recuperações. `PP` = prevenção passiva; `AL` = prevenção apoiada/alerta; `RA` = recuperação apoiada; `CE` = captura de erro sem recuperação dentro da própria interface.

#### Caminho principal

1. {{ponto de abertura → cena...}}
2. {{...}}

#### Alternativas e rupturas

| Situação | Onde ocorre | Como o usuário percebe | Caminho de recuperação/saída |
|---|---|---|---|
| {{dado inválido}} | {{...}} | {{fala/feedback}} | {{...}} |

## M02b — Acessar o sistema como gestor e cadastrar colaborador

**Autor(a):** Guilherme Matias — 22.122.071-8  
**Cenário de interação de origem:** CI02 (pré-condição de acesso) e T07 da Entrega 1 (cadastro de colaboradores).  
**Objetivo(s):** O22 (acessar o sistema como gestor), O23 (cadastrar e vincular colaborador) e O24 (recuperar acesso), a incluir na Entrega 9.  
**Signos relevantes:** e-mail do gestor; senha; nome; sobrenome; e-mail e telefone do colaborador; Telegram ID; Trello ID; vínculo do colaborador; estado da sessão.


### Diagrama

<img width="1372" height="921" alt="image" src="https://github.com/user-attachments/assets/44eb8cd0-c7aa-4706-b578-fd19b5d6d8f9" />

**Fonte editável:** https://drive.google.com/file/d/1HNhhZXRqECH_xcWImCJuT3qrnmmH3CRy/view?usp=sharing

#### Caminho principal

1. **Abertura:** `u:` URL do WorkSense (`gco`: acessar o sistema). **Cena "Identificar-se como gestor":** `d:` aviso de que o login é só para gestores; `d+u:` e-mail e senha.
2. **Processamento "validar credenciais".** Sendo válidas, `d:` acesso liberado leva à visão geral (cena 1 do M02), e a conversa de acesso se encerra (`gcc`).
3. **Cadastro:** pelo acesso ubíquo do menu lateral (`precond:` gestor autenticado; `gco`: cadastrar colaborador), João chega à **cena "Cadastrar colaborador"** e informa nome, sobrenome, e-mail, telefone, Telegram ID e Trello ID.
4. **Processamento "validar dados"**, depois **cena de confirmação do vínculo** (`AL`), depois **processamento "salvar cadastro"**, depois **cena "Colaborador cadastrado"**. Dali João cadastra outro ou conclui (`gcc`).

#### Alternativas e rupturas

| Situação | Onde ocorre | Como o usuário percebe | Caminho de recuperação/saída |
|---|---|---|---|
| E-mail ou senha incorretos | Validar credenciais | `d:` e-mail ou senha incorretos (`RA`) | Retorno tracejado ao login |
| Usuário sem perfil de gestor | Validar credenciais | `d:` acesso permitido apenas a gestores (`RA`) | Retorno tracejado ao login |
| Esqueceu a senha | Login | `u:` esqueci minha senha | Cena "Recuperar acesso"; e-mail inválido volta a ela (`RA`); `u:` voltar ao login |
| Campo vazio ou formato inválido | Validar dados | `d:` indica o campo e mantém os demais (`RA`) | Retorno tracejado ao cadastro |
| Telegram ID ou Trello ID já vinculado | Validar dados | `d:` ID já vinculado a outro colaborador (`RA`) | Corrigir o ID no cadastro |
| Vínculo digitado errado | Confirmação do vínculo | `d:` nome, Telegram ID e Trello ID para conferir (`AL`) | `u:` corrigir (retorno ao cadastro) ou `u:` confirmar |
| Erro ao salvar | Salvar cadastro | `d:` erro ao salvar; dados mantidos (`RA`) | Retorno tracejado ao cadastro |
| Sair com dados não gravados | Acesso ubíquo "sair" | `d:` há alterações não gravadas (`AL`) | `u:` sair sem salvar ou `u:` não sair |


  
### Checklist específico de modelagem

- [ ] Existe **ponto de abertura** coerente com o início do objetivo.
- [ ] As **cenas de conversa** representam tópicos/assuntos, não nomes de páginas apenas.
- [ ] As transições/falas deixam claro o que o usuário ou o sistema comunica.
- [ ] Há **ponto(s) de encerramento** para objetivos concluídos/abandonados quando aplicável.
- [ ] Processamentos do sistema estão representados conforme a notação adotada em aula, sem “inventar” fala do usuário.
- [ ] Rupturas (breakdowns) relevantes têm feedback e caminho de recuperação, não becos sem saída.
- [ ] Acessos ubíquos/atalhos só aparecem quando semanticamente justificáveis.
- [ ] O diagrama cobre caminhos alternativos importantes, e não apenas o “happy path”.
- [ ] Nomes de objetivos, tópicos e signos são coerentes com a Entrega 9.
- [ ] O diagrama é legível em tamanho normal no GitHub.
- [ ] O MoLIC representa a conversa usuário–sistema, não o fluxo interno do algoritmo.
- [ ] Processamento, filtros, administração, relatórios e históricos incluem retornos/rupturas quando relevantes.

> Repita M02, M03... para todos os integrantes.

## Consolidação da equipe

### Cobertura dos objetivos

| Objetivo | MoLIC que cobre | Lacunas/duplicidades | Decisão |
|---|---|---|---|
| O01 | M01 | {{...}} | {{...}} |
| O11 Fazer a triagem da equipe e registrar o encaminhamento | M02: abertura (`gco`) até os três `gcc` | Duplica o O01 (mesma meta; muda a persona e a tarefa) | Unificar com o O01 no mapa consolidado, mantendo M01 e M02 como variantes: o M02 tem o caminho curto |
| O12 Obter a leitura inicial da equipe em linguagem simples | M02: Cena 1 | Parcial com o O02; o M02 parte do resumo da equipe, e o M01 parte da escolha de colaborador e período | Manter, como alternativa de entrada do O02 |
| O13 Decidir se vale aprofundar | M02: Cena 2 (caminho curto e completo) | Sem equivalente no M01, porque o Rafael sempre aprofunda | Manter; é exclusivo do P02 |
| O14 Verificar a confiabilidade da análise | M02: processamento de estado e Cena 3 | Equivale ao O06, e o O14 acrescenta o estado da análise | Unificar em um nome só (O06) |
| O15 Entender o que mudou em cada dimensão | M02: Cenas 3 e 4 | Equivale ao O07 | Unificar no O07 |
| O16 Consultar o significado dos termos e do sinal | M02: Cenas 2 e 5 | Parcial com o O03; a ajuda de termos (lacuna ?03) só existe no M02 | Manter e sugerir ao Caio incluir ajuda de termos |
| O17 Reconhecer análise não confiável e aguardar dados | M02: Cena 3b | Equivale ao O08; no M02 só se permite "aguardar dados" | Unificar no O08 |
| O18 Considerar o contexto humano antes de agir | M02: Cena 6 | Relacionado ao O04; a cena só tem fala `d:`, pois a conversa ocorre fora do sistema | Manter ligado ao O04 ou fundir com ele |
| O19 Registrar e conferir o encaminhamento | M02: Cenas 7, 8 e 9 | Equivale ao O05; o M02 não tem "responsável pela retomada" | Unificar no O05 e decidir se o campo "responsável" entra no M02 |
| O20 Retomar a consulta após interrupção | M02: acesso ubíquo "retomar consulta" | Equivale ao O09, sem lacuna aparente | Unificar no O09 |
| O21 Recuperar uma falha de registro | M02: Cena 10 | Equivale ao O10; o M02 acrescenta "deixar pendente" (`CE`) | Unificar no O10 |
| O22 Acessar o sistema como gestor | M02b: login e validação | Ainda não está na Entrega 9; confirmar se a Tainá modela o login | Incluir na Entrega 9 |
| O23 Cadastrar e vincular colaborador | M02b: cadastro, confirmação e conclusão | Ainda não está na Entrega 9 | Incluir na Entrega 9 |
| O24 Recuperar acesso | M02b: "Recuperar acesso" | Ainda não está na Entrega 9 | Incluir na Entrega 9, ou cortar a cena se o professor achar fora de escopo |

### Preparação para o Figma

Liste os estados/telas que serão necessários **a partir das conversas modeladas**, incluindo feedback, confirmação, erro e recuperação.

## Erros frequentes a evitar

- desenhar apenas caixas com nomes de telas e setas de navegação;
- não modelar falhas, cancelamento, volta ou recuperação;
- usar rótulos genéricos (“Tela 1”, “Processo 2”) sem tópico de conversa;
- criar no Figma fluxos que não existem no MoLIC;
- diagrama sem legenda/fonte editável e com texto ilegível.
