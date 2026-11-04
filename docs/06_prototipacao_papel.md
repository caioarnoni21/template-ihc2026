# Entrega 6 — Prototipação em papel

**Data:** {{04/11/2026}}  
**Status:** 🟨 iniciada 
**Responsabilidade:** 1 solução integrada por equipe

## Objetivo da atividade

Externalizar rapidamente ideias de interação em baixa fidelidade para explorar alternativas antes de investir em detalhes visuais. O valor da atividade está no **ciclo construir → simular → observar → revisar**, não na beleza do desenho.

## 1. Escopo do protótipo

**Personas:** P02 — João Pedro (primária, gestor de operações não analítico).  
**Cenários/tarefas cobertos:** C02 / T02 (triagem rápida e encaminhamento, Entrega 5); T07 da Entrega 1 (cadastrar e vincular colaboradores) como fluxo de apoio.  
**Objetivos principais:** responder "preciso me preocupar ou não?" em poucos minutos, sem jargão; verificar a confiabilidade antes de agir; registrar o encaminhamento com justificativa, sem diagnóstico nem veredito automático.

## 1.1 Possíveis famílias de interface

Escolha apenas o que for coerente com tarefas e cenários. Para TCCs técnicos, o protótipo pode explorar:

- **dashboard** para monitoramento e tomada de decisão;
- **configuração/parametrização** para preparar algoritmo/modelo/processo;
- **entrada/seleção de dados** com validação;
- **acompanhamento de execução** com progresso, fila, cancelamento e recuperação;
- **relatório/resultados** com explicação, gráficos e exportação;
- **histórico** com busca, filtros, ordenação e detalhes;
- **comparação** entre execuções, versões, algoritmos ou períodos;
- **administração** de usuários, papéis, permissões ou entidades do domínio;
- **auditoria/logs** traduzidos para o perfil;
- **alertas/ocorrências** com ação de resposta.

> Não desenhe todas essas telas por obrigação. O objetivo da baixa fidelidade é experimentar a **estrutura da interação** necessária para as tarefas priorizadas.

## 2. Fluxos escolhidos

| Fluxo | Tarefa/objetivo | Por que foi priorizado |
|---|---|---|
| PF01 | Entrar como gestor e cadastrar um colaborador (T07) | Sem colaboradores vinculados não há dados para acompanhar; é o fluxo de apoio do recorte de IHC |
| PF02 | Triagem rápida: ler o resumo, decidir não aprofundar e registrar (HTA 1 > 2 > 5) | Tarefa mais frequente do João Pedro, com cerca de 15 minutos entre reuniões (C02.Q2) |
| PF03 | Triagem completa: aprofundar, verificar confiabilidade e registrar, incluindo o desvio "aguardar dados" (HTA 1 > 2 > 3 > 4 > 5) | Tarefa crítica (H17): evita agir sobre análise incompleta e prejudicar alguém injustamente |

## 3. Telas e estados

| ID | Tela/estado | Fluxo | Controles que mudam o estado |
|---|---|---|---|
| P01 | Login do gestor (e-mail, senha, "Esqueceu a senha?", aviso "O login é apenas para gestores") — *Screen 2* | PF01 | Login → P03; falha → E01 |
| P02 | Cadastrar colaboradores (nome, sobrenome, e-mail, telefone, Telegram ID, Trello ID) dentro do menu lateral do gestor — *Screen 4* | PF01 | Salvar → confirmação e volta ao P03; campo inválido → E02 |
| P03 | Visão geral (Dashboard): resumo da equipe em linguagem simples, com sinalização se houver; nomes discretos | PF02/PF03 | Selecionar sinalização → P04; menu lateral → P02 |
| P04 | Significado da sinalização: "o que este sinal significa e não significa" e opção de aprofundar | PF02/PF03 | Aprofundar → P05; Não aprofundar → P06 |
| P05 | Confiabilidade: períodos (30 e 15 dias), atualização, estado da análise e explicação resumida; "ver detalhes" e "o que significa?" opcionais | PF03 | Continuar → P06; sem dados/incompleta/insuficiente → E03 |
| P06 | Registro: encaminhamento (apoiar, acompanhar, não intervir, aguardar dados) e justificativa | PF02/PF03 | Confirmar → P07; Voltar → tela anterior |
| P07 | Confirmação do registro | PF02/PF03 | Voltar à visão geral → P03 |
| E01 | Login inválido: mensagem clara, campos preservados | PF01 | Corrigir e tentar de novo |
| E02 | Cadastro com campo vazio ou ID já vinculado | PF01 | Corrigir campo |
| E03 | Análise não confiável: aviso distinto de "sem alteração relevante"; só permite "aguardar dados" | PF03 | Seguir para P06 com "aguardar dados" pré-selecionado |
| E04 | Retomada após interrupção: reabre no colaborador e na etapa em que parou | PF02/PF03 | Continuar |

<img width="1413" height="653" alt="image" src="https://github.com/user-attachments/assets/a3b83fa3-b943-46d7-aedc-9c6ad8a0a5f3" />



## 4. Simulação / walkthrough

