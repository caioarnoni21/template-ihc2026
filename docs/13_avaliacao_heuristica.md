# Entrega 13 — Avaliação de IHC por inspeção heurística

**Data:** 25/11/2026 
**Status:** ⬜ não iniciada  
**Responsabilidade:** 1 avaliação completa por integrante, sobre todas as telas/estados relevantes do projeto.

## Objetivo da atividade

Encontrar problemas de usabilidade por inspeção sistemática da interface com as **10 heurísticas de Nielsen**. Cada avaliador trabalha individualmente primeiro; depois a equipe consolida problemas duplicados e prioridades.

> **Parte de violações:** registre somente problemas reais. Não invente uma violação para “preencher” cada heurística. Para provar que todas foram exercitadas, use a **matriz de cobertura H1–H10**. Para heurísticas sem violação, a disciplina solicita um exemplo didático de boa prática.

## 1. Heurísticas adotadas

1. Visibilidade do status do sistema
2. Compatibilidade entre o sistema e o mundo real
3. Controle e liberdade do usuário
4. Consistência e padrões
5. Prevenção de erros
6. Reconhecimento em vez de memorização
7. Flexibilidade e eficiência de uso
8. Estética e design minimalista
9. Ajudar usuários a reconhecer, diagnosticar e recuperar-se de erros
10. Ajuda e documentação

## Cobertura especial para interfaces administrativas e analíticas

Quando existirem, não limite a avaliação às “telas principais”. Inspecione também:

- dashboard em estados normal, vazio e erro;
- filtros sem resultado e filtros combinados;
- relatórios e exportação;
- histórico/listas longas;
- formulários CRUD (criação, edição, exclusão, validação);
- alteração de perfil/permissão;
- confirmações de ações destrutivas;
- processamento/loading/progresso;
- falha e recuperação;
- comparação de resultados;
- mensagens de termos técnicos, métricas e recomendações;
- ajuda/documentação contextual.

Em TCCs técnicos, observe especialmente se a interface comunica o estado do processamento e traduz informações técnicas para o vocabulário do usuário escolhido.

## 2. Escopo da inspeção

| Item | Definição |
|---|---|
| Versão avaliada | Capturas documentadas na Entrega 11 em 25/11/2026. Referência: https://www.figma.com/design/McbDfvqqGuDnR9uDmBdJrp/Login-e-Cadastro-de-Colaboradores?node-id=0-1&p=f&t=P0yKLlrbv12dHvD4-0. |
| Telas/estados | F06: visão geral; F07: sinalização; F08: confiabilidade completa; F09: análise incompleta; F10: registro; F11: confirmação; F12: registro com insuficiência; F13: confirmação de aguardar dados. IDs documentais, não IDs internos do Figma. |
| Fluxos | M01/T01: consulta, interpretação, encaminhamento e confirmação, com variante de insuficiência. Recuperação de falha, abandono e fluxos dos demais integrantes precisam ser examinados para cumprir o escopo integral. |
| Dispositivo/viewport | Revisão de imagens estáticas de interface desktop; navegador, zoom e viewport de execução não aferidos nesta revisão. |
| Avaliadores |A01: Caio Arnoni 22.221.019-7 |

## 3. Procedimento individual

Cada avaliador deve:

1. percorrer os fluxos/telas ao menos uma vez para familiarização;
2. inspecionar novamente aplicando sistematicamente H1–H10;
3. registrar cada problema com evidência e contexto;
4. atribuir severidade **depois de compreender bem o problema**, justificando a decisão;
5. não discutir achados com os demais antes de terminar a inspeção individual, quando o objetivo for preservar independência.

### Escala de severidade (0–4)

| Grau | Interpretação |
|---:|---|
| 0 | Não é considerado problema de usabilidade. |
| 1 | Problema cosmético; corrigir se houver tempo. |
| 2 | Problema menor; baixa prioridade. |
| 3 | Problema maior; alta prioridade. |
| 4 | Catástrofe de usabilidade; correção imperativa antes de disponibilizar. |

Ao justificar, considere **frequência, impacto e persistência** do problema no contexto real de uso.

---

## Avaliador A01 — Caio Arnoni

### 4. Matriz de cobertura das 10 heurísticas

