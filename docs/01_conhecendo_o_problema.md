# Entrega 1 — Conhecendo o projeto, o usuário e o problema

**Data:** {{19/08/2026}}  
**Status:** 🟨 em andamento 
**Responsabilidade:** 1 solução consolidada por equipe

## Objetivo da atividade

Reinterpretar o tema do TCC sob a perspectiva de Interação Humano-Computador e construir um **entendimento comum entre os integrantes da equipe**.

A disciplina utiliza preferencialmente o tema do TCC para os exercícios de IHC. Isso vale tanto para TCCs que já preveem uma interface quanto para trabalhos cujo resultado principal é algoritmo, modelo, API, biblioteca, análise de dados, infraestrutura, estudo experimental ou outro artefato técnico.

> **Importante:** a interface projetada na disciplina é um artefato de aprendizagem de IHC. Ela **não se torna automaticamente uma obrigação do TCC**. Sua incorporação ao trabalho de conclusão depende de decisão da equipe e do orientador.

Antes de preencher, leia [`../GUIA_ESCOPO_IHC.md`](../GUIA_ESCOPO_IHC.md).

Nesta primeira semana a equipe **não deve começar desenhando telas**. Primeiro deverá compreender:

- o que o TCC realmente produz;
- quem poderia obter valor dessa contribuição;
- quais pessoas interagem, administram, configuram, interpretam ou são afetadas;
- o que essas pessoas precisam alcançar;
- como atividades relacionadas acontecem hoje;
- problemas, limitações e contexto;
- alternativas existentes;
- qual recorte de interação fará sentido para a disciplina.

Ao final desta entrega, a equipe deve diferenciar:

- **tema do TCC** × **escopo formal do TCC** × **escopo de IHC da disciplina**;
- **objetivo do projeto** × **objetivo do usuário**;
- **problema do usuário** × **solução tecnológica**;
- **fato conhecido** × **hipótese** × **lacuna de conhecimento**;
- **capacidade técnica** × **forma de uso dessa capacidade**;
- **funcionalidade** × **atividade/resultado que o usuário precisa alcançar**;
- **usuário direto** × **stakeholders**.

---

## Como classificar as respostas

Sempre que a resposta fizer uma afirmação sobre usuários, problemas, atividades, necessidades, contexto ou mercado, use:

- **[F] Fato conhecido** — existe evidência/fonte.
- **[H] Hipótese** — afirmação plausível que ainda precisa ser investigada.
- **[?] Não sabemos ainda** — lacuna relevante.

Quando usar `[F]`, informe a origem. Hipóteses prioritárias devem receber IDs (`H01`, `H02`...) e também ser registradas em [`../RASTREABILIDADE.md`](../RASTREABILIDADE.md).

> **Exemplo:** `[H] H01 — DBAs considerariam útil comparar automaticamente o plano atual de execução com uma recomendação produzida pelo algoritmo.`

Uma hipótese explicitada é melhor do que uma suposição escondida.

---

# 0. Identificação do TCC e da equipe

## 0.1 Membros

| Caio Arnoni | 22.221.019-7 | @caioarnoni21 |
| Guilherme Matias Rodrigues de Souza | 22.122.071-8 | [?] |
| Tainá Cunha Bueno | 22.119.025-9 | [?] |

## 0.2 Título atual do TCC

**Ferramenta baseada em Inteligência Artificial para Apoio à Identificação de Alterações nos Padrões de Comunicação, Interação e Desempenho em Equipes.**


## 0.3 Orientador(a)

**Plinio Thomaz Aquino Junior.**

## 0.4 Qual é o resultado principal atualmente previsto no TCC?

Marque e descreva:

- [x] sistema/aplicação interativa;
- [x] algoritmo;
- [ ] modelo de IA/ML/LLM;
- [ ] biblioteca/API/framework;
- [x] análise de dataset;
- [x] estudo/benchmark/avaliação experimental;
- [x] infraestrutura/backend;
- [ ] componente embarcado/IoT;
- [x] outro: pipeline experimental de coleta, processamento, cálculo de scores e geração de sinalizações.

