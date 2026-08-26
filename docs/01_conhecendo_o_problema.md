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

[H03] Identificar mudanças nos padrões de comunicação, interação e indicadores profissionais ao longo do tempo, utilizando o histórico individual como referência e gerando sinalizações para apoiar a análise humana, sem caráter diagnóstico ou punitivo.

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

[H04] O gestor busca acompanhar a equipe de forma mais estruturada e preventiva, percebendo mudanças relevantes na rotina dos colaboradores, compreendendo melhor essas variações e decidindo quando é necessário algum acompanhamento humano.

## 3.2 Quais são as atividades mais importantes?

| ID | Atividade/objetivo | Quem realiza | Frequência/criticidade inicial | Status/evidência |
|---|---|---|---|---|
| A01 | Atribuir e acompanhar tarefas no quadro Kanban, definindo responsáveis, descrições e prazos | Gestor | Contínua / Alta | [H] H15 |
| A02 | Executar e atualizar as tarefas, movimentando cartões conforme o andamento do trabalho e utilizando os canais integrados ao WorkSense | Colaborador | Diária / Alta | [H] H16 |
| A03 | Acompanhar e interpretar variações apresentadas pelo WorkSense, considerando scores, indicadores, histórico individual e contexto do colaborador | Gestor | A cada ciclo ou sinalização / Alta | [H] H04; [H] H05 |

## 3.3 Qual atividade parece mais frequente? Por quê?

[H16] A execução e atualização das tarefas parece ser a atividade mais frequente, pois ocorre durante a rotina de trabalho dos colaboradores, envolvendo o acompanhamento das atividades e o registro de seu andamento.

## 3.4 Qual parece mais crítica? Que consequência existe se for mal executada?

[H] H17 - A interpretação das sinalizações pelo gestor parece ser uma das atividades mais críticas, pois uma interpretação inadequada pode atribuir significado incorreto a uma variação ou levar a uma ação de acompanhamento sem contexto suficiente. Por isso, os resultados precisam ser apresentados com seus indicadores e permanecer sujeitos à análise humana.

---

# 4. Entendendo o problema ou processo atual

## 4.1 Como essas atividades são realizadas hoje, antes da interface imaginada na disciplina?

[H] H18 - Atualmente, o gestor tende a acompanhar a equipe por meio de diferentes fontes e momentos de contato, como reuniões, conversas presenciais/online e registros em ferramentas de gestão de tarefas, precisando interpretar essas informações durante o acompanhamento cotidiano.

## 4.2 O que é difícil, demorado, confuso, repetitivo, arriscado ou pouco transparente?

[F01] Alterações sutis na comunicação, interação e evolução das atividades podem ser difíceis de perceber ao longo do acompanhamento cotidiano, especialmente quando os registros precisam ser observados em diferentes momentos e contextos.

## 4.3 Que informações o profissional precisa interpretar para tomar decisão?

[H] H19 - Para compreender mudanças na rotina de um colaborador, o gestor pode considerar informações como frequência e características das interações, andamento e regularidade das entregas, cumprimento de prazos, ocorrências de retrabalho e mudanças no contexto de trabalho, interpretando essas informações em relação ao histórico daquele profissional.

## 4.4 O que acontece quando a atividade falha ou quando o resultado é interpretado incorretamente?

[F] F02 - Indicadores comunicacionais ou profissionais isolados podem admitir diferentes interpretações. Uma mensagem classificada como negativa pode representar, por exemplo, uma dificuldade técnica, enquanto eventos de tarefas podem refletir características do processo ou da própria atividade. Por isso, uma interpretação incorreta pode atribuir significado indevido a uma sinalização, justificando a necessidade de contexto e supervisão humana.

## 4.5 Conte uma situação concreta.

[H18]; [H19] Um gestor acompanha um colaborador ao longo de sua rotina por meio de interações e registros de trabalho. Em determinado período, percebe ou recebe uma sinalização de que alguns desses registros se afastaram do histórico daquele profissional. Para decidir se a situação merece atenção, precisa compreender quais aspectos mudaram e considerar o contexto antes de realizar qualquer acompanhamento. Uma alteração isolada pode possuir diferentes explicações e, se interpretada sem contexto, pode levar a uma conclusão inadequada.

## 4.6 Que evidência existe hoje?

| Evidência/fonte | O que sustenta | Limitação |
|---|---|---|
| [F] Scholze & Hecker (2023) [1]	| Sustenta que a digitalização do trabalho introduz novas demandas e modifica a forma como atividades e interações profissionais acontecem, contribuindo para o contexto em que gestores precisam acompanhar equipes mediadas por recursos digitais. |	Não investiga diretamente como gestores identificam mudanças individuais na rotina dos colaboradores. |
| [F] Handke et al. (2024) [2] |	Sustenta as mudanças trazidas pelo trabalho híbrido para a colaboração e o funcionamento das equipes, reforçando que o acompanhamento ocorre em um contexto que combina interações presenciais e digitais.	| Discute o trabalho híbrido e a dinâmica das equipes de forma ampla, sem detalhar quais informações os gestores utilizam no acompanhamento cotidiano. |
| [F] Lütjens & Felfe (2026) [3] |	Sustenta a relevância da comunicação informal em equipes híbridas e como sua ocorrência pode variar conforme o contexto de trabalho, reforçando a importância das interações para compreender a dinâmica da equipe. |	Não analisa especificamente a percepção do gestor sobre mudanças de padrão nem o cruzamento dessas interações com registros de tarefas. |