| Heurística | Telas/fluxos examinados | Houve violação? | IDs dos achados | Exemplo de boa prática se não violada |
|---|---|---|---|---|
| H1 | F06, F08, F09, F11 e F13: status e confirmação representados. | Não | — | F09 informa falta de dados; F11/F13 apresentam resumo da confirmação. |
| H2 | F06: resumo da equipe e significado da ação de registro. | Sim | V03 | Não se aplica como declaração de ausência de violação. |
| H3 | F07–F10/F12: controles de retorno e continuidade representados. | Sim | — | “Voltar à sinalização” e “Voltar à visão geral” indicam alternativas de navegação |
| H4 | F10/F11: opção e confirmação; F12: seleção exclusiva. | Não | V01, V02 | Não se aplica como declaração de ausência de violação. |
| H5 | F12: restrição anunciada e opções apresentadas. | Não | V01 | Não se aplica como declaração de ausência de violação. |
| H6 | F06–F13: pessoa, ciclo, navegação contextual e resumo. | Sim | — | Identificação de M. F. e ciclo visíveis reduzem a necessidade de lembrar qual caso está em consulta. |
| H7 | F06: retomada de rascunho e acesso à sinalização. | Não | — | A ação “Retomar” representa um acesso direto à atividade interrompida; funcionamento e eficiência não medidos. |
| H8 | F07/F08: organização das informações em grupos. | Não | — | Comunicação, atividades e cobertura possuem títulos próprios, favorecendo a leitura por assunto. Legibilidade em outros tamanhos não verificada. |
| H9 | F09/F12: estado de insuficiência. | Sim | — | A mensagem informa ausência de dados do Telegram e sugere verificar o identificador; não comprova recuperação de falha de salvamento. |
| H10 | F07–F09: significado, limites e comparação. | Não | — | “O que este sinal NÃO significa” explica limites e evita tratar a sinalização como diagnóstico ou avaliação de desempenho. |

### 5. Declaração de violações

| ID | Heurística | Tela/estado | Problema observado | Evidência | Severidade | Justificativa da severidade | Recomendação |
|---|---|---|---|---|---:|---|---|
| V01 | H4, H5 | F12 — Registro com análise incompleta | Ao visualizar os encaminhamentos, o gestor encontra “Apoiar” e “Aguardar dados” selecionados simultaneamente, embora só aguardar dados seja permitido pelo aviso. Isso torna ambígua a decisão a registrar. | <img width="1115" height="781" alt="image" src="https://github.com/user-attachments/assets/6ba5a9c5-19ec-4fdc-a597-d6af3dbc11a2" /> | 3 — Maior, preliminar | Frequência potencial: toda abertura desse estado na versão representada. Impacto: dúvida sobre a decisão válida. Persistência: a contradição permanece enquanto os controles não forem corrigidos. Não foi verificado o valor salvo. | Desmarcar e desabilitar as opções incompatíveis com insuficiência; manter somente “Aguardar dados” selecionado e conferir sua preservação na confirmação. |
| V02 | H4 | F10/F11 — Registro e confirmação | O formulário mostra “Apoiar”, enquanto a confirmação mostra “Acompanhar”, sem mudança intermediária documentada. Se forem etapas do mesmo fluxo, o resultado diverge da escolha. | <img width="1216" height="776" alt="image" src="https://github.com/user-attachments/assets/bd18bda4-04bf-41b0-9e65-6d2e1602b489" /> | 3 — Maior, se confirmado no mesmo fluxo | Frequência e persistência dependem do encadeamento, ainda não verificado. Impacto potencial alto: perda de confiança e confirmação de decisão diferente. A divergência visual é real, mas não comprova alteração durante a navegação. | Conferir o encadeamento e alinhar escolha e confirmação. Se forem cenários independentes, identificá-los. Testar cada opção até seu resumo final. |
| V03 | H2 | F06 — Visão geral | O rótulo “Está tudo certo, registrar e sair” induz uma conclusão geral positiva diante de sinalização e insuficiência, sem explicitar a pessoa destinatária do registro. | <img width="878" height="773" alt="image" src="https://github.com/user-attachments/assets/00bfb480-38ae-41bd-a379-60c8b723fad1" /> | 2 — Menor, preliminar | Frequência potencial: acesso à visão geral nesse estado. Impacto: ambiguidade e possível encerramento prematuro; existe alternativa visível para consultar o sinal. Persistência: o rótulo reaparece a cada acesso enquanto mantido. Destino do botão ainda não verificado. | Adotar rótulo neutro, como “Registrar encaminhamento”, e explicitar o caso ao qual se aplica; não afirmar que está tudo certo diante de dados insuficientes. |

**Qualidade do relato:** o problema deve ser observável e localizado. Evite “interface confusa” sem dizer **o que**, **onde**, **quando** e **para quem**.

### 6. Boas práticas — heurísticas não violadas (atividade didática)

