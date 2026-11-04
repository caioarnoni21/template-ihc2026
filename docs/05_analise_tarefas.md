# Entrega 5 — Análise de tarefas: HTA, GOMS e CTT

**Data:** {{21/10/2026}}  
**Status:** 🟨 iniciada  
**Responsabilidade:** cada integrante modela pelo menos 1 HTA, 1 GOMS e 1 CTT. As três técnicas podem abordar a mesma funcionalidade ou funcionalidades distintas, conforme a orientação da disciplina.

## Objetivo da atividade

Modelar tarefas importantes sob perspectivas complementares: decomposição hierárquica (HTA), estrutura de metas/métodos/operações (GOMS) e relações temporais entre tarefas (CTT). O diagrama deve ser acompanhado de interpretação textual.

## Para projetos cujo TCC não previa interface

Modele **tarefas humanas relacionadas ao uso da contribuição técnica**, e não a implementação interna do algoritmo. Exemplos de boas tarefas para análise:

- investigar uma consulta de baixo desempenho;
- configurar uma análise e selecionar parâmetros;
- submeter um dataset e verificar sua validade;
- acompanhar uma execução demorada;
- comparar dois resultados/modelos;
- interpretar uma recomendação e decidir se a aceita;
- localizar uma execução anterior usando busca/filtros;
- gerar e compartilhar um relatório;
- administrar papéis/permissões quando isso for parte do trabalho real;
- revisar um alerta e registrar uma decisão.

Um CRUD pode gerar tarefas relevantes, mas “cadastrar usuário” só merece modelagem se tiver significado no domínio (papéis, validações, riscos, permissões, dependências).

## Seleção das tarefas

| ID | Tarefa | Persona/cenário de origem | Frequência/criticidade | Autor responsável |
|---|---|---|---|---|
| T01 | Consultar uma análise e registrar o próximo passo humano | Rafael Costa (P01) / E4-C01 | Revisão periódica ou sob demanda; alta | Caio Arnoni |

> Priorize tarefas necessárias para que o usuário alcance objetivos centrais. Não desperdice a modelagem em ações triviais isoladas, como “clicar em login”, se o objetivo relevante é maior. Da mesma forma, não modele o funcionamento interno do algoritmo como se fosse uma tarefa humana.

---

## HTA — T01 Consultar uma análise e registrar próximo passo

**Autor(a):** Caio Arnoni - 22.221.019-7

### Descrição da tarefa

- **Objetivo:** compreender os limites das evidências de um caso e registrar um próximo passo justificado. <br>
- **Ponto de início:** Rafael tem uma questão sobre um colaborador e acesso autorizado à equipe. O caso é identificável e há um registro de análise, mesmo que incompleto. <br>
- **Conclusão esperada:** encaminhamento persistido e conferido, com justificativa e responsável pela retomada. Um registro de insuficiência é um resultado válido da tarefa, não uma análise conclusiva da pessoa. <br>
- **Contexto:** consulta no computador, com possibilidade de interrupção; rotina ainda hipotética. <br>


### Diagrama

<img width="1320" height="605" alt="image" src="https://github.com/user-attachments/assets/a158f4f4-dcf1-405d-8be2-b96176fa562a" />


### Decomposição e planos

| ID | Objetivo/operação | Plano/ordem | Problema ou decisão de design observada |
|---|---|---|---|
| 0 | Consultar uma análise e registrar próximo passo | 1 > 2 > 3 | Registro concluído não equivale a resolver a situação da pessoa |
| 1 | Localizar a análise | 1.1 / 1.2: escolher conforme visibilidade do caso/período | Evitar abrir caso homônimo ou período errado |
| 1.1 | Selecionar caso e período em lista disponível | Operação terminal; usar se ambos estiverem visíveis | Identidade e período devem ser conferíveis |
| 1.2 | Buscar por identificador e selecionar caso/período | Operação terminal neste nível; usar se não estiverem visíveis | Refinar o identificador se os resultados forem ambíguos |
| 2 | Avaliar as evidências | 2.1 > 2.2 > 2.3 com evidência suficiente; 2.1 > 2.3 se insuficiente | Ausência de dados não significa estabilidade |
| 2.1 | Conferir identidade, período, cobertura e atualização | Operação terminal | Primeiro verificar se a comparação é pertinente e possível |
| 2.2 | Comparar comunicação e tarefas com o histórico do próprio perfil | Operação terminal, condicional à suficiência | Não confundir alteração comunicacional com piora das entregas |
| 2.3 | Definir próximo passo ou registrar insuficiência | Operação terminal | Resultado humano: conversar, acompanhar ou manter pendência; sem diagnóstico |
| 3 | Registrar próximo passo | 3.1 > 3.2; repetir após correção se o registro falhar | Não considerar envio como prova de persistência |
| 3.1 | Informar decisão, justificativa e responsável pela retomada | Operação terminal | Registrar apenas o contexto necessário; data de retomada quando aplicável |
| 3.2 | Conferir confirmação de registro persistido | Operação terminal | Conferir caso, período e conteúdo, além da mensagem de confirmação |