---

# 5. Entendendo o contexto de uso

## 5.1 Onde e em quais situações a interação poderia ocorrer?

[H] H20 - A interação com o WorkSense poderá ocorrer em contexto corporativo, presencial ou remoto, principalmente durante momentos de acompanhamento da equipe, como revisões periódicas, preparação para reuniões individuais, acompanhamento de prazos ou análise de uma sinalização específica.

## 5.2 Em quais dispositivos/equipamentos?

[H] H21 - O computador ou notebook tende a ser o dispositivo principal para o acompanhamento detalhado dos colaboradores, enquanto dispositivos móveis podem ser úteis para consultas breves ou notificações.

## 5.3 Existem condições físicas relevantes?

[H] H22 - O gestor pode utilizar a interface em situações com interrupções ou restrição de tempo e, por lidar com informações relacionadas aos colaboradores, pode precisar de condições que preservem a privacidade visual durante a consulta.

## 5.4 Existem fatores sociais ou organizacionais?

[H] H23 - Relações hierárquicas, responsabilidade do gestor, confiança da equipe, níveis de permissão e políticas organizacionais podem influenciar como o WorkSense é utilizado e como suas sinalizações são interpretadas. O acesso às informações também deverá respeitar a finalidade definida para seu uso.

[F] F03 - O tratamento de dados relacionados a pessoas está sujeito a princípios de finalidade, necessidade, transparência e segurança, considerados pelo TCC a partir da LGPD e das diretrizes de IA confiável.

## 5.5 Existe necessidade de histórico, rastreabilidade ou auditoria?

[H03] O histórico individual é necessário para que o WorkSense compare períodos e sinalize alterações em relação ao padrão anterior do próprio perfil.

[H] H24 - Para interpretar adequadamente uma sinalização, o gestor pode precisar consultar seu período de referência, os indicadores que contribuíram para o resultado e informações sobre quando a análise foi realizada.

## 5.6 Um erro pode produzir consequência relevante? Qual?

[H] H25 - Uma interpretação incorreta das sinalizações pode afetar a forma como o gestor acompanha um colaborador e gerar impactos sobre privacidade, confiança e relações de trabalho. Por isso, a apresentação dos resultados deve deixar claros seus limites e evitar interpretações diagnósticas ou punitivas.

---

# 6. Entendendo mercado e alternativas existentes

> Nesta entrega faça apenas um **levantamento inicial**. A análise aprofundada ocorre na Entrega 2.

## 6.1 Como pessoas resolvem problemas semelhantes hoje?