| Heurística sem violação | Exemplo no sistema | Evidência | Por que atende |
|---|---|---|---|
| H1 — aspecto local | Informação de insuficiência. | <img width="1017" height="778" alt="image" src="https://github.com/user-attachments/assets/0dd9b424-31e4-4fa1-a02c-b3520e2a9b62" /> | Torna explícito o estado e sua limitação, em vez de apresentar ausência de dados como estabilidade. |
| H3 — intenção representada | Alternativas de retorno. | <img width="1016" height="775" alt="image" src="https://github.com/user-attachments/assets/2b726935-0b2f-4186-8298-6ceb42459a33" /> <img width="1017" height="778" alt="image" src="https://github.com/user-attachments/assets/0a70121f-0910-4e30-8398-5eb87c6b6912" /> | Indica uma saída sem obrigar o registro. O funcionamento precisa ser verificado. |
| H6 — aspecto local | Contexto visível. |<img width="1216" height="776" alt="image" src="https://github.com/user-attachments/assets/75b5adb1-65da-4597-a78b-a950f0c48f40" /> <img width="1241" height="776" alt="image" src="https://github.com/user-attachments/assets/4ebf0a97-c654-4c61-99fb-2cbfb98725f2" /> | Permite reconhecer o contexto sem depender exclusivamente da memória da tela anterior. |
| H7 — intenção representada | Retomada de rascunho. | <img width="878" height="773" alt="image" src="https://github.com/user-attachments/assets/3eb0f178-e95b-4d03-a26a-a31551ddd624" /> | Pode reduzir etapas de reencontro da atividade; a retomada real ainda deve ser testada. |
| H8 — aspecto local | Agrupamento por assunto. | <img width="1140" height="786" alt="image" src="https://github.com/user-attachments/assets/646d58e2-7c1f-4f93-b77f-0b7e46843c85" /> | Ajuda a localizar informações relacionadas sem misturar dimensões diferentes. |
| H9 — aspecto local | Explicação da falta de dados. | <img width="1017" height="778" alt="image" src="https://github.com/user-attachments/assets/feec26c8-4a72-4b9d-bc27-17ca99a7c67f" /> | Expõe uma causa a verificar e uma ação possível, sem depender apenas de código de erro. |
| H10 — aspecto local | Ajuda contextual. |<img width="1140" height="786" alt="image" src="https://github.com/user-attachments/assets/baba6e83-004f-4dd6-a7a8-fe4e6b595d66" /> | Oferece explicação junto à informação que o gestor precisa interpretar. |

> Repita a seção para A02, A03... um avaliador por integrante.

## 7. Consolidação da equipe

Problemas iguais ou muito semelhantes encontrados por avaliadores diferentes devem ser consolidados, preservando quem os encontrou.

| ID consolidado | Achados individuais | Heurística | Problema | Severidade final | Prioridade | Responsável pela correção |
|---|---|---|---|---:|---|---|
| HC01 | V01 — revisão preliminar assistida por IA | H4, H5 | F12 apresenta “Apoiar” e “Aguardar dados” selecionados simultaneamente, apesar de permitir apenas aguardar dados. | Proposta: 3 — maior; validar com a equipe | Alta — corrigir antes do teste do estado incompleto | Proposta: Caio Arnoni, em alinhamento com o responsável pela edição do protótipo |
| HC02 | V02 — revisão preliminar assistida por IA | H4 | F10 mostra “Apoiar”, mas F11 confirma “Acompanhar”, sem alteração intermediária documentada. | Proposta: 3 — maior, se confirmado no mesmo fluxo | Alta — verificar o encadeamento e corrigir antes do teste de registro | Proposta: Caio Arnoni, em alinhamento com o responsável pela edição do protótipo |
| HC03 | V03 — revisão preliminar assistida por IA | H2 | F06 oferece “Está tudo certo, registrar e sair” mesmo apresentando sinalização e insuficiência de dados. | Proposta: 2 — menor; validar com a equipe | Baixa em relação a HC01/HC02; incluir na revisão anterior ao teste | Proposta: Caio Arnoni, em alinhamento com o responsável pela edição do protótipo |

## 8. Síntese e plano de melhoria

- Quantidade de problemas por heurística e severidade.
- Problemas críticos/graves que bloqueiam teste ou release.
- Padrões recorrentes entre telas.
- Correções que serão feitas antes/para a avaliação com usuários.

## Checklist

- [ ] Cada integrante fez uma inspeção completa e identificada.
- [ ] Todas as telas/estados relevantes foram examinados.
- [ ] Estados administrativos, filtros, relatórios, históricos, processamento e erros foram incluídos quando existentes.
- [ ] A inspeção avaliou a interface/protótipo, não o mérito técnico do algoritmo/modelo.
- [ ] H1–H10 aparecem na matriz de cobertura de cada avaliador.
- [ ] Parte de violações contém apenas violações, sem “forçar” exemplos.
- [ ] Todo problema tem print/localização e contexto.
- [ ] Severidade possui justificativa, não apenas número.
- [ ] Recomendação resolve a causa ou reduz o impacto.
- [ ] Achados duplicados foram consolidados ao final.