**Verificação do HTA:**

- O objetivo 0 representa uma meta do usuário? Sim. Consultar uma análise e registrar um próximo passo corresponde à necessidade de Rafael de compreender uma situação da equipe e decidir um acompanhamento humano.<br>
- As subtarefas são necessárias e suficientes? Sim, para o recorte proposto: localizar a análise, avaliar as evidências e registrar o encaminhamento. Elas incluem verificar a qualidade dos dados e confirmar o registro. Realizar a conversa e resolver a situação do colaborador estão fora dessa tarefa.<br>
- Os **planos** indicam ordem, alternativa, repetição ou condição? Sim. O plano principal segue 1 > 2 > 3. A localização utiliza 1.1 ou 1.2, conforme o caso esteja visível na lista ou exija busca. A comparação em 2.2 ocorre apenas com dados suficientes; caso contrário, Rafael segue para 2.3, registrando a limitação. Se o registro falhar, repete 3.1 > 3.2 após a correção; se a falha persistir, mantém a pendência explícita.<br>
- A decomposição parou em nível útil para projeto de interação? Sim. As operações finais, como selecionar um caso, conferir a cobertura e registrar uma justificativa, ajudam a definir informações, controles e respostas da interface. Não é necessário decompor cada clique nem representar o funcionamento interno do algoritmo.

---

## GOMS — T01 Consultar uma análise e registrar o próximo passo humano.

**Autor(a):** Caio Arnoni - 22.221.019-7

### Goals: metas e subobjetivos

- **G0:** consultar a análise correta e registrar um próximo passo humano justificado.
- **G1:** localizar o caso e o período corretos.
- **G2:** avaliar as evidências e definir o próximo passo.
- **G3:** registrar e conferir o encaminhamento.

### Métodos, operadores e regras de seleção

- **Method M1:** Seleção pela lista disponível
  - Ler identificador e período;
  - Selecionar o caso;
  - Conferir o caso e o período abertos;
- **Method M2:** Busca pelo identificador
  - Focalizar busca;
  - Digitar identificador;
  - Executar busca;
  - Ler resultados;
  - Selecionar caso/período;
  - Conferir correspondência;
- **Selection Rule SR1:** usar M1 se o caso e o período desejados já estão visíveis e identificáveis.
- **Selection Rule SR2:** usar se o caso ou período não está visível e Rafael conhece o identificador. 

> Não chame qualquer passo de “método”. Em GOMS, métodos são sequências alternativas capazes de atingir uma meta; regras de seleção explicam quando escolher entre eles.

---

## CTT — T01 Consultar uma análise e registrar o próximo passo humano

**Autor(a):** Caio Arnoni - 22.221.019-7

### Descrição

Rafael Costa, gestor de equipe, localiza o colaborador e o período desejados pela lista disponível ou pela busca. O sistema disponibiliza os dados da análise e informa sua cobertura. Rafael avalia as evidências e define um próximo passo, como conversar com o colaborador, acompanhar a situação ou solicitar esclarecimentos quando os dados forem insuficientes. Em seguida, informa sua decisão e justificativa, o sistema grava o encaminhamento e Rafael confere a confirmação. A tarefa termina com o registro confirmado, mantendo a interpretação e a decisão sob responsabilidade humana.

### Diagrama

<img width="1628" height="708" alt="image" src="https://github.com/user-attachments/assets/05257caa-4155-41cf-811c-923736391e6d" />


### Legenda e relações temporais usadas

| Operador/relação | Significado no diagrama | Exemplo no modelo |
|---|---|---|
| `[]` | Escolha exclusiva: ao iniciar uma alternativa, a outra não é executada naquela escolha | Selecionar pela lista ou buscar e selecionar |
| `[]>>` | Habilitação com passagem de informação: a tarefa seguinte começa após a anterior e recebe seu resultado | O caso/período selecionado orienta a recuperação; os dados orientam a avaliação; o encaminhamento é passado para registro |