**Descrição:** [H] H01 - O TCC prevê o desenvolvimento e a avaliação experimental do WorkSense. A ferramenta recebe interações comunicacionais simuladas e registros de tarefas, extrai indicadores, calcula separadamente um score comunicacional e um score profissional e compara ciclos de reanálise com o baseline de cada perfil. A solução inclui um bot no Telegram, integrações entre serviços, armazenamento, algoritmos de processamento e visualizações preliminares.

## 0.5 O TCC já previa desenvolvimento de interface com usuário?

- [ ] Sim, a interface já faz parte do TCC.
- [x] Parcialmente; existe alguma interação, mas ainda não está bem definida.
- [ ] Não. O TCC é predominantemente técnico e não previa interface.

**Explique o que está formalmente previsto no TCC:** {{...}}

** [H] H02 - Está prevista uma interação conversacional por Telegram para envio de mensagens, áudios e comandos de tarefas. O texto também prevê visualizações dos scores e sinalizações, mas ainda não define uma interface de gestão completa, seus fluxos de uso ou requisitos de usabilidade. As visualizações atuais são gráficos preliminares de resultados experimentais.

# 1. Entendendo a contribuição do projeto

## 1.1 Explique o TCC em uma frase, sem citar linguagem de programação, framework ou banco de dados.

[H] H03 - O WorkSense apoia a identificação de alterações ao longo do tempo nos padrões de comunicação, interação e execução de tarefas de perfis profissionais, mantendo a interpretação e a decisão sob responsabilidade humana.

## 1.2 Qual situação, atividade ou problema do mundo real motivou o TCC?

[F] F01 - As transformações nas formas de trabalho, com equipes atuando entre ambientes presenciais, remotos e digitais, tornaram mais difícil perceber mudanças sutis na rotina profissional dos colaboradores. Alterações na forma de comunicação, na frequência das interações ou na evolução das entregas podem ocorrer gradualmente e passar despercebidas no acompanhamento cotidiano. Ao mesmo tempo, parte dessas interações e atividades deixa registros digitais que podem ser analisados ao longo do tempo para apoiar essa percepção.

## 1.3 Qual é a **capacidade/contribuição central** produzida pelo TCC?
****** citação de hipótese
[H] H03 - Identificar mudanças nos padrões de comunicação, interação e indicadores profissionais ao longo do tempo, utilizando o histórico individual como referência e gerando sinalizações para apoiar a análise humana, sem caráter diagnóstico ou punitivo.

## 1.4 O que se espera que esteja diferente **para pessoas, organizações ou processos** se essa contribuição for bem-sucedida?

[H] H04 - A contribuição pode tornar o acompanhamento das equipes mais estruturado e preventivo, auxiliando gestores na identificação e interpretação de variações, favorecendo um acompanhamento mais contextualizado dos colaboradores e apoiando a organização em decisões de gestão mais informadas e transparentes, sempre com supervisão humana.

## 1.5 O que é mérito técnico/científico do TCC e o que seria uma possível aplicação prática?

| Mérito/contribuição técnica | Possível aplicação/valor em uso |
|---|---|
| Integração de dados comunicacionais e operacionais em um único pipeline experimental. | Oferecer uma visão mais estruturada de diferentes dimensões da rotina profissional que normalmente seriam acompanhadas de forma isolada. |
| Extração de indicadores linguísticos, de polaridade textual, semânticos e profissionais relacionados a frequência, prazo e qualidade. | Transformar registros digitais existentes em informações organizadas que possam apoiar a percepção de mudanças ao longo do tempo. |
| Construção de scores comunicacional e profissional independentes. | Permitir que alterações em comunicação e em aspectos profissionais sejam analisadas separadamente, sem que uma dimensão compense ou oculte a outra. |
| Utilização de baseline individual e ciclos temporais de reanálise. | Avaliar mudanças em relação ao histórico do próprio perfil, em vez de comparar pessoas diferentes. |
| Desenvolvimento de uma abordagem experimental para sinalização de alterações de padrão a partir de múltiplos indicadores. | Apoiar gestores na identificação de situações que mereçam análise mais aprofundada, sem transformar os scores em avaliações definitivas de desempenho ou comportamento. |
| Estruturação de uma estratégia de avaliação para verificar a resposta dos indicadores e scores a alterações de padrão. | Verificar se as sinalizações produzidas pela ferramenta representam adequadamente mudanças observadas nos dados. |
| Apresentação dos scores juntamente com seus componentes e manutenção da supervisão humana na interpretação dos resultados. | Permitir que o gestor compreenda quais dimensões contribuíram para uma sinalização e interprete o resultado dentro do contexto, sem caráter diagnóstico ou punitivo. |


