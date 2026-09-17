# Entrega 3 — Personas, mapa de empatia, contexto de uso e jornada

**Data:** {{11/09/2026}}  
**Status:** 🟨 em andamento
**Responsabilidade:** 1 persona por integrante; 1 mapa de empatia, 1 contexto de uso consolidado e 1 jornada por equipe (salvo orientação diferente do docente).

## Objetivo da atividade

Representar grupos de usuários de forma útil para decisões de design. Persona não é personagem decorativo: suas características devem alterar requisitos, prioridades, linguagem, fluxos ou critérios de avaliação.

## Atenção a projetos técnicos

Em TCCs sem interface original, a persona pode representar um **profissional que se apropria da contribuição técnica**: DBA, analista, cientista de dados, administrador, pesquisador, técnico, operador, gestor ou especialista de domínio.

Não escolha um perfil apenas porque “parece combinar” com a tecnologia. Explique **qual objetivo esse perfil teria e qual parte da contribuição do TCC produziria valor para ele**. Se ainda for hipótese, mantenha como hipótese/proto-persona a validar.

Também considere papéis diferentes quando houver tarefas distintas, por exemplo:

- operador que executa análises;
- administrador que configura e gerencia permissões;
- especialista que interpreta resultados;
- gestor que consulta relatórios e decide;
- auditor que revisa histórico.

## Entradas da Entrega 1

Antes de criar personas, retome os tipos de usuários, características relevantes, objetivos e hipóteses registradas na Entrega 1. A persona **não deve transformar uma hipótese inicial em fato por meio de uma história fictícia**.

| Item da Entrega 1 | Status inicial | Evidência disponível agora | Como será tratado nesta entrega |
|---|---|---|---|
| H01 - Gestor como usuário prioritário | H | A Entrega 1 propõe acompanhamento gerencial; o foco no gestor foi mantido pela equipe | Incorporar em P01, preservando a necessidade de pesquisa com gestores |
| H02 - Transparência e participação dos colaboradores | H | O PDF descreve expectativas fictícias de interpretação cautelosa; não há pesquisa com colaboradores reais | Incorporar em P03 como hipótese, incluindo explicação do uso dos dados e contextualização |
| H03 - RH como apoio e governança | H | As entregas anteriores mencionam esse papel, sem comprovar frequência de uso | Manter H03; propor P02 como segunda primária e registrar H09 sobre uso recorrente |
| H04 - Administração técnica distinta da gestão | H | Separação de responsabilidades proposta na Entrega 1 | Não criar uma quarta persona; manter integrações e permissões técnicas fora das jornadas principais |
| H05 - Eixos separados, componentes e limitações | H | O desenho experimental separa os eixos; o benefício de interface não foi testado | Apresentar comparações explicáveis em P01 e P02; testar compreensão |
| H06 - Revisão periódica como entrada principal | H | Não há levantamento real da rotina | Propor revisão periódica em P01 e P02, sem afirmar que a frequência foi validada |
| H07 - Distinguir estabilidade e problemas de dados | H | Os perfis sintéticos permitem exercitar estabilidade e mudanças, mas não cobrem todos os erros | Incluir estados de ausência, incompletude e baixa evidência nas futuras tarefas |
| H08 - Computador como dispositivo principal | H | Nenhuma pesquisa contextual fornecida | Usar computador como hipótese de P01/P02 e acesso responsivo em P03 |

## 1. Personas

### Persona P01 — Rafael Costa

**Autor(a):** Caio Arnoni - 22.221.019-7  
**Tipo:** primária
**Base de evidências:**  proto-persona a validar <br>
**Hipóteses da Entrega 1 relacionadas:** H01, H04, H05, H06, H07 e H08.

![Persona P01](../assets/03_personas/persona_p01.svg)