### Tipos de tarefa

| Símbolo | Tipo | Exemplo no diagrama |
|---|---|---|
| [A] | Abstrata: composição de outras tarefas | Localizar caso/período; registrar encaminhamento |
| [I] | Interação: diálogo entre pessoa e sistema | Selecionar caso; informar decisão; consultar confirmação |
| [S] | Sistema: execução automática sem intervenção durante o processamento | Disponibilizar dados; persistir encaminhamento |
| [U] | Usuário: atividade humana fora do diálogo com a interface | Rafael interpretar a evidência e definir o próximo passo |

Identifique, quando aplicável, tarefas de usuário, sistema, interação e tarefas abstratas. Verifique se concorrência, escolha, habilitação, desabilitação e repetição estão representadas corretamente segundo a notação adotada em aula.

---

## HTA — T02  Realizar triagem rápida da equipe e registrar o encaminhamento

**Autor(a):** Guilherme Matias — 22.122.071-8

### Descrição da tarefa

* Objetivo: consultar o painel entre duas reuniões, obter uma resposta simples sobre “preciso me preocupar ou não?”, decidir se vale aprofundar, confirmar com contexto humano quando necessário e registrar o encaminhamento com justificativa.
* Ponto de início: João Pedro abre o painel do WorkSense, com cerca de 15 minutos disponíveis, antes de uma reunião individual.
* Conclusão esperada: o encaminhamento (apoiar, acompanhar, não intervir ou aguardar dados) fica registrado com uma justificativa em linguagem natural, sem diagnóstico nem veredito automático.
* Contexto: notebook em sala compartilhada ou home office, com pressa, possíveis interrupções e outras pessoas por perto (H). O gestor tem pouca familiaridade com métricas.

### Diagrama

<img width="1767" height="658" alt="image" src="https://github.com/user-attachments/assets/a6062efc-e212-4faa-b478-185efad21484" />


### Decomposição e planos

| ID | Objetivo/operação | Plano/ordem | Problema ou decisão de design observada |
|---|---|---|---|
| 0 | Realizar triagem rápida da equipe e registrar o encaminhamento |Plano 0: executar 1 > 2. Se 2.2 = não aprofundar, executar 5. Se 2.2 = aprofundar, executar 3 > 4 > 5. Se 3.1 indicar “sem dados”, “incompleta” ou “insuficiente”, executar 3 > 5 (registrar “aguardar dados”)| Sem o desvio por estado da análise, o gestor agiria sobre uma análise que não existe. A tarefa precisa caber em cerca de 15 minutos |
| 1 | Obter a leitura inicial da equipe |Plano 1: executar 1.1 > 1.2| A primeira tela deve responder em linguagem simples, sem jargão técnico (RC08) |
|1.1| Abrir o painel |Operação única: acessar o painel pelo notebook| Privacidade visual: não exibir nomes e termos sensíveis de imediato, pois há pessoas por perto|
|1.2| Ler o resumo e identificar se há colaborador com sinalização |Leitura do resumo na primeira camada de informação| Poucos indicadores na visão inicial, sem ranking nem rótulos como “em risco” (RC11) |
| 2 | Decidir se vale aprofundar |Plano 2: executar 2.1 > 2.2| O aprofundamento deve ser opcional, nunca obrigatório para decidir (RC09) |
|2.1| Ler o que o sinal significa e o que não significa |Leitura de um texto curto exibido junto da sinalização|Deixar claro que não é diagnóstico nem veredito automático |
|2.2| Decidir entre aprofundar ou não |Decisão cognitiva do gestor, com base na gravidade percebida| Se não aprofundar, o caminho curto leva direto ao registro (5) |
| 4 | Confirmar com contexto humano |Plano 4: executar 4.1 > 4.2| A ferramenta não decide; reforçar a conversa humana antes de qualquer ação|
|4.1| Recordar o contexto externo à ferramenta |Recuperação da memória (picos de demanda, troca de turnos, combinados da equipe)| Esse contexto não está nos registros e depende de memória ou do supervisor (C02.Q3) |
|4.2| Conversar com o colaborador e decidir o encaminhamento |Conversa fora da ferramenta, seguida da decisão| Etapa externa ao sistema por escolha de projeto; o sistema não deve induzir a decisão|
| 5 | Registrar a decisão e a justificativa |Plano 5: executar 5.1 > 5.2| O gestor precisa de respaldo documentado, sem diagnóstico (RC14)|
|5.1| Escolher o encaminhamento |Selecionar entre apoiar, acompanhar, não intervir ou aguardar dados|Opções claras e neutras, sem punição automática|
|5.2| Escrever a justificativa e confirmar o registro |Digitar texto livre curto e clicar em confirmar| Registro mínimo para não expor a pessoa; exibir confirmação e preservar o contexto em caso de interrupção|

