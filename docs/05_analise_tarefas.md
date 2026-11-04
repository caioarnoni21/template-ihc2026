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
| T01 | {{...}} | {{P01/C01}} | {{...}} | {{...}} |

> Priorize tarefas necessárias para que o usuário alcance objetivos centrais. Não desperdice a modelagem em ações triviais isoladas, como “clicar em login”, se o objetivo relevante é maior. Da mesma forma, não modele o funcionamento interno do algoritmo como se fosse uma tarefa humana.

---

## HTA — T01 {{nome da tarefa}}

**Autor(a):** {{nome — matrícula}}

### Descrição da tarefa

{{objetivo, ponto de início, conclusão esperada, contexto}}

### Diagrama

![HTA T01](../assets/05_tarefas/hta_t01.svg)

### Decomposição e planos

| ID | Objetivo/operação | Plano/ordem | Problema ou decisão de design observada |
|---|---|---|---|
| 0 | {{objetivo principal}} | {{1 }} 2 > 3 / 1 ou 2 etc.> | {{...}} |

**Verificação do HTA:**

- O objetivo 0 representa uma meta do usuário?
- As subtarefas são necessárias e suficientes?
- Os **planos** indicam ordem, alternativa, repetição ou condição?
- A decomposição parou em nível útil para projeto de interação?

---

## GOMS — T02 {{nome da tarefa}}

**Autor(a):** {{nome — matrícula}}

### Goal

`G0: {{meta do usuário}}`

### Métodos, operadores e regras de seleção

- **Method M1:** {{...}}
  - Operators: {{perceber, apontar, clicar, digitar, decidir... conforme o nível adotado}}
- **Method M2:** {{...}}
  - Operators: {{...}}
- **Selection Rule SR1:** usar M1 quando {{condição}}; usar M2 quando {{condição}}.

> Não chame qualquer passo de “método”. Em GOMS, métodos são sequências alternativas capazes de atingir uma meta; regras de seleção explicam quando escolher entre eles.

---

## CTT — T03 {{nome da tarefa}}

**Autor(a):** {{nome — matrícula}}

### Descrição

{{...}}

### Diagrama

![CTT T03](../assets/05_tarefas/ctt_t03.svg)

### Legenda e relações temporais usadas

| Operador/relação | Significado no diagrama | Exemplo no modelo |
|---|---|---|
| {{...}} | {{...}} | {{...}} |

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

![HTA T01](../assets/05_tarefas/hta_t01.svg)

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

## GOMS — T02 {{nome da tarefa}}

**Autor(a):** {{nome — matrícula}}

### Goal

`G0: {{meta do usuário}}`

### Métodos, operadores e regras de seleção

- **Method M1:** {{...}}
  - Operators: {{perceber, apontar, clicar, digitar, decidir... conforme o nível adotado}}
- **Method M2:** {{...}}
  - Operators: {{...}}
- **Selection Rule SR1:** usar M1 quando {{condição}}; usar M2 quando {{condição}}.

> Não chame qualquer passo de “método”. Em GOMS, métodos são sequências alternativas capazes de atingir uma meta; regras de seleção explicam quando escolher entre eles.

---

## CTT — T03 {{nome da tarefa}}

**Autor(a):** {{nome — matrícula}}

### Descrição

{{...}}

### Diagrama

![CTT T03](../assets/05_tarefas/ctt_t03.svg)

### Legenda e relações temporais usadas

| Operador/relação | Significado no diagrama | Exemplo no modelo |
|---|---|---|
| {{...}} | {{...}} | {{...}} |

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
