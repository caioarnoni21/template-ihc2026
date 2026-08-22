# Matriz de rastreabilidade de IHC

A matriz deve ser atualizada ao longo do semestre. Ela ajuda a demonstrar que a interface não surgiu arbitrariamente e registra **como o conhecimento da equipe evoluiu**.

Para projetos cujo TCC não previa interface, esta matriz é especialmente importante: deve ficar visível a passagem da **contribuição técnica do TCC** para um **cenário de uso plausível**, e desse cenário para as decisões de interação.

## 1. Derivação do escopo de IHC a partir do TCC

| Elemento | Registro da equipe | Evidência/justificativa | Estado |
|---|---|---|---|
| Tema do TCC | WorkSense — ferramenta baseada em Inteligência Artificial para apoio à identificação de alterações nos padrões de comunicação, interação e desempenho em equipes. | TCC atual; título, introdução e objetivo. | definido |
| Resultado técnico esperado | Ferramenta experimental que integra registros comunicacionais e operacionais, extrai indicadores, calcula separadamente score comunicacional e score profissional e compara períodos de reanálise com o baseline individual. | [H] H01; descrição técnica atual do TCC. | definido |
| O TCC previa interface? | Parcialmente. | Há interação conversacional pelo Telegram e visualizações preliminares dos resultados, mas não uma interface de gestão completa com fluxos e requisitos de usabilidade definidos. [H] H02; descrição atual do TCC. | definido |
| Capacidade/contribuição central | Identificar mudanças nos padrões de comunicação, interação e indicadores profissionais ao longo do tempo, utilizando o histórico individual como referência e gerando sinalizações para apoiar a análise humana, sem caráter diagnóstico ou punitivo. | [H] H03. | H |
| Possíveis beneficiários/stakeholders | Gestor ou líder de equipe, colaborador, profissional de RH/gestão de pessoas, administrador da solução e pesquisadores/equipe do TCC. | [H] H04, H05, H06, H07, H08 e H09. | H |
| Usuário escolhido para IHC | Gestor ou líder de equipe. | [H] H05; é o perfil definido para utilizar diretamente a interface de gestão e interpretar os resultados. | H |
| Objetivo principal do usuário | Acompanhar a equipe de forma mais estruturada e preventiva, percebendo e interpretando variações relevantes e decidindo quando uma situação merece acompanhamento humano. | [H] H04; derivado do benefício esperado e do papel atribuído ao gestor. | H |
| Contexto de uso adotado | Acompanhamento cotidiano de equipes em contextos presenciais, remotos e digitais, no qual o gestor consulta informações produzidas pelo WorkSense para apoiar sua análise. | [F] F01 e [H] H04/H05. O contexto geral é fundamentado, mas o uso concreto da interface ainda precisa ser investigado. | H |
| Interface/recorte de IHC | Interface gerencial para cadastro e vínculo de colaboradores e para acompanhamento de scores, sinalizações, variações em relação ao histórico individual e indicadores associados. O foco principal do recorte será a interpretação dos resultados pelo gestor. | Deriva de [H] H03, H04 e H05. | proposta |
| Relação com o TCC | Aprofundamento de algo parcialmente previsto. | [H] H02; o TCC já prevê interação, scores, sinalizações e visualizações, mas não especifica uma interface gerencial completa. | definido |

> Se o escopo de IHC mudar ao longo do semestre, preserve a decisão anterior no histórico e registre **qual evidência motivou a mudança**.

## 2. Registro de hipóteses e lacunas da Entrega 1

Use esta tabela para itens importantes marcados como `[H]` ou `[?]`. Preserve o histórico: não apague uma hipótese refutada.