| Campo | Descrição |
|---|---|
| Faixa etária / contexto relevante | 30 anos. Lidera uma equipe distribuída e concilia acompanhamento de pessoas com entregas de projeto (H). |
| Ocupação/papel | Gestor responsável por prioridades, acompanhamento de tarefas e conversas de apoio com sua equipe (H). |
| Conhecimento do domínio | Conhece desenvolvimento e gestão de tarefas; não é especialista em PLN nem em interpretação estatística de modelos (H). |
| Experiência tecnológica | Usa quadros de tarefas, chat e relatórios; consegue interpretar gráficos simples quando há período, legenda e definição (H). |
| Objetivos | Identificar situações que merecem conversa, entender o que mudou e combinar ações de apoio sem julgar alguém apenas por um indicador (H). |
| Necessidades | Comparar períodos da mesma pessoa; separar comunicação e atividade profissional; verificar cobertura e atualização; recuperar o contexto de acompanhamentos anteriores (H). |
| Dores/frustrações | Informações dispersas entre tarefas e conversas; dificuldade para distinguir mudança persistente de episódio pontual; receio de interpretar sinais fora de contexto (H). |
| Motivadores | Ajudar a equipe, organizar o trabalho e ter elementos compreensíveis para decisões responsáveis (H). |
| Restrições/acessibilidade | Pode ser interrompido durante a análise (H). |
| Ambiente típico de uso | Notebook no escritório ou em trabalho remoto; revisão periódica e consulta antes de uma conversa individual, em ambiente que preserve a confidencialidade (H). |
| Comportamentos relevantes | Primeiro observa uma visão geral; depois investiga a mudança, consulta o contexto e conversa com a pessoa antes de decidir (H). |

**Decisões de design influenciadas por P01:**

- Mostrar referência de 30 dias e reanálise de 15 dias com datas explícitas e comparação do próprio histórico, sem ranking entre colaboradores.
- Separar os dois eixos e permitir consultar componentes, fontes e limitações com detalhamento progressivo.
- Distinguir “sem alteração relevante”, “sem dados”, “análise incompleta” e “evidência insuficiente”.
- Oferecer registro restrito de contexto, decisão humana e próximo acompanhamento, como proposta do protótipo.
- Evitar alertas conclusivos e notificações repetitivas; preservar filtros e posição quando houver interrupção.

### Persona P02 — {{João Pedro}}

**Autor(a):** {{Guilherme Matias — 22.122.071-8}}  
**Tipo:** primária  
**Base de evidências:** proto-persona a validar  <br>
**Hipóteses da Entrega 1 relacionadas:** {{H01, H02 ou —}}

![Persona P01](../assets/03_personas/persona_p01.svg)

| Campo | Descrição |
|---|---|
| Faixa etária / contexto relevante | 42 anos. Lidera uma equipe grande e majoritariamente presencial/híbrida de atendimento ao cliente, com alta rotatividade de tarefas (H). |
| Ocupação/papel | Gestor de operações, responsável por metas de atendimento, escalas e bem-estar da equipe (H). |
| Conhecimento do domínio | Forte conhecimento de gestão de pessoas e processos operacionais; pouca familiaridade com métricas de PLN, estatística ou dashboards analíticos (H).|
| Experiência tecnológica | Usa principalmente planilhas, e-mail e sistemas de chamados; sente-se pouco confortável interpretando gráficos sem explicação em linguagem simples (H). |
| Objetivos | Identificar sinais de sobrecarga ou desengajamento antes que virem problema; entender se algo mudou sem depender de jargão técnico; agir com segurança jurídica e ética (H). |
| Necessidades | Explicações em linguagem simples, sem termos técnicos; garantias claras sobre limites e uso adequado do indicador; histórico documentado para justificar decisões (H). |
| Dores/frustrações | Medo de usar a ferramenta de forma equivocada e prejudicar alguém injustamente; desconfiança de números que não entende plenamente; sobrecarga de informação em relatórios longos (H). |
| Motivadores | Proteger a equipe de desgaste, evitar decisões injustas, ter respaldo documentado para conversas difíceis (H). |
| Restrições/acessibilidade | Pouco tempo disponível entre reuniões; prefere leitura rápida e direta, com opção de aprofundar só se necessário (H). |
| Ambiente típico de uso | Sala compartilhada ou home office; consulta rápida antes de decisões pontuais, muitas vezes sob pressão de tempo (H). |
| Comportamentos relevantes | Busca primeiro uma resposta simples ("preciso me preocupar ou não?"); só aprofunda em detalhes técnicos se a situação parecer séria; valoriza confirmação humana antes de agir (H). |

**Decisões de design influenciadas por P01:**

- Oferecer um resumo em linguagem simples antes de qualquer detalhamento técnico ou estatístico.
- Explicitar, de forma acessível, os limites do que o indicador pode e não pode afirmar (evitar leitura como "diagnóstico").
- Priorizar objetividade e brevidade na primeira camada de informação, com aprofundamento opcional.
- Reforçar, em qualquer alerta, a necessidade de conversa humana antes de qualquer ação nunca apresentar como veredito automático.