# 2. Entendendo as pessoas envolvidas

## 2.1 Quem interage diretamente com o produto, se já existe interface prevista?

[H] H05 - O gestor ou líder de equipe será o usuário direto da interface prevista para o WorkSense. Por meio dela, poderá cadastrar e vincular os usuários dos colaboradores às fontes de dados utilizadas pela ferramenta, acompanhar os perfis cadastrados e visualizar seus scores comunicacionais e profissionais, sinalizações e os indicadores que contribuíram para cada resultado.

## 2.2 Quem poderia **usar, configurar, administrar, operar, interpretar ou tomar decisões** a partir da contribuição técnica?

Considere perfis profissionais e stakeholders, não apenas consumidores finais.

| Perfil | Relação com a contribuição | O que faria | Status/evidência |
|---|---|---|---|
| Gestor ou líder de equipe | Usuário principal da interface e responsável pela interpretação dos resultados | Cadastraria e vincularia colaboradores, acompanharia seus scores e sinalizações, consultaria os indicadores envolvidos e decidiria se alguma situação merece acompanhamento humano | [H] H05; usuário principal da interface |
| Colaborador | Pessoa associada ao perfil acompanhado pela ferramenta | Utilizaria normalmente os canais integrados ao WorkSense, como o agente conversacional e a ferramenta de tarefas, gerando os registros utilizados na análise. Não teria acesso à interface de gestão prevista | [H] H06 — O colaborador será a principal pessoa acompanhada pela ferramenta, produzindo registros comunicacionais e profissionais utilizados nas análises, mas não utilizará diretamente a interface de gestão |
| Profissional de RH ou responsável pela gestão de pessoas | Stakeholder interessado no uso adequado da ferramenta | Poderia auxiliar na definição de políticas de uso, transparência, consentimento e limites para interpretação das sinalizações | [H] H07 — Profissionais de RH ou responsáveis pela gestão de pessoas poderão atuar como stakeholders do WorkSense, contribuindo para políticas de uso, transparência, consentimento e limites de interpretação das sinalizações |
| Administrador da solução | Responsável pela operação e configuração técnica | Configuraria integrações, acessos, permissões, credenciais e demais parâmetros necessários ao funcionamento da ferramenta | [H] H08 — A operação do WorkSense exigirá um perfil de administração responsável por configurar integrações, acessos, permissões, credenciais e demais parâmetros técnicos da solução |
| Pesquisadores/equipe do TCC | Desenvolve, opera e avalia a solução experimental | Prepararia os dados utilizados no experimento, executaria os módulos de processamento, testaria a solução e avaliaria os resultados obtidos | [H] H09 — Durante o contexto experimental do TCC, a equipe de pesquisadores será responsável por preparar os dados de avaliação, executar os processamentos, realizar testes e analisar os resultados produzidos pela ferramenta. |

## 2.3 Existem pessoas afetadas que não usariam a interface diretamente?

| Stakeholder | Como é afetado | Usa interface? | Status/evidência |
|---|---|---|---|
| Colaborador | Seus registros de comunicação e de atividades podem compor os indicadores e scores apresentados ao gestor. Pode ser afetado pelas interpretações e ações de acompanhamento decorrentes das sinalizações | Não | [H] H06; principal pessoa afetada pelos resultados |
| Profissional de RH ou responsável pela gestão de pessoas | Mesmo sem utilizar a interface no escopo atual, pode ser afetado pelas necessidades de definição de políticas de uso, consentimento, transparência e limites para utilização das sinalizações no ambiente organizacional | Não | [H] H07; stakeholder relacionado à governança do uso.

## 2.4 Que características desses perfis podem influenciar a interação?

Considere conhecimento do domínio, experiência tecnológica, frequência de uso, necessidades de acessibilidade, responsabilidade profissional, familiaridade com métricas, linguagem técnica, urgência etc.

