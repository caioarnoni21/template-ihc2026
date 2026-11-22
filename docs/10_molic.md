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

## M02 — Fazer a triagem rápida da equipe e registrar o encaminhamento

**Autor(a):** Guilherme Matias — 22.122.071-8  
**Cenário de interação de origem:** CI02, derivado de C02 (Entrega 4).  
**Objetivo(s):** O11 e seus desdobramentos O12 a O21, conforme a Entrega 9.  
**Tarefa(s) relacionada(s):** T02 — Fazer uma triagem rápida da equipe e registrar o encaminhamento (HTA, GOMS e CTT da Entrega 5).  
**Signos relevantes:** resumo da equipe; identificação discreta; colaborador; período analisado; período de referência; sinalização; limites da análise; dimensão alterada; explicação resumida; evidências de comunicação e de trabalho; termo de ajuda; última atualização; cobertura; estado da análise; lembrete de conversa humana; encaminhamento; justificativa; data de retomada; estado do registro; motivo da falha.

### Diagrama

<img width="1372" height="921" alt="image" src="https://github.com/user-attachments/assets/44eb8cd0-c7aa-4706-b578-fd19b5d6d8f9" />

**Fonte editável:** {{[link para o arquivo .drawi](https://drive.google.com/file/d/1HNhhZXRqECH_xcWImCJuT3qrnmmH3CRy/view?usp=sharing)}}

### Leitura do diagrama

Cenas têm o tópico no cabeçalho e diálogos/signos no corpo; `u:` identifica a fala do usuário, `d:` a do preposto e `d+u:` o diálogo. Quadrados pretos representam processamento do sistema; o círculo cheio indica abertura e o círculo duplo, encerramento. `gco` abre a conversa sobre o objetivo e `gcc` a fecha. Linhas tracejadas indicam retornos/recuperações. `PP` = prevenção passiva; `AL` = prevenção apoiada/alerta; `RA` = recuperação apoiada; `CE` = captura de erro sem recuperação dentro da própria interface.

#### Caminho principal (triagem completa)

1. **Abertura:** João abre o painel (`gco`: fazer a triagem da equipe). O sistema carrega as análises (processamento).
2. **Cena 1 — Leitura inicial da equipe (O12):** `d:` resumo da equipe, sinalização e identificação discreta (iniciais). João seleciona a sinalização.
3. **Cena 2 — Significado do sinal (O13, O16):** `d:` o que a sinalização significa e não significa (limites da análise). João decide aprofundar.
4. **Processamento:** o sistema verifica o estado da análise e, sendo confiável, segue.
5. **Cena 3 — Confiabilidade e variação (O14, O15):** `d:` períodos de referência e analisado, última atualização, cobertura, estado da análise, dimensão alterada e explicação resumida. João pode abrir os detalhes (Cena 4) ou um termo de ajuda (Cena 5) e voltar.
6. **Cena 6 — Contexto humano (O18):** `d:` lembrete de que o sinal não substitui a conversa com a pessoa. A conversa acontece fora do sistema.
7. **Cena 7 — Registro do encaminhamento (O19):** `u:` encaminhamento, justificativa e data de retomada. O sistema valida os campos.
8. **Cena 8 — Conferência do registro:** `d:` resumo do que será salvo. `u:` confirma. O sistema salva (processamento).
9. **Cena 9 — Registro concluído:** `d:` registro salvo. João volta à visão geral ou encerra (`gcc`).

**Caminho curto:** na Cena 2, se João decide **não aprofundar**, vai direto à Cena 7 (HTA 1 > 2 > 5; GOMS M1).

#### Alternativas e rupturas

| Situação | Onde ocorre | Como o usuário percebe | Caminho de recuperação/saída |
|---|---|---|---|
| Nenhuma situação a observar | Cena 1 | `d:` "Nenhuma situação a observar nos dados disponíveis" (só com análise completa, `PP`) | Encerra (`gcc`) sem registro |
| Análise sem dados, incompleta ou insuficiente | Processamento após a Cena 2 | Cena 3b: `d:` fonte ou período que falhou e "sem conclusão sobre mudança" (`PP`) | `u:` aguardar dados → Cena 7 com "aguardar dados" pré-selecionado; ou voltar à Cena 1 |
| Termo não compreendido | Cena 3 | Termo marcado com ajuda disponível (`PP`) | Cena 5 (termo de ajuda) e retorno tracejado à Cena 3 |
| Campo obrigatório vazio ou data inválida | Validação após a Cena 7 | `d:` indica o campo e preserva os demais dados (`RA`) | Retorno tracejado à Cena 7 |
| Encaminhamento incompatível com análise insuficiente | Cena 7 | `d:` alerta de que não há dados para sustentar essa escolha (`AL`) | Corrigir o encaminhamento ou manter "aguardar dados" |
| Revisão antes de confirmar | Cena 8 | O resumo mostra pessoa, período e encaminhamento | `u:` corrigir → retorno tracejado à Cena 7 |
| Falha ao salvar | Processamento após a Cena 8 | Cena 10: `d:` "não foi salvo; seu texto foi mantido" e o motivo da falha (`RA`) | Tentar novamente; corrigir o dado (Cena 7); ou deixar pendente e encerrar (`CE`) |
| Interrupção (supervisor chama) | Qualquer cena da 2 à 8 | Ao voltar: `d:` "Você estava vendo C. D., no período [datas], na etapa X" | Acesso ubíquo "retomar consulta" restaura a última cena (O20) |


### Cobertura dos objetivos (para a consolidação da equipe)

| Objetivo | Onde aparece no M02 |
|---|---|
| O11 Fazer a triagem e registrar | Abertura (`gco`) até Cena 9 (`gcc`) |
| O12 Leitura inicial | Cena 1 |
| O13 Decidir se aprofunda | Cena 2 (caminho curto e completo) |
| O14 Verificar confiabilidade | Cena 3 e processamento de estado |
| O15 Entender o que mudou | Cenas 3 e 4 |
| O16 Termos e significado do sinal | Cenas 2 e 5 |
| O17 Análise não confiável | Cena 3b |
| O18 Contexto humano | Cena 6 |
| O19 Registrar e conferir | Cenas 7, 8 e 9 |
| O20 Retomar após interrupção | Acesso ubíquo e restauração da sessão |
| O21 Recuperar falha de registro | Cena 10 |

### Estados/telas necessários para o Figma (a partir do M02)

- Visão geral com resumo e identificação discreta (Cena 1), com variações "situação a observar", "nenhuma situação" e "análise incompleta".
- Significado do sinal, com a escolha entre aprofundar e registrar (Cena 2).
- Confiabilidade e variação (Cena 3), com estado "análise não confiável" (Cena 3b).
- Detalhes por dimensão (Cena 4) e ajuda de termo (Cena 5).
- Lembrete de conversa humana (Cena 6).
- Registro com erros de campo e alerta de incompatibilidade (Cena 7).
- Conferência (Cena 8), confirmação (Cena 9) e falha ao salvar (Cena 10).
- Retomada após interrupção.

  
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

### Preparação para o Figma

Liste os estados/telas que serão necessários **a partir das conversas modeladas**, incluindo feedback, confirmação, erro e recuperação.

## Erros frequentes a evitar

- desenhar apenas caixas com nomes de telas e setas de navegação;
- não modelar falhas, cancelamento, volta ou recuperação;
- usar rótulos genéricos (“Tela 1”, “Processo 2”) sem tópico de conversa;
- criar no Figma fluxos que não existem no MoLIC;
- diagrama sem legenda/fonte editável e com texto ilegível.