> Repita para P02, P03... Cada integrante deve produzir ao menos uma persona.

### Síntese das personas

Explique diferenças entre os perfis e qual persona é prioritária. Evite personas duplicadas que só mudam nome/foto.

## 2. Mapa de empatia — equipe

**Persona escolhida:** {{P01}}  
**Justificativa:** {{por que esse perfil é relevante}}

![Mapa de empatia](../assets/03_personas/mapa_empatia.svg)

Documente também em texto: o que vê; ouve; diz/faz; pensa/sente; dores; ganhos. Diferencie **evidência** de **hipótese**.

## 3. Contexto de uso — consolidação

### 3.1. Contexto CT01 - Rafael Costa (P01, primária)

| Dimensão | Descrição | Implicação de design |
|---|---|---|
| Usuários | Gestor autorizado da própria equipe; não especialista em modelos de linguagem (H) | Linguagem de trabalho, definições acessíveis e escopo de equipe explícito |
| Tarefas | Revisar sinais, verificar dados, investigar diferenças, buscar contexto e decidir acompanhamento (H) | Fluxo de visão geral para detalhes e registro restrito de próximos passos |
| Equipamentos | Notebook ou computador; celular apenas como acesso secundário hipotético (H08) | Priorizar legibilidade no desktop sem inviabilizar leitura responsiva |
| Ambiente físico | Escritório ou trabalho remoto, com interrupções e necessidade de privacidade (H) | Preservar filtros e progresso; não expor detalhes em notificações |
| Ambiente social/organizacional | Relação hierárquica com os colaboradores; necessidade de escuta antes de agir (H) | Rótulos neutros e incentivo à contextualização; nenhuma decisão automática |
| Papéis/permissões/governança | Acesso apenas ao escopo e ao nível de detalhe autorizados; configuração técnica separada (P/H04) | Restringir detalhes, informar o escopo e registrar acessos; não pressupor acesso a mensagens brutas |
| Volume de dados/histórico | Referência de 30 dias e reanálise de 15 dias no experimento; número real de pessoas e eventos desconhecido (H) | Exibir datas, cobertura e atualização; não apresentar ausência de dados como estabilidade |

### 3.2. Contexto CT01 - João Pedro (P02, primária)

| Dimensão | Descrição | Implicação de design |
|---|---|---|
| Usuários | Gestor autorizado da própria equipe operacional; pouca familiaridade com métricas de PLN ou estatística (H)| Linguagem simples por padrão, sem jargão técnico; termos explicados na primeira aparição|
| Tarefas | Consultar rapidamente se "há algo a se preocupar"; só aprofunda em componentes/fontes se a situação parecer relevante; registra decisão e justificativa antes de agir (H) | Resposta simples e objetiva na primeira camada, com aprofundamento técnico totalmente opcional |
| Equipamentos | Notebook em sala compartilhada ou home office; acesso entre reuniões, com pouco tempo disponível (H) | Priorizar leitura rápida (poucos cliques até a informação essencial); evitar relatórios longos por padrão |
| Ambiente físico | Ambiente com pressão de tempo e possíveis interrupções; nem sempre em local reservado (H) | Preservar contexto/progresso ao retomar; discrição visual (sem termos sensíveis expostos em tela) |
| Ambiente social/organizacional | Receio de prejudicar alguém injustamente; busca respaldo documentado para decisões e conversas difíceis (H) | Reforçar, em qualquer indicação, que não é diagnóstico nem veredito automático; exigir confirmação humana antes de qualquer ação |
| Papéis/permissões/governança | Acesso restrito ao escopo da própria equipe; não deve inferir acesso a conteúdo bruto de mensagens (H) | Explicitar limites do que o indicador pode/não pode afirmar; registrar decisão e justificativa em linguagem natural, sem exigir conhecimento técnico |
| Volume de dados/histórico | Mesma janela do experimento (30 dias de referência / 15 dias de reanálise); desconhece volume real de eventos por pessoa (H) | Indicar claramente datas e cobertura; diferenciar "sem dados"/"análise incompleta" de "sem alteração relevante", para não gerar falsa sensação de segurança ou de alarme |