[H] H10 - Gestores podem apresentar diferentes níveis de familiaridade com métricas, indicadores e ferramentas digitais, além de diferentes frequências e contextos de acompanhamento da equipe. A interface deve permitir compreender scores, variações e sinalizações sem exigir conhecimento técnico sobre IA ou sobre os algoritmos utilizados.

[H] H11 - Colaboradores apresentam padrões distintos de comunicação, interação e utilização das ferramentas de trabalho e podem possuir diferentes percepções sobre a finalidade e o uso de seus dados pela solução.

[H] H12 - Profissionais de RH ou responsáveis pela gestão de pessoas tendem a possuir maior familiaridade com processos organizacionais, privacidade e governança, mas podem apresentar diferentes níveis de familiaridade com indicadores quantitativos e ferramentas digitais.

[H] H13 - Administradores da solução necessitam de maior familiaridade técnica com integrações, acessos, permissões e configurações para realizar atividades de implantação e manutenção do WorkSense.

[H] H14 - Os pesquisadores/equipe do TCC necessitam de maior nível de detalhamento técnico sobre indicadores, scores e processamento dos dados para testar e avaliar a solução experimental.

# 3. Entendendo objetivos e atividades

## 3.1 O que o usuário está tentando conseguir no mundo real?

investigar como uma ferramenta baseada em inteligência artificial pode apoiar gestores na identificação de indícios de alteração nos padrões de comunicação, interação e desempenho de colaboradores 

** citação de hipótese **
[H] H04; o gestor busca acompanhar a equipe de forma mais estruturada e preventiva, percebendo mudanças relevantes na rotina dos colaboradores, compreendendo melhor essas variações e decidindo quando é necessário algum acompanhamento humano.

## 3.2 Quais são as atividades mais importantes?

| ID | Atividade/objetivo | Quem realiza | Frequência/criticidade inicial | Status/evidência |
|---|---|---|---|---|
| A01 | Atribuir e organizar tarefas no quadro Kanban, definindo responsável, descrição e prazo | Gestor | Contínua / Alta | {{...}} |
| A02 | Executar e atualizar as tarefas, realizando a movimentação dos cartões entre as etapas do Kanban e registrando as interações relacionadas às atividades e tirando duvidas com a IA integrada Ollama | Colaborador | Diária / Alta | {{...}} |
| A03 | Analisar os dados coletados e identificar alterações de padrão por meio dos indicadores comunicacionais e profissionais e da comparação com o baseline | Sistema / Gestor | A cada ciclo de análise / Alta | {{...}} |

## 3.3 Qual atividade parece mais frequente? Por quê?

A mais frequente é a execução e atualização das tarefas pelos colaboradores. Isso ocorre porque, durante o desenvolvimento das atividades, os colaboradores podem consultar suas tarefas, interagir pelo Telegram, esclarecer dúvidas com o agente de IA e movimentar os cartões no Kanban conforme o andamento do trabalho

{{[F/H/?] ...}}

## 3.4 Qual parece mais crítica? Que consequência existe se for mal executada?

A atividade mais crítica seria a análise dos dados e identificação de alterações nos padrões, pois é responsável por transformar os registros coletados em indicadores, scores e sinalizações para o gestor. Se for mal executada, pode gerar sinalizações incorretas ou deixar de identificar alterações planejadas, comprometendo a avaliação da ferramenta

{{[F/H/?] ...}}

---

# 4. Entendendo o problema ou processo atual

## 4.1 Como essas atividades são realizadas hoje, antes da interface imaginada na disciplina?

É feito manualmente o registros dos colaboradores no banco de dados dentro da VPS e a analise por meio de script

{{[F/H/?] ...}}

## 4.2 O que é difícil, demorado, confuso, repetitivo, arriscado ou pouco transparente?

É difícil para o gestor perceber alterações sutis nos padrões de comunicação, interação e desempenho ao longo do tempo, especialmente quando essas informações estão distribuídas entre mensagens, registros de tarefas e métricas operacionais. A simples disponibilidade desses dados não garante que estejam organizados de maneira interpretável e temporalmente comparável

{{[F/H/?] ...}}

