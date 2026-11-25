# Formulário de avaliação heurística — modelo

**Avaliador:** Caio Arnoni 22.221.019-7 
**Versão:** capturas F06–F13 documentadas na Entrega 11.  
**Data:** 25/11/2026.  
**Estados especiais examinados:** representação visual de análise completa, análise incompleta, seleção de encaminhamento e confirmação; navegação, validação e recuperação de falha não verificadas nesta revisão.

## Cobertura

| H | Heurística | Fluxos/telas examinados | Violação? | IDs |
|---:|---|---|---|---|
| 1 | Visibilidade do status do sistema | F06, F08, F09, F11 e F13: status, cobertura, atualização e confirmação representados. Falha de salvamento e feedback durante processamento ainda precisam de inspeção interativa. | Pendente de inspeção completa | — |
| 2 | Compatibilidade sistema–mundo real | F06: relação entre o resumo da equipe e o significado da ação “Está tudo certo, registrar e sair”. | Sim | V03 |
| 3 | Controle e liberdade do usuário | F07–F10 e F12: ações de voltar e continuar visíveis; funcionamento de retorno, edição e abandono ainda precisa ser percorrido. | Não | — |
| 4 | Consistência e padrões | F10/F11: comparação entre encaminhamento selecionado e resumo de confirmação; F12: aparência de opções mutuamente exclusivas. | Sim | V01, V02 |
| 5 | Prevenção de erros | F12: restrição anunciada para análise incompleta e opções visualmente selecionadas. | Sim | V01 |
| 6 | Reconhecimento em vez de memorização | F06–F13: identificação do caso, período, navegação contextual e resumo representados; continuidade desses dados entre telas ainda precisa ser verificada. | Não | — |
| 7 | Flexibilidade e eficiência de uso | F06: acesso à sinalização e retomada de rascunho representados; não foram medidos tempo, atalhos ou funcionamento da retomada. | Não | — |
| 8 | Estética e design minimalista | F06–F13: hierarquia, densidade e relevância do conteúdo visível; conferir legibilidade e adaptação na versão de teste. | Não | — |
| 9 | Reconhecer, diagnosticar e recuperar erros | F09/F12: falta de dados explicada. Estados de campo inválido, falha ao salvar e nova tentativa não demonstrados nas capturas. | Sim | — |
| 10 | Ajuda e documentação | F07–F09: explicações sobre significado, limites e comparação. Acesso e suficiência da ajuda precisam ser inspecionados no fluxo. | Sim | — |

## Problemas

| ID | H | Tela/estado | Ação/condição | Problema | Consequência | Evidência | Severidade 0–4 | Justificativa | Recomendação |
|---|---|---|---|---|---|---|---:|---|---|
| V01 | 4, 5 | F12 — Registro com análise incompleta | Visualizar as opções de encaminhamento no estado em que apenas “Aguardar dados” deveria estar disponível. | “Apoiar” e “Aguardar dados” aparecem simultaneamente selecionados, embora o aviso diga que só é possível aguardar dados. | O gestor pode não compreender qual decisão será registrada ou acreditar que apoiar está disponível nesse estado. | Na tela F12, “Apoiar” e “Aguardar dados” exibem indicadores de seleção e contornos verdes simultaneamente, em conflito com o aviso superior. | 3 — Grave | A contradição afeta diretamente a interpretação de uma decisão central de T01; não é apenas acabamento visual. Não foi verificado qual valor seria salvo. | Manter somente “Aguardar dados” selecionado; desabilitar e desmarcar as demais opções nesse estado. Verificar que a confirmação preserve essa escolha. |
| V02 | 4 | F10/F11 — Registro e confirmação | Comparar as capturas do formulário de registro e de sua confirmação proposta. | F10 exibe “Apoiar” selecionado, enquanto F11 apresenta “Acompanhar” no resumo, sem evidência de uma mudança intermediária. | Se ocorrer no mesmo fluxo, o gestor pode confirmar ou acreditar que salvou uma decisão diferente da escolhida. | Na tela F10, a opção selecionada é “Apoiar”; na tela F11, o resumo apresenta “Acompanhar”. | 3 — Grave, se confirmado no mesmo fluxo | A divergência compromete a confiança na confirmação. Nas capturas ela é verificável, mas não prova alteração de dados durante a navegação. | Alinhar seleção e confirmação do mesmo cenário. Se forem exemplos independentes, identificá-los como tais. Percorrer cada opção até a confirmação e conferir a preservação do valor. |
| V03 | 2 | F06 — Visão geral da equipe | Ler o resumo e escolher uma ação inicial. | O botão “Está tudo certo, registrar e sair” sugere uma conclusão geral positiva, embora o resumo mostre uma sinalização e uma análise incompleta; também não explicita a quem o registro se refere. | Pode induzir encerramento prematuro ou dúvida sobre o caso e a decisão que serão registrados. | Na tela F06, o resumo informa uma pessoa com sinalização e uma análise incompleta, enquanto o botão afirma “Está tudo certo, registrar e sair”. | 2 — Menor | O rótulo cria ambiguidade e pode orientar uma interpretação inadequada, mas a alternativa de consultar a sinalização permanece visível. A consequência depende do destino do botão, ainda não verificado. | Usar uma ação neutra, como “Registrar encaminhamento”, exigindo identificação clara do caso. Não afirmar que está tudo certo quando há sinalização ou dados insuficientes. |