## 4. Jornada do usuário — equipe

### 4.1. Jornada J01 - Rafael Costa (P01, primária)

**Persona:** Rafael Costa   <br>
**Objetivo da jornada:** compreender uma mudança e decidir um acompanhamento responsável.  <br>
**Início e fim da jornada:** começa na necessidade de revisar o andamento da equipe e termina na revisão do próximo passo combinado.

| Etapa | Situação/ação | Objetivo | Pensamento/emoção | Dor | Oportunidade de design | Evidência |
|---|---|---|---|---|---|---|
| 1 | {{...}} | {{...}} | {{...}} | {{...}} | {{...}} | {{...}} |

> A jornada pode incluir etapas **antes, durante e depois** do uso do produto. Não transforme a jornada em lista de telas.


### 4.2. Jornada J02 - João Pedro (P02, primária)

**Persona:** João Pedro <br>
**Objetivo da jornada:** obter uma resposta simples e confiável sobre se há necessidade de atenção com alguém da equipe, e decidir com segurança se e como agir. <br> 
**Início e fim da jornada:** começa numa consulta rápida antes de uma decisão pontual (ex: antes de uma reunião ou conversa individual) e termina no registro simples da decisão tomada.

| Etapa | Situação/ação | Objetivo | Pensamento/emoção | Dor | Oportunidade de design | Evidência |
|---|---|---|---|---|---|---|
| 1 | Abre o painel entre duas reuniões, com pouco tempo disponível | Saber rapidamente se "precisa se preocupar ou não" com alguém da equipe | Pressa; quer uma resposta direta sem rodeios | Falta de tempo para explorar relatórios longos | Resumo em linguagem simples logo na abertura, sem exigir navegação por menus técnicos | H |
| 2 | Vê um resumo indicando possível mudança em uma pessoa | Entender, em termos simples, o que esse sinal significa | Insegurança: "isso é grave? é sobre o quê?" | Medo de interpretar mal um termo técnico ou estatístico | Explicações em linguagem acessível, sem jargão, explicando o que o indicador é e não é | H |
| 3 | Decide se quer aprofundar ou não, dependendo da gravidade percebida | Confirmar se vale a pena investigar mais a fundo | Cautela; não quer "abrir uma caixa" sem necessidade | Risco de ignorar algo importante por falta de clareza | Aprofundamento técnico disponível, mas totalmente opcional e não obrigatório para decidir | H |
| 4 | Ao aprofundar, verifica se há dados suficientes e atualizados | Garantir que a informação é confiável antes de agir | Necessidade de segurança e respaldo | Agir com base em dado incompleto e prejudicar alguém injustamente | Indicação clara de "sem dados", "análise incompleta" ou "evidência insuficiente", nunca omitida | H |
| 5 | Conversa com a pessoa (fora da ferramenta), já ciente de que o sinal não é diagnóstico | Confirmar humanamente a situação antes de decidir qualquer ação | Empatia; alívio por saber que não precisa agir sozinho com base no dado | Risco de tratar um sinal do sistema como verdade absoluta, sem ouvir a pessoa | Reforço explícito, em qualquer indicação, de que o sinal exige conversa humana antes de qualquer ação — nunca apresentado como veredito automático | H |


> A jornada pode incluir etapas **antes, durante e depois** do uso do produto. Não transforme a jornada em lista de telas.

## Síntese

Quais necessidades e objetivos devem obrigatoriamente aparecer nos cenários e nas tarefas seguintes?

## Checklist

- [ ] Existe pelo menos uma persona por integrante.
- [ ] As personas não são apenas diferenças demográficas superficiais.
- [ ] Está claro o que é dado real e o que é hipótese/proto-persona.
- [ ] A persona não “validou por ficção” uma hipótese da Entrega 1; afirmações continuam marcadas como hipótese quando não há evidência.
- [ ] Objetivos e dores têm consequência para o design.
- [ ] Contexto de uso está coerente com a Entrega 1.
- [ ] Em TCC sem interface original, a persona possui relação explícita com a contribuição técnica.
- [ ] Papéis administrativos, técnicos e decisórios só foram criados quando possuem objetivos/tarefas diferentes.
- [ ] Jornada possui etapas, dores e oportunidades e não é apenas wireflow.
- [ ] IDs das personas foram adicionados à rastreabilidade.