## 4.3 Que informações o profissional precisa interpretar para tomar decisão?

O profissional precisa considerar, em conjunto, os indicadores comunicacionais e profissionais. No eixo comunicacional, são relevantes sentimento/polaridade, frequência de mensagens, tamanho das respostas, quantidade de palavras, diversidade lexical e estabilidade ou mudança semântica. No eixo profissional, são considerados frequência de ações, cumprimento de prazos e sinais de qualidade, como reabertura de cartões e pendências em checklist

{{[F/H/?] ...}}

## 4.4 O que acontece quando a atividade falha ou quando o resultado é interpretado incorretamente?

Uma sinalização incorreta pode levar o gestor a interpretar uma alteração textual ou operacional fora de seu contexto. Isso é especialmente problemático porque uma mudança na polaridade, no conteúdo semântico ou nos registros de tarefas não determina, por si só, sua causa. O trabalho destaca justamente a necessidade de análise humana complementar.

{{[F/H/?] ...}}

## 4.5 Conte uma situação concreta.

Um gestor acompanha uma equipe e precisa perceber se determinado profissional está apresentando uma alteração relevante em sua rotina. Durante um período de acompanhamento, as mensagens enviadas pelo perfil passam a apresentar mudanças em frequência e conteúdo, enquanto os registros de tarefas também podem indicar alterações na rotina de trabalho. O gestor precisa analisar essas informações em relação ao histórico anterior do profissional, mas os dados estão distribuídos entre diferentes registros e uma alteração isolada pode ter várias explicações. Se a mudança for interpretada sem considerar o contexto e os demais indicadores, existe o risco de atribuir significado incorreto ao comportamento observado


{{[F/H/?] narrativa...}}

## 4.6 Que evidência existe hoje?

| Evidência/fonte | O que sustenta | Limitação |
|---|---|---|
| {{...}} | {{...}} | {{...}} |

---

# 5. Entendendo o contexto de uso

## 5.1 Onde e em quais situações a interação poderia ocorrer?

Em ambiente corporativo, no escritório ou em trabalho remoto, durante revisão periódica da equipe, preparação para reunião individual, planejamento de capacidade, acompanhamento de prazos ou análise de uma sinalização específica.

{{[F/H/?] ...}}

## 5.2 Em quais dispositivos/equipamentos?

Computador ou notebook será o dispositivo principal para análise detalhada. Um dispositivo móvel poderá ser usado para consulta breve ou notificação, mas não é considerado inicialmente adequado para investigações extensas.

{{[F/H/?] ...}}

## 5.3 Existem condições físicas relevantes?

A interação pode ocorrer sob interrupções e pressão de tempo. Como envolve informações sensíveis, a tela deve ser usada em ambiente com privacidade visual e não deve permanecer exposta em monitores compartilhados.

{{[F/H/?] ...}}

## 5.4 Existem fatores sociais ou organizacionais?

Sim. Relações hierárquicas, assimetria de poder, permissões, responsabilidade do gestor, confiança da equipe, políticas internas e legislação de proteção de dados influenciam o uso. Uma mesma sinalização não deve ser visível a qualquer pessoa nem utilizada fora da finalidade declarada.

{{[F/H/?] ...}}

## 5.5 Existe necessidade de histórico, rastreabilidade ou auditoria?

Sim. O histórico é necessário para comparar cada ciclo de 15 dias com o baseline individual de 30 dias e acompanhar a evolução dos scores.

Na interface do gestor, a rastreabilidade deverá mostrar o período e as fontes analisadas, os indicadores que originaram a sinalização, a data do processamento, quem realizou a análise e qual encaminhamento foi registrado, sem expor conteúdo bruto desnecessário.

{{[F/H/?] ...}}

## 5.6 Um erro pode produzir consequência relevante? Qual?

Sim. A interpretação incorreta pode afetar privacidade, confiança, relações de trabalho e decisões sobre pessoas. Por isso, a interface deverá comunicar incerteza, insuficiência de dados e proibição de uso diagnóstico ou punitivo.

{{[F/H/?] ...}}

---

# 6. Entendendo mercado e alternativas existentes

> Nesta entrega faça apenas um **levantamento inicial**. A análise aprofundada ocorre na Entrega 2.