**Verificação do HTA:**

* O objetivo 0 representa uma meta do usuário? Sim. É a meta real do João Pedro: saber rapidamente se há algo a observar e deixar a decisão registrada com segurança.
* As subtarefas são necessárias e suficientes? Sim. Cobrem da leitura inicial ao registro final, incluindo a verificação de confiabilidade e o contexto humano, que são as maiores preocupações da persona.
* Os planos indicam ordem, alternativa, repetição ou condição? Sim. Há sequência (1 > 2), alternativa (aprofundar ou não), condição (estado da análise em 3.1) e opcionalidade (3.3).
* A decomposição parou em nível útil para projeto de interação? Sim. Parou no nível de leitura, clique e digitação, que é adequado para o protótipo.

---

## GOMS — T02 Realizar triagem rápida da equipe e registrar o encaminhamento

**Autor(a):** Guilherme Matias — 22.122.071-8

### Goal

`G0: Decidir se há algo a observar na equipe e registrar o encaminhamento com justificativa, em cerca de 15 minutos entre reuniões.`

### Métodos, operadores e regras de seleção

- **Method M1 — Triagem curta (não aprofundar):** caminho mais rápido, para quando a leitura inicial basta.
  * 1 Abrir o painel, por iniciativa própria ou por notificação discreta (HTA 1.1).
  * 2 Ler o resumo e identificar se há colaborador com sinalização (HTA 1.2).
  * 3 Ler o que o sinal significa e não significa (HTA 2.1).
  * 4 Decidir não aprofundar (HTA 2.2).
  * 5 Escolher o encaminhamento "acompanhar" ou "não intervir" e confirmar com justificativa curta (HTA 5.1 e 5.2).
  * - Operators: apontar, clicar, perceber, ler, decidir, digitar.

- **Method M2 — Triagem completa (aprofundar e confirmar com contexto humano):**
  * 1 Executar os passos 1 a 3 de M1, decidindo aprofundar em HTA 2.2.
  * 2 Conferir períodos de referência e reanálise, atualização e estado da análise (HTA 3.1).
  * 3 Ler a explicação resumida da variação, indicando qual eixo mudou (HTA 3.2).
  * 4 Consultar componentes ou ajuda, apenas se a explicação resumida não bastar (HTA 3.3, opcional).
  * 5 Recordar o contexto externo: pico de demanda, troca de turnos, combinados da equipe (HTA 4.1).
  * 6 Conversar com o colaborador, fora da ferramenta, e decidir o encaminhamento (HTA 4.2).
  * 7 Escolher o encaminhamento (apoiar, acompanhar ou não intervir) (HTA 5.1).
  * 8 Digitar a justificativa em linguagem natural, confirmar e perceber a confirmação (HTA 5.2).
  * - Operators: apontar, clicar, perceber, ler, decidir, recordar, falar, ouvir, digitar.

- **Method M3 — Aguardar dados (análise não confiável):**
  1. Executar os passos 1 a 3 de M1, decidindo aprofundar em HTA 2.2.
  2. Conferir o estado da análise e identificar "sem dados", "incompleta" ou "evidência insuficiente" (HTA 3.1).
  3. Escolher o encaminhamento "aguardar dados" (HTA 5.1).
  4. Confirmar com justificativa curta ou predefinida e perceber a confirmação (HTA 5.2).
  - Operators: apontar, clicar, perceber, ler, decidir.

- **Method M4 — Retomar após interrupção:**
  * 1 Reabrir o painel.
  * 2 Perceber que o colaborador e a etapa foram preservados.
  * 3 Continuar a partir da etapa em que parou, seguindo M1, M2 ou M3.
  * - Operators: clicar, perceber, decidir.