| Alternativa atual | Quem usa | Para quê | Status/evidência |
|---|---|---|---|
| Conversas, reuniões e observação cotidiana | Gestores e equipes | Compreender dificuldades e acompanhar o trabalho | [H] H18; processo atual ainda precisa ser investigado |
| Telegram, Teams, Slack ou e-mail | Equipes | Comunicação e registro de interações | [F] Classe de ferramentas existente; Telegram integra o TCC |
| Trello e outros quadros Kanban | Equipes e gestores | Organizar tarefas, prazos e responsáveis | [F] Trello utilizado no TCC |
| Planilhas, relatórios e scripts | Pesquisadores/analistas | Consolidar dados e calcular indicadores | [F] Processo experimental atual do TCC |
| Microsoft Viva Insights | Gestores, líderes e analistas | Analisar padrões de colaboração, produtividade e bem-estar |  [F] documentação oficial da Microsoft (https://learn.microsoft.com/en-us/viva/insights/introduction) |
| ActivTrak | Gestores e líderes | Acompanhar produtividade, carga de trabalho e tendências | [F] documentação oficial do ActivTrak (https://support.activtrak.com/hc/en-us/articles/18821721976475-Organization-Overview) |
| Worklytics | Lideranças, RH e People Analytics | Integrar métricas de colaboração e trabalho com foco em privacidade | [F] documentação oficial do Worklytics (https://www.worklytics.co/workplace-insights-dashboard) |
| Workday Peakon Employee Voice | Gestores, RH e colaboradores | Coletar feedback, acompanhar sentimento, prioridades e planos de ação | [F] documentação oficial do Workday(https://www.workday.com/en-us/products/employee-voice/overview.html) |

## 6.2 Existem produtos que atuam na mesma área, mesmo sem serem equivalentes ao TCC?

[F] F04 - Existem soluções que atuam em áreas próximas ao WorkSense, como Microsoft Viva Insights, ActivTrak, Worklytics e Workday Peakon Employee Voice, abrangendo workplace analytics, colaboração, produtividade, carga de trabalho e escuta de colaboradores. Essas soluções não são equivalentes ao WorkSense, mas apresentam capacidades e contextos de uso relacionados.

## 6.3 Quais interfaces profissionais esse público já conhece?

[H] H26 - Gestores podem estar familiarizados com interfaces profissionais como dashboards, relatórios, planilhas, ferramentas de comunicação, calendários e quadros Kanban, enquanto perfis com maior atuação analítica podem também utilizar ferramentas de BI e visualização de dados.

## 6.4 O que essas soluções parecem fazer bem?

[F] F05 - As soluções analisadas apresentam recursos para organizar indicadores, visualizar tendências e comparar informações ao longo do tempo, além de permitir diferentes níveis de aprofundamento. Também foram observados mecanismos relacionados a controle de acesso e privacidade, como separação por papéis no Viva Insights e agregação/anonimização de dados no Worklytics.

## 6.5 O que parecem fazer mal, dificultar ou não atender?

[H] H27 - Interfaces que concentram grande quantidade de métricas podem aumentar a dificuldade de interpretação para gestores com menor familiaridade com análise de dados.

[H] H28 - Soluções percebidas como mecanismos de monitoramento individual podem gerar preocupações relacionadas a vigilância, privacidade e confiança.

[?] ?02 - Ainda não sabemos se alguma solução existente combina de forma semelhante ao WorkSense análise comunicacional, registros de tarefas, comparação com baseline individual, scores comunicacional e profissional separados e explicação dos indicadores que contribuíram para uma sinalização.

## 6.6 Que padrões de interface ou vocabulário parecem familiares a esse público?

Gestores podem já ter contato com padrões comuns em ferramentas profissionais, como dashboards, indicadores resumidos, filtros, gráficos de tendência, comparações históricas, tabelas e detalhamento de informações. Ferramentas como planilhas, calendários, sistemas administrativos, canais de comunicação e quadros Kanban também podem influenciar suas expectativas sobre organização e navegação.

[F] F06 - Nas soluções profissionais analisadas aparecem padrões como dashboards, indicadores resumidos, tendências temporais, comparações históricas, detalhamento progressivo e diferentes níveis de acesso conforme o papel do usuário.

[H26] A familiaridade dos gestores com esses tipos de interface e ferramentas ainda precisa ser investigada.

[?] ?03 - Ainda não sabemos quais termos são mais compreensíveis para gestores ao apresentar conceitos como baseline, score, variação e sinalização.

---

# 7. Derivando o escopo de IHC da disciplina

## 7.1 Escolha o caminho do projeto

### Caminho A — TCC já possui interface

Explique qual parte da interface será usada como recorte da disciplina e por que esse fluxo é relevante.

[H05] Para a disciplina de IHC, o recorte será a interface destinada ao gestor ou líder de equipe. Ela permitirá cadastrar e vincular colaboradores ao WorkSense e, principalmente, acompanhar os resultados produzidos pela ferramenta, consultando scores comunicacionais e profissionais, sinalizações, variações em relação ao histórico individual e os indicadores que contribuíram para cada resultado.

O fluxo de acompanhamento e interpretação das sinalizações será priorizado, pois está diretamente relacionado à contribuição central do TCC e envolve decisões importantes de IHC, como apresentar informações complexas de forma compreensível, evitar interpretações punitivas ou definitivas e fornecer contexto suficiente para apoiar a decisão humana. O cadastro e vínculo dos colaboradores será considerado um fluxo de apoio necessário para permitir esse acompanhamento.

## 7.2 Qual perfil será priorizado no projeto de IHC?

Gestor ou líder de equipe.

**Por que esse perfil foi escolhido?** 
[H05] O gestor foi escolhido por ser o usuário responsável por acompanhar os resultados produzidos pelo WorkSense e interpretar as sinalizações antes de qualquer ação relacionada ao colaborador. É para esse perfil que a interface deverá organizar os scores, suas variações e os indicadores associados, oferecendo informações suficientes para uma interpretação contextualizada.

## 7.3 Qual objetivo desse usuário será priorizado?

[H04] Acompanhar a equipe de forma mais estruturada e preventiva, identificando e compreendendo variações relevantes nos padrões dos colaboradores para decidir quando uma situação merece acompanhamento humano.

## 7.4 Que interface será explorada na disciplina?

Complete:

> **Para fins da disciplina de IHC, será projetada uma interface que permita a `{{perfil}}` utilizar `{{capacidade/resultado do TCC}}` para `{{objetivo}}`, no contexto de `{{situação}}`.**

Para fins da disciplina de IHC, será projetada uma interface que permita ao gestor ou líder de equipe utilizar as sinalizações, scores e indicadores produzidos pelo WorkSense para acompanhar e compreender alterações nos padrões comunicacionais e profissionais dos colaboradores, no contexto do acompanhamento cotidiano de equipes.

[H03]; [H05] A interface deverá permitir o cadastro e vínculo dos colaboradores, a consulta de seus scores comunicacional e profissional, a comparação com o histórico individual e a visualização dos indicadores que contribuíram para eventuais sinalizações. O foco da disciplina estará na forma como essas informações são apresentadas e interpretadas pelo gestor.

## 7.5 Qual é a relação dessa interface com o TCC?

- [ ] Já fazia parte do TCC.
- [ X ] É um aprofundamento de algo parcialmente previsto.
- [ ] É uma extensão conceitual criada para a disciplina.
- [ ] É um protótipo demonstrativo de aplicação potencial.
- [ ] Outra: {{...}}.

> **Declaração:** a interface desenvolvida nesta disciplina é um artefato de aprendizagem de IHC baseado no tema do TCC. Sua inclusão ou implementação no TCC somente ocorrerá se isso for posteriormente decidido pela equipe e pelo orientador.

[H02] O TCC já prevê o vínculo entre usuários, a geração de scores e sinalizações e a apresentação de seus componentes, além de possuir visualizações preliminares dos resultados. Entretanto, ainda não define uma interface de gestão completa, seus fluxos de interação ou requisitos de usabilidade.
O projeto de IHC aprofundará essa parte, projetando especificamente a interação do gestor com o cadastro dos colaboradores e com os resultados produzidos pelo WorkSense.

---

# 8. Levantando possibilidades de interação — sem desenhar ainda

A equipe pode registrar possibilidades para investigação. **Não significa que todas serão implementadas.**

Marque apenas as que parecem plausíveis e explique o objetivo correspondente.

| Possibilidade | Pode fazer sentido? | Objetivo/tarefa que justificaria | Evidência atual |
|---|---|---|---|
| Dashboard/visão geral | Sim | Obter uma visão geral da equipe e identificar colaboradores ou sinalizações que mereçam análise mais detalhada | [H] H04, H05; alinhado ao objetivo de acompanhamento do gestor |
| Relatório/resultados | Sim | Compreender o que mudou em determinado perfil, em qual período e quais indicadores contribuíram para o resultado | [H] H03, H04, H24; [F] F02 |
| Histórico com busca/filtros | Sim | Consultar períodos e sinalizações anteriores de um colaborador e acompanhar sua evolução ao longo do tempo | [H] H03, H24 |
| Comparação com o baseline | Sim | Comparar o período analisado com o histórico individual do próprio colaborador | [H] H03; comparação temporal faz parte da contribuição proposta |
| Explicabilidade/detalhamento dos indicadores | Sim | Entender quais componentes comunicacionais ou profissionais contribuíram para um score ou sinalização | [F] requisito não funcional do TCC; [F] F02 |
| Alertas/sinalizações | Sim | Direcionar a atenção do gestor para uma variação que possa merecer análise | [H] H03, H04; sinalizações fazem parte da contribuição proposta |
| Cadastro de colaboradores | Sim | Cadastrar os perfis que serão acompanhados, assim realizando vinculação às fontes necessárias para associação dos registros | [H] H05; faz parte do recorte definido para a interface |
| Ajuda/documentação | Sim | Ajudar o gestor a compreender scores, indicadores, limites de interpretação e significado das sinalizações | [H] H10; [F] F02 |
| Configuração/parametrização técnica	| Não, inicialmente |	Poderia permitir alteração de períodos, thresholds ou outras regras do processamento	| [H] H08, H13; parece pertencer ao administrador e não ao fluxo principal do gestor |
| Entrada/seleção/preparação de dados	| Não, inicialmente	| Poderia permitir importar datasets ou selecionar fontes para processamento	| [H] H09, H14; pertence principalmente ao processo experimental, não à atividade do gestor |
| Execução / acompanhamento do processamento	| Não, inicialmente	| Poderia permitir iniciar análises ou acompanhar execução do pipeline |	Não foi identificada uma necessidade do gestor de controlar diretamente o processamento |
| Relatórios / exportação | Talvez | Exportar ou compartilhar resultados de uma análise quando houver necessidade organizacional |	[?] PENDENTE; ainda não sabemos se essa tarefa é necessária |
| Administração global | Não, inicialmente | Manter integrações, parâmetros globais, credenciais e configurações técnicas |	[H] H08, H13; pertence ao perfil administrador |
| Auditoria/logs técnicos	| Não, inicialmente	| Consultar registros técnicos de execução ou falhas | Auditoria técnica é requisito do TCC, mas não foi identificada como tarefa do gestor |

> **Atenção:** “login + dashboard + CRUD” não é uma solução universal. Cada padrão deve surgir de uma tarefa real.

---

# 9. Benefícios e ações iniciais

## 9.1 Qual benefício concreto o projeto de IHC pretende oferecer?

| Benefício esperado | Problema/necessidade | Usuário | Status/evidência |
|---|---|---|---|
| Apoiar um acompanhamento mais estruturado e preventivo da equipe | Mudanças relevantes na rotina profissional podem ocorrer gradualmente e passar despercebidas no acompanhamento cotidiano | Gestor | [F] F01; [H] H04 |
| Dar ao gestor melhores condições para decidir quando um colaborador pode precisar de acompanhamento | O gestor precisa perceber e compreender variações antes de decidir se alguma ação humana é necessária | Gestor | [H] H04 |
| Favorecer uma análise mais contextualizada de cada colaborador ao longo do tempo |	Observações e indicadores isolados podem admitir diferentes interpretações e não representam, sozinhos, a situação do colaborador |	Gestor e colaborador afetado |	[F] F02; [H] H03 |
| Aproximar os resultados técnicos do WorkSense da atividade real de gestão |	O TCC produz scores, indicadores e sinalizações, mas ainda não possui uma interface gerencial estruturada para que esses resultados sejam utilizados pelo gestor |	Gestor |	[H] H02; [H] H05 |

## 9.2 Que ações o usuário deverá conseguir realizar?

| ID | O usuário precisa conseguir... | Para alcançar... | Prioridade inicial |
|---|---|---|---|
| T01 | Visualizar os colaboradores acompanhados e suas sinalizações recentes | Identificar situações que possam merecer análise | Alta |
| T02 | Selecionar um colaborador e consultar seus resultados | Analisar uma situação específica | Alta |
| T03 | Distinguir score comunicacional e profissional | Identificar em qual dimensão ocorreu maior variação | Alta |
| T04 | Comparar o período analisado com o baseline individual | Compreender a mudança em relação ao histórico do próprio colaborador | Alta |
| T05 | Consultar os indicadores que contribuíram para um score ou sinalização | Entender por que aquela variação foi apresentada | Alta |
| T06 | Consultar períodos e sinalizações anteriores | Acompanhar a evolução do perfil ao longo do tempo | Média |
| T07 | Cadastrar e vincular colaboradores | Definir quais perfis poderão ser acompanhados pela ferramenta | Alta |
| T08 | Acessar explicações sobre métricas, sinalizações e limites de interpretação | Interpretar os resultados de forma adequada | Média |
| T09 | Consultar informações sobre o período e atualização da análise | Entender a que dados o resultado apresentado se refere | Média |
| T10 | Exportar ou compartilhar resultados | Compartilhar uma análise quando houver necessidade autorizada | Baixa / PENDENTE |

## 9.3 Tecnologias/restrições já definidas no TCC

A tecnologia aparece **agora**, depois do entendimento do uso.

| Tecnologia/restrição | Por que existe | Possível impacto na interação |
|---|---|---|
| Telegram | Canal previsto para interação comunicacional associada aos perfis | A interface gerencial deverá permitir identificar corretamente quais usuários estão vinculados aos perfis acompanhados |
| Trello | Fonte dos registros profissionais relacionados às tarefas | Informações sobre tarefas, prazos, conclusões e reaberturas poderão aparecer no detalhamento dos indicadores profissionais |
| n8n | Orquestra as integrações entre os componentes da solução | Estados de falha ou desatualização do fluxo não devem ser confundidos com resultados da análise, caso essas informações sejam apresentadas ao gestor |
| PostgreSQL | Mantém vínculos e registros operacionais utilizados pelo fluxo | O cadastro e vínculo dos colaboradores deve considerar as associações necessárias entre os usuários e as fontes utilizadaso |
| Ollama e modelo conversacional | Responsáveis pela interação do agente conversacional | O papel do agente deve permanecer separado dos resultados analíticos, evitando sugerir que o modelo conversacional calcula ou avalia os scores |
| Módulos de PLN e análise | Extraem os indicadores comunicacionais e profissionais | Os resultados técnicos precisam ser apresentados em uma forma compreensível para o gestor, sem exigir conhecimento dos algoritmos utilizados |
| Baseline de 30 dias e reanálise de 15 dias | Estruturam a comparação temporal atualmente prevista no TCC | A interface deve deixar clara a relação entre período de referência e período analisado, evitando comparação direta entre colaboradores |
| Score comunicacional e score profissional separados | Mantêm independentes dimensões de naturezas diferentes | A interface deve preservar a distinção entre os dois resultados e seus respectivos componentes |
| Origem da base experimental ainda em definição | A equipe ainda avalia o uso de dados simulados, reais ou provenientes de uma base existente | [?] ?01 — a decisão poderá alterar requisitos de privacidade, consentimento, apresentação e tratamento dos dados |
| Sem finalidade diagnóstica, punitiva ou decisão automatizada | Delimitação ética e metodológica do WorkSense | Linguagem, explicações e fluxo de análise devem reforçar que as sinalizações apoiam a interpretação humana e não constituem conclusões definitivas |

---

# 10. Hipóteses e dúvidas prioritárias

| ID | Hipótese/dúvida | Por que importa | Como poderá ser investigada |
|---|---|---|---|
| H01 | O TCC prevê o desenvolvimento e a avaliação experimental do WorkSense, com processamento de registros comunicacionais e profissionais, extração de indicadores, cálculo separado dos scores e comparação temporal com baseline individual. | Delimita o que pertence ao TCC e quais capacidades técnicas podem dar origem ao recorte de IHC. | {Entrega ...} |
| H02 | O TCC já prevê o vínculo entre usuários, a geração de scores e sinalizações e a apresentação de seus componentes, além de possuir visualizações preliminares dos resultados. Entretanto, ainda não define uma interface de gestão completa, seus fluxos de interação ou requisitos específicos de usabilidade. | Justifica o aprofundamento da interação do gestor no projeto de IHC sem ignorar os requisitos funcionais e não funcionais já definidos para o WorkSense. | {Entrega ...} |
| H03 | O WorkSense pode apoiar a identificação de alterações ao longo do tempo nos padrões de comunicação, interação e execução de tarefas de perfis profissionais, mantendo a interpretação e a decisão sob responsabilidade humana. | Representa a principal capacidade do WorkSense que deverá ser traduzida para uma interação útil e compreensível para o gestor. | {Entrega ...} |
| H04 | A contribuição pode tornar o acompanhamento das equipes mais estruturado e preventivo, auxiliando gestores na identificação e interpretação de variações, favorecendo um acompanhamento mais contextualizado dos colaboradores e apoiando decisões de gestão mais informadas e transparentes, sempre com supervisão humana. | Define o benefício esperado para o gestor e orienta quais tarefas da interface devem receber maior prioridade. | {Entrega ...} |
| H05 | O gestor ou líder de equipe será o usuário direto da interface de IHC, podendo cadastrar e vincular colaboradores, acompanhar seus perfis e consultar scores, sinalizações e indicadores comunicacionais e profissionais. | Delimita o usuário principal e o conjunto inicial de atividades consideradas no recorte da interface. | {Entrega ...} |
| H06 | O colaborador é a pessoa associada ao perfil acompanhado pelo WorkSense, gera registros comunicacionais e profissionais por meio dos canais integrados, mas não utiliza diretamente a interface gerencial. | Distingue o usuário direto da interface da pessoa afetada pelas informações e interpretações produzidas a partir de seus registros. | {Entrega ...} |
| H07 | Profissionais de RH ou gestão de pessoas podem participar como stakeholders relacionados a políticas de uso, transparência, privacidade e limites de interpretação dos resultados, sem necessariamente serem usuários diretos da interface. | Ajuda a identificar responsabilidades organizacionais e possíveis necessidades de governança que podem afetar o projeto. | {Entrega ...} |
| H08 | O administrador da solução pode ser responsável por atividades técnicas como configuração de integrações, acessos, permissões, credenciais e parâmetros necessários ao funcionamento do WorkSense. | Permite separar tarefas administrativas das atividades que realmente pertencem ao fluxo principal do gestor. | {Entrega ...} |
| H09 | A equipe responsável pelo TCC desenvolve, opera e avalia experimentalmente o WorkSense, preparando os dados de avaliação, executando os processamentos, realizando testes e analisando os resultados obtidos. | Diferencia as atividades experimentais e técnicas da equipe do TCC das tarefas que deverão ser realizadas pelo usuário da interface. | {Entrega ...} |
| H10 | Gestores podem apresentar diferentes níveis de familiaridade com métricas, indicadores e ferramentas digitais. | A familiaridade do usuário pode afetar a compreensão dos resultados e o nível de detalhamento adequado para a interface. | {Entrega ...} |
| H11 | Colaboradores possuem padrões distintos de comunicação, interação e uso de ferramentas de trabalho e podem apresentar diferentes percepções ou preocupações sobre a finalidade e o uso de seus dados. | Reforça a necessidade de considerar diferenças individuais e os possíveis efeitos do sistema sobre as pessoas acompanhadas. | {Entrega ...} |
| H12 | Profissionais de RH ou gestão de pessoas podem possuir maior familiaridade com processos de pessoas, privacidade e governança, mas apresentar diferentes níveis de experiência com indicadores quantitativos e ferramentas digitais. | Ajuda a compreender de que forma esse stakeholder poderia participar da governança ou interpretação dos resultados. | {Entrega ...} |
| H13 | Administradores da solução precisam de maior familiaridade técnica com integrações, acessos, permissões e configurações necessárias à implantação e manutenção do WorkSense. | Ajuda a distinguir necessidades técnicas de administração das necessidades de interação do gestor. | {Entrega ...} |
| H14 | A equipe responsável pelo TCC precisa de maior nível de detalhe sobre indicadores, componentes dos scores e processamento dos dados para realizar testes, avaliar os resultados e identificar erros. | Diferencia as necessidades de análise técnica da equipe do TCC das informações que precisam ser apresentadas ao gestor. | {Entrega ...} |
| H15 | Gestores organizam e acompanham continuamente as atividades da equipe por meio de informações como responsáveis, andamento e prazos. | Ajuda a compreender quais atividades fazem parte da rotina do gestor e quais informações podem ser relevantes para o acompanhamento. | {Entrega ...} |
| H16 | A execução e atualização das tarefas constituem uma atividade frequente dos colaboradores durante sua rotina de trabalho. | Ajuda a entender como os registros profissionais utilizados pelo WorkSense são produzidos no cotidiano. | {Entrega ...} |
| H17 | A interpretação das sinalizações pelo gestor parece ser uma das atividades mais críticas, pois uma interpretação inadequada pode atribuir significado incorreto a uma variação ou levar a uma ação de acompanhamento sem contexto suficiente. Por isso, os resultados precisam ser apresentados com seus indicadores e permanecer sujeitos à análise humana. | Define um fluxo central de IHC e envolve consequências sobre pessoas caso o resultado seja interpretado inadequadamente. | {Entrega ...} |
| H18 | Atualmente, o gestor tende a acompanhar a equipe por meio de diferentes fontes e momentos de contato, como reuniões, conversas presenciais/online e registros em ferramentas de gestão de tarefas, precisando interpretar essas informações durante o acompanhamento cotidiano. | Compreender o processo atual permite projetar uma interface que complemente a atividade do gestor em vez de pressupor um fluxo inexistente. | {Entrega ...} |
| H19 | Para compreender mudanças na rotina de um colaborador, o gestor pode considerar informações como frequência e características das interações, andamento e regularidade das entregas, cumprimento de prazos, ocorrências de retrabalho e mudanças no contexto de trabalho, interpretando essas informações em relação ao histórico daquele profissional. | Ajuda a identificar quais informações realmente apoiam a interpretação do gestor e evita simplesmente reproduzir na interface todas as métricas calculadas pelo sistema. | {Entrega ...} |
| H20 | A interação com o WorkSense poderá ocorrer em contexto corporativo, presencial ou remoto, principalmente durante momentos de acompanhamento da equipe, como revisões periódicas, preparação para reuniões individuais, acompanhamento de prazos ou análise de uma sinalização específica. | O momento e a situação de uso influenciam o nível de detalhe, duração da interação e informações necessárias. | {Entrega ...} |
| H21 | O computador ou notebook tende a ser o dispositivo principal para o acompanhamento detalhado dos colaboradores, enquanto dispositivos móveis podem ser úteis para consultas breves ou notificações. | O dispositivo influencia espaço disponível, densidade das informações e possíveis formas de interação. | {Entrega ...} |
| H22 | O gestor pode utilizar a interface em situações com interrupções ou restrição de tempo e, por lidar com informações relacionadas aos colaboradores, pode precisar de condições que preservem a privacidade visual durante a consulta. | Condições físicas de uso podem afetar atenção, leitura das informações e exposição indevida de dados. | {Entrega ...} |
| H23 | Relações hierárquicas, responsabilidade do gestor, confiança da equipe, níveis de permissão e políticas organizacionais podem influenciar como o WorkSense é utilizado e como suas sinalizações são interpretadas. O acesso às informações também deverá respeitar a finalidade definida para seu uso. | O sistema envolve dados sobre colaboradores e relações de poder, tornando o contexto organizacional relevante para acesso e interpretação. | {Entrega ...} |
| H24 | Para interpretar adequadamente uma sinalização, o gestor pode precisar consultar seu período de referência, os indicadores que contribuíram para o resultado e informações sobre quando a análise foi realizada. | Ajuda a definir qual contexto precisa acompanhar uma sinalização para que ela não seja apresentada como um resultado isolado. | {Entrega ...} |
| H25 | Uma interpretação incorreta das sinalizações pode afetar a forma como o gestor acompanha um colaborador e gerar impactos sobre privacidade, confiança e relações de trabalho. Por isso, a apresentação dos resultados deve deixar claros seus limites e evitar interpretações diagnósticas ou punitivas. | Erros de interpretação podem produzir consequências sobre pessoas e sobre a relação entre gestor e colaborador. | {Entrega ...} |
| H26 | Gestores podem estar familiarizados com interfaces profissionais como dashboards, relatórios, planilhas, ferramentas de comunicação, calendários e quadros Kanban, enquanto perfis com maior atuação analítica podem também utilizar ferramentas de BI e visualização de dados. | A familiaridade prévia pode influenciar expectativas, vocabulário e padrões de interação compreendidos com menor esforço. | {Entrega ...} |
| H27 | Interfaces que concentram grande quantidade de métricas podem aumentar a dificuldade de interpretação para gestores com menor familiaridade com análise de dados. | O WorkSense produz diversos indicadores e pode gerar sobrecarga se todos receberem o mesmo nível de destaque. | {Entrega ...} |
| H28 | Soluções percebidas como mecanismos de monitoramento individual podem gerar preocupações relacionadas a vigilância, privacidade e confiança. | A percepção de vigilância pode afetar aceitação, confiança e uso responsável do sistema. | {Entrega ...} |

Registre em [`../RASTREABILIDADE.md`](../RASTREABILIDADE.md).

---

# 11. Síntese da equipe

| Pergunta | Síntese atual |
|---|---|
| Qual é a contribuição central do TCC? |  Desenvolver o WorkSense para identificar indícios de alterações ao longo do tempo em padrões comunicacionais e profissionais, a partir de indicadores e scores separados comparados ao histórico individual, gerando sinalizações para apoiar a análise humana. |
| O TCC já previa interface? | Parcialmente. O TCC já prevê interação com o WorkSense por meio do agente conversacional e contempla vínculo de usuários, geração de scores e sinalizações, apresentação de seus componentes e visualizações preliminares. Porém, não havia sido projetada uma interface gerencial completa para apoiar o uso e a interpretação desses resultados pelo gestor. |
| Quem é o usuário prioritário de IHC? | [H] Gestor ou líder de equipe. |
| O que ele precisa alcançar? | [H] Acompanhar a equipe de forma mais estruturada, perceber mudanças relevantes na rotina de cada colaborador e compreender essas variações em relação ao seu histórico e contexto para decidir quando é necessário aprofundar o acompanhamento humano. |
| Qual problema/atividade será estudado? | [H] A O acompanhamento e a interpretação, pelo gestor, de mudanças nos padrões comunicacionais e profissionais dos colaboradores, especialmente quando uma sinalização indica uma variação que pode merecer atenção. |
| Como isso acontece hoje? | [H] O gestor tende a acompanhar a equipe por diferentes momentos e fontes de informação, como reuniões, conversas e registros em ferramentas de gestão de tarefas, interpretando essas informações durante sua rotina de acompanhamento. |
| Qual é o contexto de uso? |  [H] Ambiente corporativo presencial ou remoto, em situações de acompanhamento periódico da equipe ou quando uma situação específica leva o gestor a consultar mais detalhadamente um colaborador. |
| Que interface/recorte será explorado? | Uma interface gerencial que permita cadastrar e vincular colaboradores, obter uma visão geral da equipe, identificar sinalizações que mereçam atenção e aprofundar a análise de um perfil por meio dos scores comunicacional e profissional, histórico individual, comparação temporal e indicadores relacionados. |
| Como a interface se relaciona ao TCC? | É um aprofundamento de algo parcialmente previsto no TCC. O projeto de IHC utiliza capacidades já propostas pelo WorkSense e aprofunda especificamente a interação do gestor com o cadastro dos colaboradores e com os resultados produzidos pela ferramenta. |
| Quais pontos ainda são hipóteses? | Permanecem em investigação as características e práticas dos usuários e stakeholders, o processo atual de acompanhamento, as informações consideradas relevantes pelo gestor, o contexto e os dispositivos de uso, os riscos de interpretação, a familiaridade com métricas e padrões de interface e outras hipóteses registradas de H01 a H28. Também permanecem abertas as dúvidas ?01, ?02 e ?03. |

### Delimitação

**Dentro do escopo de IHC:** compreender o contexto em que gestores acompanham mudanças nos colaboradores e projetar uma interface que apresente de forma explícita os resultados produzidos pelo WorkSense, preservando a separação entre os scores comunicacional e profissional, a comparação com o histórico individual e os indicadores que contribuíram para cada resultado.
**Fora do escopo de IHC:** redesenhar toda a interação pelo Telegram; definir ou alterar os algoritmos de PLN e as fórmulas dos scores; projetar todos os módulos administrativos do WorkSense; validar políticas organizacionais de uso; ou avaliar se a ferramenta melhora efetivamente a gestão de equipes em um ambiente organizacional real.
**Dentro do escopo formal do TCC:** desenvolver e avaliar experimentalmente o pipeline do WorkSense, incluindo integrações, processamento dos registros comunicacionais e profissionais, extração de indicadores, cálculo separado dos scores, comparação com baseline individual e geração de sinalizações. A avaliação busca verificar se os indicadores e scores produzidos respondem de forma coerente às alterações presentes nos dados e tornar explícitos os componentes que contribuíram para os resultados. 
**Interface da disciplina será implementada no TCC?** Não definido.

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

1. **Problema/atividade humana:** Em equipes que atuam entre contextos presenciais e remotos, gestores podem ter mais dificuldade para perceber e acompanhar mudanças sutis que ocorrem ao longo do tempo na comunicação, interação e execução das atividades dos colaboradores.
2. **Contribuição técnica do TCC:** O WorkSense processa registros comunicacionais e profissionais, extrai indicadores, calcula scores separados e compara os resultados com o histórico individual para identificar possíveis alterações de padrão.
3. **Como uma pessoa poderia utilizar essa contribuição:** Um gestor poderia consultar essas sinalizações, scores e indicadores para apoiar o acompanhamento dos colaboradores e decidir quando uma situação merece análise mais detalhada.

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
