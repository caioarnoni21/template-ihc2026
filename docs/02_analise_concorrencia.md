# Entrega 2 — Público-alvo e análise de concorrência

**Data:** {{26/08/2026}}  
**Status:** 🟩 concluída
**Responsabilidade mínima:** cada integrante analisa pelo menos 1 concorrente/interface representativa; a equipe produz síntese comparativa.

## Objetivo da atividade

Compreender soluções do mesmo domínio **e também interfaces familiares ao público-alvo**. O objetivo não é copiar telas, mas identificar convenções, padrões, affordances percebidas, problemas recorrentes, expectativas e oportunidades de design.

> **Concorrente não precisa ser idêntico ao produto.** Pode atuar na mesma área, resolver objetivo semelhante ou disputar a mesma necessidade. Quando não houver concorrente direto, use produtos análogos e softwares que o público já utiliza.

### Para TCCs que não previam interface

Não procure apenas um “concorrente do algoritmo”. Investigue **interfaces profissionais que materializam atividades semelhantes** às que o usuário escolhido precisaria realizar.

Exemplos:

- TCC de banco de dados → consoles de administração, ferramentas para DBA, monitoramento e análise de consultas;
- TCC de LLM/ML → painéis de experimentos, gestão de modelos/datasets, comparação de métricas, revisão de resultados;
- TCC de análise de dados → dashboards, ferramentas de BI, filtros, relatórios e exploração;
- TCC de infraestrutura/API → portais administrativos, observabilidade, logs, gestão de credenciais e uso;
- TCC de cibersegurança → consoles de alertas, triagem, histórico e auditoria.

A pergunta é: **“que convenções esse perfil já conhece para executar tarefas equivalentes?”**

## Entrada obrigatória da Entrega 1

Retome o mapa inicial de alternativas e produtos citado na Entrega 1. Aqui a equipe deixa de trabalhar apenas com impressão inicial e passa a **investigar sistematicamente** cada solução.