- **Selection Rule SR1:** usar M1 quando não houver sinalização ou quando, depois de ler o significado do sinal, João considerar a variação pequena e a leitura simples suficiente; usar M2 quando a sinalização parecer relevante ou quando ele não entender o que o texto diz.
- **Selection Rule SR2:** durante M2, se o estado da análise em HTA 3.1 for "sem dados", "incompleta" ou "evidência insuficiente", abandonar M2 e passar para M3, sem conversar com o colaborador com base em dado não confiável.
- **Selection Rule SR3:** dentro de M2, consultar componentes ou ajuda (HTA 3.3) somente quando a explicação resumida não bastar ou quando ele não reconhecer um termo; caso contrário, seguir direto para HTA 4.1.
- **Selection Rule SR4:** no registro (HTA 5.2), digitar justificativa completa quando o encaminhamento for "apoiar" ou "acompanhar" após conversa, porque ele precisa de respaldo documentado; usar justificativa curta ou predefinida quando for "não intervir" ou "aguardar dados", ou quando estiver sem tempo.
- **Selection Rule SR5:** usar M4 sempre que houver interrupção (por exemplo, um supervisor chamando para resolver uma escala) entre HTA 2.1 e HTA 5.2; sem preservação de contexto, João recomeça de HTA 1.1.

> Não chame qualquer passo de “método”. Em GOMS, métodos são sequências alternativas capazes de atingir uma meta; regras de seleção explicam quando escolher entre eles.

---

## CTT — T02 Realizar triagem rápida da equipe e registrar o encaminhamento

**Autor(a):** Guilherme Matias — 22.122.071-8

### Descrição
O CTT modela as relações temporais entre as ações do João Pedro e as respostas do WorkSense na triagem entre reuniões. Ele mostra:
* a sequência obrigatória (leitura inicial, decisão, registro);
* o aprofundamento opcional;
* a escolha entre análise confiável e análise sem dados suficientes;
* a interrupção, que suspende a triagem e permite retomá-la do ponto em que parou.

### Diagrama

<img width="2788" height="1296" alt="image" src="https://github.com/user-attachments/assets/d57a027c-f910-417d-ae88-26422c151ab7" />



### Legenda e relações temporais usadas

| Operador/relação | Significado no diagrama | Exemplo no modelo |
|---|---|---|
| `>>` (Habilitação) | A conclusão de uma tarefa habilita o início da seguinte. | Abrir painel >> Exibir resumo >> Ler resumo e identificar sinalização |
| `[]` (Escolha) | Apenas uma das alternativas é executada. | Análise confiável `[]` Análise não confiável (A7 `[]` A8) |
| `[ ]` (Opcional) | A tarefa pode ser omitida sem comprometer a meta. | Aprofundar e confirmar (A4); Consultar componentes ou ajuda (I2) |
| `\|>` (Suspensão/retomada) | Uma tarefa interrompe a principal, que é retomada do ponto em que parou. | Executar triagem (A1) `\|>` Tratar interrupção (A6) |

| Tipo de tarefa | Representação | Exemplos |
|---|---|---|
| Abstrata (A) | Caixa com borda grossa | A0 a A8 |
| Usuário (U) | Caixa branca, borda fina | U1 Ler resumo; U3 Decidir aprofundar ou não; U7 Conversar com o colaborador |
| Sistema (S) | Caixa cinza | S1 Exibir resumo da equipe; S3 Exibir estado, períodos e atualização; S4 Salvar e exibir confirmação |
| Interação (I) | Caixa azul clara | I1 Abrir painel; I3 Escolher encaminhamento; I4 Digitar justificativa |

Identifique, quando aplicável, tarefas de usuário, sistema, interação e tarefas abstratas. Verifique se concorrência, escolha, habilitação, desabilitação e repetição estão representadas corretamente segundo a notação adotada em aula.

---

## Síntese da equipe

Quais problemas de interação, oportunidades e requisitos apareceram a partir das modelagens? Quais tarefas irão para o protótipo e para o teste de usabilidade?

## Checklist

- [ ] Cada integrante produziu ao menos 1 HTA, 1 GOMS e 1 CTT.
- [ ] Cada artefato identifica autor e tarefa.
- [ ] Diagramas são legíveis e possuem fonte editável quando possível.
- [ ] HTA contém planos, não apenas árvore de tópicos.
- [ ] GOMS distingue Goals, Operators, Methods e Selection Rules.
- [ ] CTT usa operadores temporais e tipos de tarefa coerentes.
- [ ] Há texto explicando cada diagrama.
- [ ] Tarefas estão ligadas a cenários/personas na rastreabilidade.
- [ ] Em TCC técnico, as tarefas descrevem o que a pessoa faz com a contribuição/resultados, não passos internos do código.
- [ ] CRUDs, relatórios, filtros e atividades administrativas foram escolhidos por relevância ao objetivo do usuário.