| ID | Afirmação / dúvida inicial | Tipo | Por que importa | Como/onde investigar | Evidência obtida | Estado atual | Impacto no projeto |
|---|---|---|---|---|---|---|---|
| H01 | O TCC prevê o desenvolvimento e a avaliação experimental do WorkSense, com processamento de registros comunicacionais e profissionais, extração de indicadores, cálculo separado dos scores e comparação temporal com baseline individual. | H | Delimita o que pertence ao TCC e quais capacidades técnicas podem dar origem ao recorte de IHC. | Entrega 1 | TCC atual. O desenvolvimento do WorkSense, a extração de indicadores, o cálculo dos scores e a comparação temporal com baseline estão previstos, enquanto a origem definitiva dos dados de avaliação ainda está em discussão. | aberta | Delimita as capacidades técnicas que poderão ser utilizadas pela interface de IHC e o que precisa permanecer consistente entre o TCC e o projeto da disciplina. |
| H02 | O TCC prevê interação conversacional e visualização de resultados, mas ainda não define uma interface gerencial completa e seus fluxos de uso ou requisitos de usabilidade. | H | Justifica o aprofundamento da interface na disciplina de IHC e delimita o que ainda precisa ser projetado. | Entrega 1 | O documento atual descreve Telegram, scores, sinalizações e visualizações preliminares, sem especificar uma interface gerencial completa. | sustentada | Os requisitos existentes funcionam como restrições e bases para o projeto de IHC, enquanto os requisitos específicos da interface deverão ser derivados da investigação com o usuário e das atividades modeladas na disciplina. |
| H03 | O WorkSense pode apoiar a identificação de alterações ao longo do tempo nos padrões de comunicação, interação e indicadores profissionais, utilizando o histórico individual como referência e mantendo a interpretação e a decisão sob responsabilidade humana. | H | É a contribuição central que a interface deverá tornar compreensível e utilizável pelo gestor. | Entrega 1 | PENDENTE | aberta | Orienta quais informações precisam ser apresentadas e quais interpretações a interface deve evitar induzir. |
| H04 | A contribuição pode tornar o acompanhamento das equipes mais estruturado e preventivo, auxiliando gestores na identificação e interpretação de variações, favorecendo um acompanhamento mais contextualizado dos colaboradores e apoiando decisões de gestão mais informadas e transparentes, sempre com supervisão humana. | H | Define o benefício esperado no mundo real e ajuda a distinguir objetivo do usuário de tarefas de interface. | Entrega 1 | PENDENTE | aberta | Orienta o objetivo principal do gestor e os critérios de utilidade percebida da interface. |
| H05 | O gestor ou líder de equipe será o usuário direto da interface do WorkSense, utilizando-a para cadastrar e vincular colaboradores e acompanhar scores, sinalizações e indicadores associados. | H | Define o usuário prioritário e os principais fluxos que serão projetados na disciplina. | Entrega 1 | Decisão inicial de escopo da equipe; validação com usuários PENDENTE. | aberta | Determina o perfil prioritário para personas, cenários, tarefas e testes de usabilidade. |
| H06 | O colaborador é a principal pessoa acompanhada pela ferramenta, produzindo registros comunicacionais e profissionais utilizados nas análises, mas não utilizando diretamente a interface de gestão. | H | O colaborador pode ser afetado pelas interpretações e decisões tomadas a partir da interface mesmo sem utilizá-la. | Entrega 1 | PENDENTE | aberta | Exige considerar transparência, privacidade, linguagem não punitiva e possíveis efeitos indiretos das decisões de design. |
| H07 | Profissionais de RH ou responsáveis pela gestão de pessoas podem atuar como stakeholders do WorkSense, contribuindo para políticas de uso, transparência, consentimento e limites de interpretação das sinalizações. | H | Esse perfil pode influenciar governança e condições de adoção da solução em contexto organizacional. | Entrega 1 | PENDENTE | aberta | Pode gerar requisitos de governança, transparência e controle de uso posteriormente. |
| H08 | A operação do WorkSense exigirá um perfil de administração responsável por configurar integrações, acessos, permissões, credenciais e demais parâmetros técnicos da solução. | H | Ajuda a separar tarefas de gestão das tarefas técnicas de manutenção e administração. | Entrega 1 | Requisitos técnicos atuais sugerem essa necessidade; validação do papel PENDENTE. | aberta | Evita inserir tarefas técnicas desnecessárias no fluxo principal do gestor. |
| H09 | Durante o contexto experimental do TCC, a equipe de pesquisadores será responsável por preparar os dados utilizados na avaliação, executar processamentos, realizar testes e analisar os resultados da ferramenta. | H | Delimita quem opera a solução experimental e evita confundir atividades de pesquisa com tarefas do usuário final. | Entrega 1 | Processo atual de desenvolvimento do TCC. | sustentada | Mantém atividades experimentais fora do fluxo principal da interface destinada ao gestor. |
| H10 | Gestores podem apresentar diferentes níveis de familiaridade com métricas, indicadores e ferramentas digitais. | H | O nível de familiaridade pode influenciar a compreensão dos scores, sinalizações e comparações temporais. | Entrega 1 | PENDENTE | aberta | A apresentação dos resultados deverá ser testada com usuários de diferentes níveis de familiaridade, sem presumir domínio técnico. |
| H11 | Colaboradores apresentam padrões distintos de comunicação, interação e utilização das ferramentas de trabalho e podem possuir diferentes percepções sobre a finalidade e o uso de seus dados pela solução. | H | Diferenças individuais influenciam a justificativa do baseline individual e os riscos de interpretação dos resultados. | Entrega 1 | PENDENTE | aberta | Reforça a necessidade de evitar comparações simplistas entre pessoas e de considerar transparência sobre o uso dos dados. |
| H12 | Profissionais de RH ou responsáveis pela gestão de pessoas tendem a possuir maior familiaridade com processos organizacionais e questões de governança, mas podem apresentar diferentes níveis de familiaridade com indicadores quantitativos e ferramentas digitais. | H | Pode influenciar o tipo de informação e nível de detalhamento necessário caso esse stakeholder participe do uso ou governança da solução. | Entrega 1 | PENDENTE | aberta | Pode influenciar requisitos futuros de explicação, relatórios ou governança, caso o perfil seja mantido no escopo. |
| H13 | Administradores da solução necessitam de maior familiaridade técnica com integrações, acessos, permissões e configurações para realizar atividades de implantação e manutenção do WorkSense. | H | Permite distinguir necessidades técnicas das necessidades de acompanhamento do gestor. | Entrega 1 | PENDENTE | aberta | Pode justificar uma área administrativa separada, caso essa necessidade seja confirmada. |
| H14 | A equipe de pesquisa necessita de maior nível de detalhamento técnico sobre indicadores, scores e processamento dos dados para testar e avaliar a solução experimental. | H | O nível de informação necessário para pesquisa é diferente daquele necessário ao gestor. | Entrega 1 | A equipe precisa consultar indicadores, componentes dos scores e resultados dos algoritmos para validar cálculos e identificar erros. | sustentada | Evita projetar a interface do gestor com excesso de informação técnica necessária apenas à pesquisa. |
| ?01 | Qual será a origem dos dados utilizados na avaliação do WorkSense: dados simulados, dados reais ou uma base de dados existente? | ? | A escolha afeta o protocolo experimental, os critérios de avaliação, as limitações do estudo e as questões éticas envolvidas. | Discussão com orientador; levantamento de bases existentes; análise das implicações metodológicas e éticas de cada alternativa. | TCC atual prevê dados simulados, mas essa decisão está sendo reavaliada pela equipe e pelo orientador. | aberta | Pode alterar a metodologia de avaliação do TCC e os requisitos relacionados a privacidade, consentimento e tratamento dos dados. Neste momento, não determina diretamente o recorte da interface de IHC. |