**Participante:** Laura de Souza Parente (não participou da elaboração das telas)  
**Data:** {{04/11/2026}}  
**Cenário dado:** "Você é gestora de atendimento, tem 15 minutos entre duas reuniões e quer saber se precisa se preocupar com alguém da equipe. Decida e deixe registrado."

| Observação | Tela/ação | Evidência | Consequência para o design |
|---|---|---|---|
| {{...}} | P03 / Leitura inicial do resumo | {{o que ela disse ou fez}} | {{...}} |
| {{...}} | P04 / Texto "o que significa e não significa" | {{...}} | {{...}} |
| {{...}} | P05 e E03 / Distinguir "sem alteração" de "sem dados" | {{...}} | {{...}} |
| {{...}} | P02 / Preencher Telegram ID e Trello ID | {{...}} | {{...}} |
| {{...}} | P06 / Escolher encaminhamento e justificar | {{...}} | {{...}} |

## 5. Alterações após a simulação

As quatro primeiras linhas vêm da revisão que a equipe fez no protótipo antes da simulação, com base nas Entregas 1 a 5. As alterações decorrentes do teste com a Laura entram nas linhas seguintes.

| Antes | Problema | Depois | Justificativa |
|---|---|---|---|
| Telas em moldura de celular | A Entrega 1 (H21) e a Entrega 3 (H08, CT01) indicam o notebook como dispositivo principal | Telas redesenhadas em formato site, com menu lateral | Coerência com o contexto de uso definido |
| Login e tela inicial separados, com uma tela intermediária | Um passo a mais para um gestor com pouco tempo (C02.Q2) | Login e tela inicial unificados em uma única tela (P01) | Menos etapas até chegar à triagem |
| Campos Trello ID e Telegram ID com o mesmo texto de ajuda | O João Pedro tem pouca familiaridade técnica (P02) e não saberia diferenciar cada ID | Campos com rótulos distintos: "Telegram ID" e "Trello ID" | Reduz erro de vínculo entre colaborador e fontes de dados |
| Telas sem estado de erro | Senha errada, campo vazio ou ID duplicado deixavam o usuário sem saída | Estados E01 e E02 previstos, com mensagem clara e campos preservados | Prevenção e recuperação de erro |
| {{alteração decorrente da simulação com a Laura}} | {{...}} | {{...}} | {{...}} |

## 1. Escopo do protótipo

**Personas:** {{...}}  
**Cenários/tarefas cobertos:** {{C01/T01...}}  
**Objetivos principais:** {{...}}

## 1.1 Possíveis famílias de interface

Escolha apenas o que for coerente com tarefas e cenários. Para TCCs técnicos, o protótipo pode explorar:

- **dashboard** para monitoramento e tomada de decisão;
- **configuração/parametrização** para preparar algoritmo/modelo/processo;
- **entrada/seleção de dados** com validação;
- **acompanhamento de execução** com progresso, fila, cancelamento e recuperação;
- **relatório/resultados** com explicação, gráficos e exportação;
- **histórico** com busca, filtros, ordenação e detalhes;
- **comparação** entre execuções, versões, algoritmos ou períodos;
- **administração** de usuários, papéis, permissões ou entidades do domínio;
- **auditoria/logs** traduzidos para o perfil;
- **alertas/ocorrências** com ação de resposta.

> Não desenhe todas essas telas por obrigação. O objetivo da baixa fidelidade é experimentar a **estrutura da interação** necessária para as tarefas priorizadas.

## 2. Fluxos escolhidos

| Fluxo | Tarefa/objetivo | Por que foi priorizado |
|---|---|---|
| PF01 | {{...}} | {{...}} |

## 3. Telas e estados

- Numere as telas/estados (`P01`, `P02`...).
- Indique controles que mudam o estado.
- Mostre pelo menos caminhos principais e estados de erro/retorno relevantes.

![Protótipo](../assets/06_prototipos/prototipo_fluxo_01.svg)

## 4. Simulação / walkthrough

Realize uma simulação com uma pessoa que não participou da elaboração dessas telas. Um colega pode ser usado **para essa iteração formativa**, mas isso não substitui os participantes finais da Entrega 14.

| Observação | Tela/ação | Evidência | Consequência para o design |
|---|---|---|---|
| {{...}} | {{...}} | {{...}} | {{...}} |

## 5. Alterações após a simulação

| Antes | Problema | Depois | Justificativa |
|---|---|---|---|
| {{...}} | {{...}} | {{...}} | {{...}} |

## Checklist

- [ ] O protótipo cobre tarefas relevantes da Entrega 5.
- [ ] Cada tela/estado pode ser justificado por uma tarefa, decisão ou informação necessária.
- [ ] O projeto não criou dashboard/CRUD/login apenas para parecer “completo”.
- [ ] Telas/estados estão numerados e navegáveis na documentação.
- [ ] Há pelo menos uma simulação/walkthrough documentado.
- [ ] Críticas não foram apenas listadas: geraram decisão de revisão.
- [ ] O protótipo continua em baixa fidelidade; detalhes visuais não mascaram problemas de fluxo.