## 6.1 Como pessoas resolvem problemas semelhantes hoje?

| Alternativa atual | Quem usa | Para quê | Status/evidência |
|---|---|---|---|
| Conversas, reuniões e observação cotidiana | Gestores e equipes | Compreender dificuldades e acompanhar o trabalho | Processo real ainda precisa ser investigado |
| Telegram, Teams, Slack ou e-mail | Equipes | Comunicação e registro de interações | [F] Classe de ferramentas existente; Telegram integra o TCC |
| Trello e outros quadros Kanban | Equipes e gestores | Organizar tarefas, prazos e responsáveis | [F] Trello utilizado no TCC |
| Planilhas, relatórios e scripts | Pesquisadores/analistas | Consolidar dados e calcular indicadores | [F] Processo experimental atual do TCC |
| Microsoft Viva Insights | Gestores, líderes e analistas | Analisar padrões de colaboração, produtividade e bem-estar |  (https://learn.microsoft.com/en-us/viva/insights/introduction) |
| ActivTrak | Gestores e líderes | Acompanhar produtividade, carga de trabalho e tendências | (https://support.activtrak.com/hc/en-us/articles/18821721976475-Organization-Overview) |
| Worklytics | Lideranças, RH e People Analytics | Integrar métricas de colaboração e trabalho com foco em privacidade | (https://www.worklytics.co/workplace-insights-dashboard) |
| Workday Peakon Employee Voice | Gestores, RH e colaboradores | Coletar feedback, acompanhar sentimento, prioridades e planos de ação | (https://www.workday.com/en-us/products/employee-voice/overview.html) |

## 6.2 Existem produtos que atuam na mesma área, mesmo sem serem equivalentes ao TCC?

Sim. Microsoft Viva Insights, ActivTrak, Worklytics e Workday Peakon atuam em áreas próximas, como workplace analytics, people analytics, produtividade, colaboração, bem-estar e escuta contínua.

{{[F/H/?] ...}}

## 6.3 Quais interfaces profissionais esse público já conhece?

[H] Gestores provavelmente conhecem dashboards, relatórios, planilhas, sistemas administrativos, ferramentas de comunicação, calendários e quadros Kanban. Analistas podem conhecer ferramentas de BI e visualização de dados.

{{[F/H/?] ...}}

## 6.4 O que essas soluções parecem fazer bem?

As soluções observadas organizam informações em visões gerais, filtros por período e grupo, comparações temporais, cartões de indicadores e aprofundamento progressivo. Algumas também separam papéis de acesso, apresentam planos de ação e adotam agregação ou anonimização para reduzir riscos de privacidade.

{{[F/H/?] ...}}

## 6.5 O que parecem fazer mal, dificultar ou não atender?

Algumas interfaces exibem grande quantidade de métricas, o que pode exigir conhecimento analítico. Produtos de monitoramento podem reforçar sensação de vigilância. Soluções de employee listening dependem principalmente de pesquisas, enquanto ferramentas de produtividade podem enfatizar atividade e tempo. Ainda não sabemos se alguma alternativa combina, de maneira comparável ao WorkSense, conteúdo comunicacional, registros de tarefas, baseline individual, scores separados e explicabilidade.

{{[F/H/?] ...}}

## 6.6 Que padrões de interface ou vocabulário parecem familiares a esse público?

Menu lateral por área; cartões de indicadores; filtros de data, equipe e perfil; gráficos de tendência; comparação antes/depois; status de alerta; detalhamento por clique; tabelas com ordenação; exportação; histórico; permissões por papel; e termos como período, tendência, baseline, score, indicador, participação, carga de trabalho e plano de ação.

{{[F/H/?] ...}}

---

# 7. Derivando o escopo de IHC da disciplina

## 7.1 Escolha o caminho do projeto

### Caminho A — TCC já possui interface

Explique qual parte da interface será usada como recorte da disciplina e por que esse fluxo é relevante.

{{...}}

### Caminho B — TCC não possui interface prevista

Faça o exercício de transferência de uso:

> **Imagine que o TCC foi concluído com sucesso e uma empresa, laboratório ou organização quer transformar a contribuição em algo utilizável. Quem precisaria interagir com ela e para quê?**

Responda:

1. quem poderia contratar/adotar a solução? {{...}}
2. quem seria o usuário direto? {{...}}
3. quem administraria/configuraria? {{...}}
4. quem interpretaria resultados? {{...}}
5. quem tomaria decisões? {{...}}
6. quais dados/entradas seriam necessários? {{...}}
7. quais resultados deveriam ser compreendidos? {{...}}
8. que erros/rupturas seriam possíveis? {{...}}

## 7.2 Qual perfil será priorizado no projeto de IHC?

{{...}}

**Por que esse perfil foi escolhido?** {{...}}

## 7.3 Qual objetivo desse usuário será priorizado?

{{...}}

## 7.4 Que interface será explorada na disciplina?

Complete:

> **Para fins da disciplina de IHC, será projetada uma interface que permita a `{{perfil}}` utilizar `{{capacidade/resultado do TCC}}` para `{{objetivo}}`, no contexto de `{{situação}}`.**

{{...}}

## 7.5 Qual é a relação dessa interface com o TCC?

- [ ] Já fazia parte do TCC.
- [ ] É um aprofundamento de algo parcialmente previsto.
- [ ] É uma extensão conceitual criada para a disciplina.
- [ ] É um protótipo demonstrativo de aplicação potencial.
- [ ] Outra: {{...}}.

> **Declaração:** a interface desenvolvida nesta disciplina é um artefato de aprendizagem de IHC baseado no tema do TCC. Sua inclusão ou implementação no TCC somente ocorrerá se isso for posteriormente decidido pela equipe e pelo orientador.

---

# 8. Levantando possibilidades de interação — sem desenhar ainda

A equipe pode registrar possibilidades para investigação. **Não significa que todas serão implementadas.**

Marque apenas as que parecem plausíveis e explique o objetivo correspondente.

| Possibilidade | Pode fazer sentido? | Objetivo/tarefa que justificaria | Evidência atual |
|---|---|---|---|
| Dashboard/visão geral | sim/não/talvez | {{...}} | {{...}} |
| Configuração/parametrização | sim/não/talvez | {{...}} | {{...}} |
| Entrada/upload/seleção de dados | sim/não/talvez | {{...}} | {{...}} |
| Acompanhamento de processamento | sim/não/talvez | {{...}} | {{...}} |
| Relatório/resultados | sim/não/talvez | {{...}} | {{...}} |
| Histórico com busca/filtros | sim/não/talvez | {{...}} | {{...}} |
| Comparação de resultados | sim/não/talvez | {{...}} | {{...}} |
| Explicabilidade/detalhamento | sim/não/talvez | {{...}} | {{...}} |
| Administração/configurações globais | sim/não/talvez | {{...}} | {{...}} |
| Usuários/perfis/permissões | sim/não/talvez | {{...}} | {{...}} |
| CRUD de entidade do domínio | sim/não/talvez | {{...}} | {{...}} |
| Auditoria/logs | sim/não/talvez | {{...}} | {{...}} |
| Alertas/ocorrências | sim/não/talvez | {{...}} | {{...}} |
| Ajuda/documentação | sim/não/talvez | {{...}} | {{...}} |

> **Atenção:** “login + dashboard + CRUD” não é uma solução universal. Cada padrão deve surgir de uma tarefa real.

---

# 9. Benefícios e ações iniciais

## 9.1 Qual benefício concreto o projeto de IHC pretende oferecer?

| Benefício esperado | Problema/necessidade | Usuário | Status/evidência |
|---|---|---|---|
| {{...}} | {{...}} | {{...}} | {{...}} |

## 9.2 Que ações o usuário deverá conseguir realizar?

| ID | O usuário precisa conseguir... | Para alcançar... | Prioridade inicial |
|---|---|---|---|
| F01 | {{ação}} | {{objetivo}} | alta/média/baixa |

## 9.3 Tecnologias/restrições já definidas no TCC

A tecnologia aparece **agora**, depois do entendimento do uso.

| Tecnologia/restrição | Por que existe | Possível impacto na interação |
|---|---|---|
| {{...}} | {{...}} | {{...}} |

---

# 10. Hipóteses e dúvidas prioritárias

| ID | Hipótese/dúvida | Por que importa | Como poderá ser investigada |
|---|---|---|---|
| H01 | {{...}} | {{...}} | Entrega 2/3/7/... |
| H02 | {{...}} | {{...}} | {{...}} |
| H03 | {{...}} | {{...}} | {{...}} |

Registre em [`../RASTREABILIDADE.md`](../RASTREABILIDADE.md).

---

# 11. Síntese da equipe

| Pergunta | Síntese atual |
|---|---|
| Qual é a contribuição central do TCC? | {{...}} |
| O TCC já previa interface? | {{...}} |
| Quem é o usuário prioritário de IHC? | {{...}} |
| O que ele precisa alcançar? | {{...}} |
| Qual problema/atividade será estudado? | {{...}} |
| Como isso acontece hoje? | {{...}} |
| Qual é o contexto de uso? | {{...}} |
| Que interface/recorte será explorado? | {{...}} |
| Como a interface se relaciona ao TCC? | {{...}} |
| Quais pontos ainda são hipóteses? | {{H01...}} |

### Delimitação

**Dentro do escopo de IHC:** {{...}}  
**Fora do escopo de IHC:** {{...}}  
**Dentro do escopo formal do TCC:** {{...}}  
**Interface da disciplina será implementada no TCC?** não definido / sim / não — {{justificativa, se houver}}

---

# 12. Como esta entrega alimenta as próximas

- **Entrega 2:** verifica mercado, concorrentes e interfaces profissionais representativas.
- **Entrega 3:** detalha perfis e contexto.
- **Entrega 4:** aprofunda situações problemáticas.
- **Entrega 5:** modela tarefas centrais.
- **Entrega 6:** experimenta alternativas em baixa fidelidade.
- **Entrega 7:** investiga hipóteses com dados.
- **Entrega 8:** define restrições e metas de usabilidade.
- **Entregas 9–11:** transformam o recorte em modelo de interação e protótipo.
- **Entregas 12–14:** avaliam a interface construída na disciplina.

A Entrega 1 é uma **fotografia inicial do conhecimento**. Ela pode e deve ser revisada quando surgirem evidências.

---

# 13. Relação com INOVA e comunicação do projeto

Prepare uma explicação de até três frases:

1. **Problema/atividade humana:** {{...}}
2. **Contribuição técnica do TCC:** {{...}}
3. **Como uma pessoa poderia utilizar essa contribuição:** {{...}}

Essa síntese ajuda a apresentar o projeto para público não especializado sem reduzir seu mérito técnico.

---

# Checklist de qualidade

- [ ] Está clara a diferença entre tema do TCC, escopo formal do TCC e escopo de IHC.
- [ ] A equipe declarou se o TCC já previa interface.
- [ ] Se não previa, foi derivado um usuário plausível e um objetivo de uso.
- [ ] A interface de IHC não foi apresentada como obrigação automática do TCC.
- [ ] A contribuição do TCC foi descrita sem começar por tecnologias de implementação.
- [ ] Usuários diretos e stakeholders foram diferenciados.
- [ ] Foram considerados profissionais que configuram, administram, interpretam ou decidem, quando pertinente.
- [ ] Objetivo do usuário não foi confundido com objetivo do projeto.
- [ ] Processo/problema atual foi descrito antes da solução.
- [ ] Existe situação concreta de uso/problema.
- [ ] Contexto físico, social/organizacional, dispositivos e consequências de erro foram considerados.
- [ ] Mercado/alternativas existentes foram levantados inicialmente.
- [ ] Possibilidades como dashboard, relatório, histórico, filtros e CRUD foram tratadas como hipóteses de solução, não como requisitos automáticos.
- [ ] Cada possibilidade de interface tem um objetivo/tarefa que poderia justificá-la.
- [ ] Afirmações relevantes estão marcadas `[F]`, `[H]` ou `[?]`.
- [ ] Hipóteses prioritárias receberam IDs e foram para a rastreabilidade.
- [ ] O recorte de IHC é viável para modelar, prototipar e avaliar no semestre.
- [ ] A equipe consegue explicar problema humano → contribuição computacional → forma de uso.