## 3. Rastreabilidade entre contribuição técnica, necessidades e artefatos

| ID | Capacidade do TCC utilizada | Necessidade/problema | Persona | Cenário problema | Objetivo/tarefa | HTA/GOMS/CTT | Cenário de interação / signos | MoLIC | Tela(s) Figma | Heurística / problema | Tarefa no teste | Decisão/melhoria |
|---|---|---|---|---|---|---|---|---|---|---|---|---|
| R01 | {{ex.: recomendação de otimização}} | {{...}} | {{P01}} | {{C01}} | {{T01}} | {{links}} | {{...}} | {{M01}} | {{F01...}} | {{V01 ou —}} | {{UT01}} | {{...}} |
| R02 |  |  |  |  |  |  |  |  |  |  |  |  |

## 4. Rastreabilidade de padrões de interface

Use esta tabela quando o projeto incorporar padrões como dashboard, relatório, histórico, filtros ou administração. O objetivo é **justificar o padrão**, não apenas listar telas.

| ID da tela/fluxo | Padrão de interface | Objetivo/tarefa que justifica | Informação/ação principal | Evidência de necessidade | Artefatos relacionados |
|---|---|---|---|---|---|
| F01 | dashboard | {{T01}} | {{...}} | {{H01/evidência...}} | {{C01/M01}} |
| F02 | histórico com filtros | {{T02}} | {{...}} | {{...}} | {{...}} |
| F03 | administração/CRUD | {{T03}} | {{...}} | {{...}} | {{...}} |

## 5. Registro de mudanças de escopo

| Data | O que mudou | Evidência/feedback que motivou | Artefatos afetados | Responsável |
|---|---|---|---|---|
| {{...}} | {{...}} | {{...}} | {{...}} | {{...}} |

## Como usar

- Use identificadores estáveis (`H01`, `P01`, `C01`, `T01`, `M01`, `F01`, `UT01`).
- Quando uma necessidade/problema tiver origem em hipótese da Entrega 1, cite o ID correspondente.
- Em TCC sem interface original, pelo menos uma linha deve mostrar claramente **como uma capacidade técnica chega até uma tarefa de usuário e uma tela/fluxo**.
- Uma linha pode se desdobrar quando um objetivo possui múltiplos caminhos.
- Não force relação inexistente: se algo ainda não foi modelado, marque `PENDENTE`.
- Ao remover uma funcionalidade, registre a decisão em vez de apagar silenciosamente o histórico.
- Dashboard, CRUD, filtros e relatórios só devem aparecer quando houver objetivo/tarefa que os justifique.