| Item citado na Entrega 1 | Tipo | Por que foi citado | Status inicial | Decisão nesta entrega |
|---|---|---|---|---|
| Microsoft Viva Insights | concorrente  | É uma ferramente que usa dados para melhorar o bem-estar e a produtividade no trabalho | [F] documentação oficial da Microsoft (https://learn.microsoft.com/en-us/viva/insights/introduction) | analisar|
| ActivTrak | concorrente  | é uma plataforma em nuvem de monitoramento de funcionários e análise de produtividade projetada para equipes presenciais, remotas ou híbridas | [F] documentação oficial do ActivTrak (https://support.activtrak.com/hc/en-us/articles/18821721976475-Organization-Overview) | analisar|
| Worklytics | concorrente  | é uma plataforma de People Analytics e análise de local de trabalho (workplace analytics) baseada em Inteligência Artificial | [F] documentação oficial do Worklytics (https://www.worklytics.co/workplace-insights-dashboard) | analisar|
| Workday Peakon Employee Voice | concorrente  | é uma plataforma de escuta de funcionários impulsionada por inteligência artificial que mede o engajamento, o bem-estar e o sentimento no ambiente de trabalho | [F] documentação oficial do Workday(https://www.workday.com/en-us/products/employee-voice/overview.html) | analisar|

Se uma hipótese da Entrega 1 for confirmada ou refutada durante esta análise, atualize `H01`, `H02`... em [`../RASTREABILIDADE.md`](../RASTREABILIDADE.md).

## 1. Público-alvo desta análise

O publico alvo é os gestores

## 2. Concorrentes diretos/indiretos

### Análise C01 — Microsoft Viva Insights

**Autor(a):** Caio Arnoni — 22.221.019-7  
**Tipo:** direto 
**Link oficial:** https://learn.microsoft.com/en-us/viva/insights/introduction  
**Data de acesso:** 26/08/2026

#### Contexto e proposta

O Viva Insights ajuda pessoas e empresas a prosperarem com insights baseados em dados e protegidos pela privacidade, além de oferecer recomendações para melhorar a produtividade e o bem-estar. A proposta dele é fornecer insights pessoais para seus funcionários, insights de equipe para gerentes, insights organizacionais para seus gerentes e líderes de negócios

#### Funcionalidades relevantes

| Funcionalidade | Como é realizada | Evidência/print | Observação de IHC |
|---|---|---|---|
| Análise de Rede Organizacional | O Viva Insights utiliza dados agregados de colaboração do Microsoft 365, como reuniões, e-mails, calendário e chats. A interface representa equipes como nós e suas relações como conexões, permitindo filtrar grupos, segmentar dados, alternar entre grafo e matriz e comparar períodos anteriores e posteriores a uma mudança organizacional. | <img width="1275" height="1650" alt="image" src="https://github.com/user-attachments/assets/5f466ce3-af91-4af6-bc32-d7a41435be87" /> | A comparação lado a lado reduz a necessidade de o usuário memorizar resultados de telas diferentes. Filtros, legendas e detalhamento ajudam na exploração. Porém, o grafo pode ficar visualmente carregado e depende bastante de cores, exigindo rótulos, explicações textuais e formas alternativas de apresentar os resultados. |

#### Experiência do usuário e opiniões

Na pagina do G2, o Viva Insights possuia nota 4,5/5 em 43 avaliacoes. O resumo agregado destaca integracao com Microsoft 365, produtividade, bem-estar e agendamento de tempo de foco como pontos valorizados; tambem registra relatos de perda de acompanhamento de algumas pendencias.

#### Preço/modelo de negócio

A pagina oficial apresentava o Viva Insights por **US$ 4 por usuario/mes**, com pagamento anual, e o pacote Workplace Analytics and Employee Feedback por **US$ 6 por usuario/mes**. A elegibilidade depende de licenca Microsoft 365/Office 365 compativel.

#### Padrões e tendências percebidos

- dashboard e biblioteca de relatorios por papel;
- filtros de periodo, grupo e atributo organizacional;
- comparacao antes/depois;
- alternancia entre grafo, matriz e visualizacoes quantitativas;
- legenda persistente e detalhamento progressivo;
- agregacao e limite minimo de grupo;
- exportacao/publicacao de resultados para outros atores.

#### Pontos positivos, limitações e lições

| Ponto | Evidência | Implicação para nosso projeto |
|---|---|---|
| Positivo: comparacao temporal explicita | Figura C01 | Comparar baseline e periodo recente lado a lado |
| Positivo: multiplas representacoes | Grafo e matriz oficiais | Oferecer resumo simples e aprofundamento opcional |
| Positivo: privacidade incorporada | Documentacao oficial | Definir limiares, papeis e protecao antes de exibir dados |
| Limitacao: alta densidade visual | Figura C01 | Priorizar poucos indicadores na visao inicial |
| Limitacao: dependencia de cor e legenda | Arestas verdes/roxas e nos segmentados | Repetir significado com texto, icone, rotulo ou padrao visual |
| Limitacao: dependencia do ecossistema Microsoft | Licenciamento e fontes de dados | Manter o WorkSense independente de um unico fornecedor |


### Análise C02 — ActivTrak

**Autor(a):** Guilherme Matias — 22.122.071-8  
**Tipo:** direto <br>
**Link oficial:** https://www.activtrak.com/product/executive-insights/ <br>
**Data de acesso:** 03/09/2026

#### Contexto e proposta

O ActivTrak é uma plataforma em nuvem de monitoramento de funcionários e análise de produtividade, voltada a equipes presenciais, remotas ou híbridas. É posicionada como uma plataforma de workforce analytics que ajuda líderes a entender como as equipes de fato usam seu tempo, onde a produtividade trava e onde o risco de burnout está crescendo, diferenciando-se de ferramentas de vigilância pura por não fazer captura de tela constante nem registro de teclas. O sistema não registra teclas digitadas, não usa a câmera nem grava vídeos, focando em coletar dados de uso de aplicativos e sites de forma automática e silenciosa em segundo plano. A proposta central é transformar dados de atividade em dashboards e relatórios que apoiem decisões de gestão de produtividade, e não em um processo aberto de vigilância granular

#### Funcionalidades relevantes

| Funcionalidade | Como é realizada | Evidência/print | Observação de IHC |
|---|---|---|---|
Alocação de Tempo por Categoria e Aplicativo| O ActivTrak classifica o tempo em categorias (Business App, Productivity, Office, etc.) num gráfico de rosca, mostra a variação percentual entre períodos numa tabela e lista os aplicativos mais usados em um ranking de barras.| <img width="728" height="532" alt="image" src="https://github.com/user-attachments/assets/94129834-6cad-4125-b9bd-ef1c43453ec5" /> |A interface é voltada à análise gerencial, priorizando indicadores consolidados em vez de informações detalhadas de cada atividade. Essa abordagem facilita uma visão geral da produtividade, mas pode dificultar a compreensão do motivo das alterações apresentadas, exigindo que o usuário navegue ou analise outros dados para encontrar possíveis causas.

#### Experiência do usuário e opiniões

Na página do Capterra, o ActivTrak possui nota 4,5/5 em 587 avaliações. O resumo agregado destaca facilidade de uso, navegação intuitiva e qualidade dos insights de produtividade como pontos valorizados; também registra relatos frequentes de lentidão, travamentos e monitoramento em tempo real pouco confiável.

#### Preço/modelo de negócio

A página oficial apresenta os planos Essentials por US$ 10 por usuário/mês, Essentials Plus por US$ 15 por usuário/mês e Professional por US$ 19 por usuário/mês, além de um plano gratuito para até 3 usuários (com 30 dias de histórico de dados) e um plano Enterprise sob consulta. A contratação não depende de licença de nenhum outro produto.

#### Padrões e tendências percebidos

* dashboard com abas separadas por tipo de dado (categoria, aplicativo, produtividade);
* comparação de variação percentual entre período de referência e período atual;
* ranking por volume/tempo (aplicativos, categorias);
* pontuação agregada (Productivity Score) para benchmarking;
* indicador de risco (Burnout Risk) como sinalização preventiva;
* sugestões geradas por IA (ActivTrak Coach) em vez de dashboard cru;
* captura de dados automática e contínua, sem intervenção do usuário monitorado.

#### Pontos positivos, limitações e lições

| Ponto | Evidência | Implicação para nosso projeto |
|---|---|---|
| Positivo: visão geral da produtividade | Dashboard de Category Allocation | Apresentar ao gestor uma visão resumida da distribuição do tempo e das atividades |
| Positivo: comparação entre períodos | Top Changes in Category Allocation | Permitir comparar o comportamento atual com um período de referência para identificar desvios |
| Positivo: múltiplas representações | Gráfico de rosca, tabela e gráficos de barras | Utilizar diferentes formas de visualização conforme o tipo de informação apresentada |
| Positivo: categorização automática | Categorias de aplicativos e sites | Classificar as atividades dos usuários para facilitar a identificação de padrões |
| Limitação: alta densidade visual | Dashboard apresenta gráficos, tabelas e diversos indicadores simultaneamente | Priorizar poucos indicadores na visão inicial e permitir o aprofundamento conforme a necessidade |
| Limitação: comparação de categorias pouco intuitiva | Gráfico de rosca com várias categorias próximas | Utilizar gráficos mais adequados para comparação direta entre categorias |
| Limitação: pouca contextualização dos desvios | Alterações são apresentadas principalmente por valores e percentuais | Relacionar o desvio identificado às tarefas ou atividades que podem ter contribuído para sua ocorrência |
| Limitação: foco no monitoramento de atividades | Dados de aplicativos e sites são o principal elemento analisado | Priorizar a análise de tarefas e desvios no WorkSense, evitando transformar o sistema em uma ferramenta de vigilância |


### Análise C03 — Worklytics

**Autor(a):** Guilherme Matias — 22.122.071-8  
**Tipo:** direto <br>
**Link oficial:** https://www.worklytics.co/workplace-insights-dashboard <br>
**Data de acesso:** 08/09/2026

#### Contexto e proposta

O Worklytics é uma plataforma de workplace analytics voltada à análise de como o trabalho acontece dentro das organizações. A plataforma coleta dados de ferramentas corporativas utilizadas pelas equipes, como Google Workspace, Microsoft 365, Slack, Zoom e GitHub, e transforma esses dados em métricas sobre colaboração, reuniões, comunicação, foco, carga de trabalho e outros aspectos da experiência profissional.

#### Funcionalidades relevantes

| Funcionalidade | Como é realizada | Evidência/print | Observação de IHC |
|---|---|---|---|
Análise de reuniões| Analisa dados de calendário para identificar tempo gasto em reuniões, frequência, duração, sobrecarga e indicadores de efetividade das reuniões.| <img width="1438" height="749" alt="image" src="https://github.com/user-attachments/assets/2f1d2130-16ff-4411-b517-f1d281ec2451" />|A informação transforma uma grande quantidade de eventos de calendário em indicadores mais fáceis de interpretar, permitindo identificar rapidamente possíveis problemas relacionados ao excesso ou à baixa efetividade de reuniões.

#### Experiência do usuário e opiniões

A experiência do Worklytics é bastante orientada a dashboards analíticos, nos quais o usuário pode explorar métricas, aplicar filtros e comparar diferentes grupos ou períodos. O novo Workplace Insights Dashboard foi desenvolvido justamente para transformar dados provenientes de calendário, e-mail, Slack, documentos, código e outras fontes em visualizações que permitam responder perguntas sobre como as equipes estão trabalhando.

#### Preço/modelo de negócio

O plano Free é gratuito e permite até 100 usuários, utilizando apenas dados de calendário, com histórico de 30 dias e acesso a indicadores básicos de reuniões, foco e colaboração.
O plano Business começa em US$ 2.500 por mês, inclui até 200 usuários e permite adicionar integrações, visibilidade organizacional, indicadores de adoção de IA, histórico de até três meses, benchmarks básicos e mais de 200 métricas pré-configuradas de colaboração. Usuários adicionais custam US$ 10 por usuário/mês.

#### Padrões e tendências percebidos

* Dashboards orientados à análise organizacional, em vez de monitoramento individual;
* Integração de múltiplas fontes de dados, como Google Workspace, Microsoft 365, Slack, Zoom e GitHub;
* Comparação entre equipes e períodos, permitindo identificar mudanças nos padrões de trabalho;
* Métricas agregadas de colaboração, reuniões, foco e jornada;
* Network Graphs, utilizados para representar relações de colaboração entre pessoas e equipes;
* Benchmarks, utilizados para contextualizar os indicadores;
* Filtros por grupos, funções, gestores e outros atributos, permitindo aprofundar a análise;
* Identificação de sinais relacionados a burnout e sobrecarga, sem realizar diagnóstico individual;
* Análise de adoção de IA, acompanhando como as equipes estão incorporando ferramentas de IA;
* Privacidade incorporada ao modelo, com anonimização, pseudonimização e agregação dos dados;
* Ausência de análise do conteúdo das comunicações, utilizando metadados sobre a atividade de trabalho.

#### Pontos positivos, limitações e lições

| Ponto | Evidência | Implicação para nosso projeto |
|---|---|---|
| Positivo: análise de padrões de trabalho | Métricas de colaboração, foco e reuniões           | Analisar padrões relacionados às tarefas e não apenas atividades isoladas        |
| Positivo: comparação entre períodos      | Comparação de métricas e benchmarks                | Comparar o comportamento atual com períodos anteriores para identificar desvios  |
| Positivo: privacidade incorporada        | Dados agregados e análise por grupos               | Priorizar a privacidade e evitar monitoramento individual excessivo              |
| Positivo: múltiplas fontes de dados      | Integração com ferramentas de trabalho             | Futuramente, integrar diferentes fontes para enriquecer a análise                |
| Limitação: grande quantidade de métricas | Mais de 200 métricas e diversos filtros            | Priorizar poucos indicadores na visão inicial e permitir aprofundamento          |
| Limitação: foco organizacional           | Análise de colaboração e comportamento das equipes | Manter o WorkSense focado em tarefas e desvios, evitando ampliar demais o escopo |
| Limitação: dependência de integrações    | Dados provenientes de diversas ferramentas         | Começar com as fontes essenciais para reduzir a complexidade                     |

### Análise C04 — Workday Peakon Employee Voice

**Autor(a):** Tainá Cunha — 22.119.025-9  
**Tipo:** direto 
**Link oficial:** (https://www.workday.com/en-us/products/employee-voice/overview.html)
**Data de acesso:** 09/09/2026

#### Contexto e proposta

O Workday Peakon Employee Voice é uma plataforma de escuta de funcionários voltada à coleta e análise contínua de feedback. A ferramenta utiliza pesquisas, dashboards e recursos de inteligência artificial para acompanhar indicadores relacionados a engajamento, sentimento, bem-estar e outros aspectos da experiência dos funcionários. Os resultados são apresentados aos gestores por meio de scores, comparações, áreas prioritárias e recomendações que auxiliam na identificação de pontos que podem exigir atenção.
A plataforma também utiliza Processamento de Linguagem Natural para analisar comentários dos funcionários. O recurso AI Topics agrupa comentários semanticamente semelhantes, gera resumos dos principais assuntos e associa informações como sentimento, volume de comentários e segmentos mais relacionados ao tema.

#### Funcionalidades relevantes

| Funcionalidade | Como é realizada | Evidência/print | Observação de IHC |
|---|---|---|---|
| Dashboard de engajamento e acompanhamento temporal [4.1] | O dashboard reúne o score de engajamento, comparação com benchmarks, evolução do score ao longo do tempo, participação nas pesquisas e os principais fatores associados aos resultados. Também destaca áreas consideradas prioridades ou pontos fortes para facilitar o direcionamento da análise pelo gestor. |   <img width="837" height="522" alt="image" src="https://github.com/user-attachments/assets/7a6d7a36-0d3d-4009-a0b3-10941d290eb1" /> | A interface apresenta primeiro um score geral e permite aprofundar a análise pelos indicadores que contribuíram para o resultado. A tendência temporal e a comparação com uma referência ajudam o gestor a interpretar o valor dentro de um contexto. Por outro lado, a presença simultânea de scores, benchmarks, percentuais e indicadores visuais pode induzir interpretações simplificadas caso o significado de cada elemento não esteja claro. |

#### Experiência do usuário e opiniões

Na página do Capterra, o Workday Peakon Employee Voice possui nota 4,7/5 em 64 avaliações, com 4,7/5 em facilidade de uso e 4,8/5 em atendimento ao cliente. Entre os pontos positivos relatados está a facilidade para dividir os resultados por áreas, funções, características organizacionais e drivers, além de acompanhar como os resultados mudam ao longo do tempo. Também há avaliações que apontam limitações nas funcionalidades de planejamento e acompanhamento das ações criadas a partir dos resultados. [4.2]

#### Preço/modelo de negócio

O Workday não apresenta uma tabela pública de preços para o Peakon Employee Voice na página oficial. A contratação segue um modelo comercial voltado a organizações, com solicitação de demonstração e contato com a equipe de vendas para definição da proposta.

#### Padrões e tendências percebidos

- dashboard com score principal e detalhamento progressivo dos fatores relacionados ao resultado;
- comparação dos resultados com benchmarks internos e externos;
- acompanhamento da evolução dos scores ao longo do tempo;
- identificação de áreas prioritárias e pontos fortes;
- segmentação dos resultados por equipes e outros atributos organizacionais;
- uso de mapas de calor para comparar grupos e períodos;
- análise de comentários por PLN, com agrupamento de tópicos e identificação de sentimento [4.3];
- recomendações e planos de ação associados aos resultados;
- controle de visibilidade e uso de limites mínimos de respostas para preservar a confidencialidade dos funcionários.

#### Pontos positivos, limitações e lições

| Ponto | Evidência | Implicação para nosso projeto |
|---|---|---|
| Positivo: comparação temporal explícita | Score over time e comparação entre rodadas | Apresentar de forma clara a diferença entre o baseline e o período de reanálise |
| Positivo: detalhamento dos fatores do score | Pontos destacados e áreas prioritárias | Mostrar quais componentes contribuíram para uma alteração no score, evitando apresentar apenas o valor final |
| Positivo: contextualização dos valores | Benchmarks internos e externos | Apresentar o score junto de uma referência que ajude o gestor a interpretar a alteração |
| Positivo: análise de comentários por IA | AI Topics agrupa comentários e apresenta sentimento, volume e temas | Contextualizar os indicadores comunicacionais apresentados ao gestor em forma de texto |
| Limitação: dependência de pesquisas e participação | Os indicadores são construídos principalmente a partir das respostas e comentários dos funcionários | O WorkSense pode utilizar registros comunicacionais e profissionais já produzidos durante a rotina de trabalho, reduzindo/eliminando a dependência de pesquisas periódicas |
| Limitação: grande quantidade de informações | Dashboard reúne scores, benchmarks, tendências, participação e drivers (pontos destacados) | Priorizar no WorkSense uma visão inicial simples e permitir aprofundamento conforme a necessidade |
| Limitação: scores e cores podem favorecer interpretação classificatória | Dashboard e heat maps utilizam valores e cores para destacar diferenças | Apresentar as alterações como sinalizações para investigação, com contexto e explicação dos indicadores, evitando representar o colaborador como simplesmente “bom” ou “ruim” |

## 3. Softwares que o público-alvo usa no cotidiano

Analise interfaces que moldam a expectativa do público, mesmo que não sejam concorrentes.

| Software | Por que o público usa | Padrões relevantes | Prints | O que aprender |
|---|---|---|---|---|
| Trello | Fonte de dados de tarefas e representacao Kanban do TCC | quadro, listas, cartoes, responsaveis, etiquetas, prazo, filtros, tabela, calendario e dashboard | [Trello Views](https://trello.com/en/views) | Manter correspondencia entre indicador profissional e objetos conhecidos, como tarefa, prazo e estado |
| Telegram | Fonte de mensagens, audios e comandos do experimento | conversa cronologica, remetente, resposta, status de envio, grupo, bot e comandos | [Telegram Bot Platform](https://core.telegram.org/bots) | Usar linguagem conversacional apenas para tarefas simples e fornecer feedback imediato de processamento |


## 3.1 Padrões de interface relevantes ao escopo de IHC

Registre somente padrões encontrados nas soluções analisadas e que possam ter relação com objetivos reais da equipe.

| Padrão observado | Produto(s) | Para qual tarefa serve | Vantagem percebida | Risco/limitação | Aplicável ao nosso escopo? |
|---|---|---|---|---|---|
| dashboard | Todos | Acompanhar indicadores e obter uma visão geral dos dados antes de aprofundar a análise | Permite identificar rapidamente informações relevantes e concentrar diferentes indicadores em uma mesma visão | A concentração de muitos indicadores pode aumentar a carga visual e dificultar a interpretação | Sim |
| relatório | Todos, exceto C03 | Consultar resultados consolidados e informações mais detalhadas sobre os indicadores analisados | Facilita o aprofundamento e o compartilhamento dos resultados | Relatórios extensos podem dificultar a identificação rápida das informações que merecem atenção | Sim |
| histórico + filtros | Todos, exceto C02 | Explorar resultados por período, grupo ou outros atributos e acompanhar sua evolução ao longo do tempo | Permite investigar alterações e visualizar os dados dentro de um contexto específico | Muitos filtros e possibilidades de segmentação podem tornar a exploração mais complexa | Sim |
| administração/CRUD | C04 | Cadastrar e gerenciar usuários, grupos, atributos e permissões de acesso ao sistema | Permite controlar quem pode acessar e administrar diferentes dados e funcionalidades | O excesso de opções administrativas pode aumentar a complexidade da interface e exige cuidado com permissões de acesso a dados sensíveis | Sim |
| comparação de resultados | Todos | Comparar períodos, grupos, benchmarks ou valores de referência para identificar alterações | Facilita a percepção de mudanças e reduz a necessidade de o gestor comparar informações de telas diferentes mentalmente | Comparações sem contexto podem levar a interpretações simplificadas ou classificatórias dos resultados | Sim |

> O objetivo não é concluir “todo concorrente tem dashboard, então teremos um”. O padrão só será adotado se apoiar uma tarefa rastreável.

## 4. Síntese comparativa da equipe

| Critério | C01 | C02 | C03 | C04 | Oportunidade para o projeto |
|---|---|---|---|---|---|
| Navegação | Areas e visoes por papel; exploracao profunda | Abas separadas por categoria, aplicativo e produtividade | Dashboards com filtros e diferentes métricas | Dashboards e áreas de análise | Organizar a interface por níveis de detalhe, começando com uma visão geral dos perfis e permitindo aprofundar a análise de scores, componentes e períodos quando necessário |
| Feedback/estado | Período, filtros, legenda e visualizacao atual | Indicadores, rankings e variação percentual | Métricas, benchmarks e comparações entre períodos | Score, benchmark, tendência e participação | Exibir claramente o período analisado, o baseline de referência, a variação dos scores e quais componentes contribuíram para cada sinalização |
| Prevenção/recuperação de erro | Agregacao e controles de privacidade; complexidade pode gerar erro analitico | Grande quantidade de indicadores pode dificultar a interpretação | Muitos dados e filtros podem gerar sobrecarga | Limites mínimos de respostas | Evitar interpretações equivocadas por meio de explicações dos indicadores, contexto das sinalizações e avisos quando houver dados insuficientes para uma análise confiável |
| Terminologia | Técnica: ONA, insularidade, colaboracao | Termos como Productivity Score e Burnout Risk | Termos relacionados a colaboração, métricas e benchmarks | Termos como engagement score, drivers, benchmark e topics | Utilizar termos simples e próximos da linguagem do gestor, explicando conceitos técnicos como baseline, score e variação sempre que necessário |
| Acessibilidade | Não auditada; grafo depende de cor e densidade | Diversos gráficos podem dificultar comparação direta | Grande quantidade de métricas pode aumentar a carga visual | Atenção à dependência de cores nos heat maps | Evitar depender somente de cores para representar alterações, utilizando também textos, valores, ícones ou outros elementos visuais para indicar o significado dos dados |
| Eficiência | Comparação lado a lado reduz etapas | Dashboard apresenta resumo de vários indicadores | Filtros e benchmarks facilitam exploração | Destaque automático de prioridades e mudanças mais relevantes | Destacar primeiro os perfis e indicadores com alterações mais relevantes, reduzindo o esforço do gestor para identificar quais situações merecem análise mais detalhada |

## 5. Recomendações derivadas

Liste recomendações com origem explícita.

- **RC01:** Apresentar a comparação entre o baseline e o período atual de forma visual e direta, destacando a variação ocorrida — derivada de C04, que apresenta a evolução dos scores ao longo do tempo e comparações entre períodos.
- **RC02:** Exibir junto ao score os indicadores que mais contribuíram para sua alteração, permitindo que o gestor entenda a origem da sinalização — derivada de C04, que detalha os drivers relacionados aos resultados apresentados.
- **RC03:** Destacar na visão inicial as alterações que mais merecem atenção e permitir o aprofundamento dos dados quando necessário — derivada de C04, que utiliza áreas prioritárias e detalhamento progressivo dos resultados.
- **RC04:** Evitar que cores sejam o único recurso para indicar melhora, piora ou variação, apresentando também valores e informações textuais — derivada de C04, cujo dashboard e mapas de calor utilizam cores para representar diferenças entre resultados.
- **RC05:** mostrar baseline e periodo recente lado a lado, com datas explicitas - derivada de C01 e C03; relacionada a A01 e A02.
- **RC06:** separar score comunicacional e score profissional e permitir ver seus componentes - derivada de C04 e do requisito tecnico do TCC; relacionada a H05.
- **RC07:** apresentar definicao, fonte, periodo, cobertura e limitacao junto de cada indicador - derivada de C02; relacionada a A03 e H05.
- **RC08:** limitar a visao inicial aos indicadores necessarios para decidir se vale investigar - derivada da densidade observada em C01-C03; relacionada a H06.
- **RC09:** oferecer aprofundamento progressivo por sinalizacao, preservando filtros e contexto - derivada de C01, C03 e C04; relacionada a A02.
- **RC10:** distinguir visual e textualmente estabilidade, dados ausentes, dados insuficientes, processamento em andamento e erro - derivada da comparacao dos estados de C01-C03; relacionada a H07.
- **RC11:** evitar rotulos como "produtivo", "improdutivo", "saudavel" ou "em risco" sem contexto - derivada das limitacoes de C03 e C04; relacionada a prevencao de dano.
- **RC12:** nao usar somente cor para representar aumento, reducao, prioridade ou alerta - derivada das telas de C01, C03 e C04; relacionada a acessibilidade.
- **RC13:** aplicar minimizacao, agregacao, limite de grupo, papeis de acesso e registro de consulta - derivada de C01, C02 e C04; relacionada a H02-H04.
- **RC14:** permitir que o gestor registre contexto, decisao e acompanhamento sem receber diagnostico ou punicao automatica - derivada de C04 e do escopo do TCC; relacionada a A04.
- **RC15:** oferecer mecanismo posterior de incluir voz/contexto do colaborador - derivada do contraste entre C01-C03 e C04; relacionada a H02.

## Referências

| ID | Concorrente | Link|
|---|---|---|
| 1.1 | CO1 | https://learn.microsoft.com/en-us/viva/insights/introduction |
| 1.2 | CO1 | https://learn.microsoft.com/en-us/viva/insights/advanced/analyst/network-collaboration-insights |
| 1.3 | CO1 | https://adoption.microsoft.com/files/viva/insights/Microsoft-Viva-Insights_Measuring-change.pdf |
| 2.1 | C02 | https://support.activtrak.com/hc/en-us/articles/18821721976475-Organization-Overview |
| 2.2 | C02 | https://www.activtrak.com/pricing/ |
| 2.3 | C02 | https://support.activtrak.com/hc/en-us/articles/360050977352-What-Data-Does-ActivTrak-Collect |
| 2.4 | C02 | https://www.capterra.com/p/135366/ActivTrak/reviews/ |
| 3.1 | C03 | https://www.worklytics.co/workplace-insights-dashboard
| 3.2 | C03 | https://www.worklytics.co/pricing |
| 3.3 | C03 | https://www.worklytics.co/how-it-works |
| 3.4 | C03 | https://www.g2.com/sellers/worklytics |
| 4.1 | C04 | https://forms.workday.com/en-us/quick-demos/workday-peakon-employee-voice/form.html | 
| 4.2 | C04 | https://www.capterra.com/p/151069/Peakon/reviews/ |
| 4.3 | C04 | https://doc.workday.com/peakon/en-us/workday-peakon-employee-voice/insights/topics/concept--ai-topics.html |

## Checklist

- [ ] O mapa inicial de alternativas da Entrega 1 foi revisitado e aprofundado.
- [ ] Hipóteses relevantes sobre mercado/padrões foram atualizadas na rastreabilidade quando surgiram evidências.
- [ ] Há pelo menos uma análise completa por integrante.
- [ ] Cada análise contém prints legíveis da interface.
- [ ] Prints mostram telas/estados relevantes, não apenas logos/homepage.
- [ ] Foram analisados concorrentes e/ou interfaces representativas ao público.
- [ ] Em TCC sem interface original, foram investigadas ferramentas profissionais análogas às atividades do usuário escolhido.
- [ ] Padrões como dashboard, relatório, filtros e CRUD foram analisados como soluções para tarefas, não como requisitos automáticos.
- [ ] Opiniões de UX têm fonte.
- [ ] A síntese compara critérios comuns e produz recomendações.
- [ ] Não há “copiar porque o concorrente faz”; há justificativa de adequação ao público/contexto.
