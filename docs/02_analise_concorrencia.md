# Entrega 2 — Público-alvo e análise de concorrência

**Data:** {{26/08/2026}}  
**Status:** 🟨 em andamento  
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


### Análise C02 — Worklytics

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


### Análise C03 — ActivTrak 

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

> Repita a subseção para C02, C03... até atender à quantidade da equipe.

## 3. Softwares que o público-alvo usa no cotidiano

Analise interfaces que moldam a expectativa do público, mesmo que não sejam concorrentes.

| Software | Por que o público usa | Padrões relevantes | Prints | O que aprender |
|---|---|---|---|---|
| {{...}} | {{...}} | {{...}} | {{link local}} | {{...}} |

## 3.1 Padrões de interface relevantes ao escopo de IHC

Registre somente padrões encontrados nas soluções analisadas e que possam ter relação com objetivos reais da equipe.

| Padrão observado | Produto(s) | Para qual tarefa serve | Vantagem percebida | Risco/limitação | Aplicável ao nosso escopo? |
|---|---|---|---|---|---|
| dashboard | {{...}} | {{...}} | {{...}} | {{...}} | sim/não/talvez |
| relatório | {{...}} | {{...}} | {{...}} | {{...}} | {{...}} |
| histórico + filtros | {{...}} | {{...}} | {{...}} | {{...}} | {{...}} |
| administração/CRUD | {{...}} | {{...}} | {{...}} | {{...}} | {{...}} |
| comparação de resultados | {{...}} | {{...}} | {{...}} | {{...}} | {{...}} |

> O objetivo não é concluir “todo concorrente tem dashboard, então teremos um”. O padrão só será adotado se apoiar uma tarefa rastreável.

## 4. Síntese comparativa da equipe

| Critério | C01 | C02 | C03 | Oportunidade para o projeto |
|---|---|---|---|---|
| Navegação | Areas e visoes por papel; exploracao profunda |  |  |  |
| Feedback/estado | Periodo, filtros, legenda e visualizacao atual |  |  |  |
| Prevenção/recuperação de erro | Agregacao e controles de privacidade; complexidade pode gerar erro analitico |  |  |  |
| Terminologia | Tecnica: ONA, insularidade, colaboracao |  |  |  |
| Acessibilidade | Nao auditada; grafo depende de cor e densidade |  |  |  |
| Eficiência | Comparacao lado a lado reduz etapas |  |  |  |

## 5. Recomendações derivadas

Liste recomendações com origem explícita.

- **RC01:** {{recomendação}} — derivada de {{C01/C02/evidência}}.
- **RC02:** {{...}}

## Referências

{{fontes dos produtos, avaliações e literatura}}

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
