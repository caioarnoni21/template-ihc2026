# Entrega 14 — Avaliação de usabilidade por observação de usuários

**Data:** 25/11/2026 
**Status:** ⬜ não iniciada  
**Responsabilidade:** solução consolidada por equipe. O número de participantes finais observados deve ser igual ao número de integrantes, conforme o modelo da disciplina; recomenda-se que cada integrante seja responsável por conduzir/analisar ao menos um participante.

## Objetivo da atividade

Observar usuários representativos realizando tarefas reais ou realisticamente simuladas para identificar problemas de eficácia, eficiência, compreensão e satisfação que não podem ser inferidos apenas por inspeção.

> **Participantes finais não devem ser membros da equipe.** Um integrante pode participar do teste piloto apenas para validar roteiro/equipamentos, sem contar na amostra final.

### Quando o usuário é um perfil profissional especializado

Em TCCs técnicos, o público pode ser DBA, analista, pesquisador, administrador, técnico ou outro especialista. Priorize participantes que possuam relação real com as tarefas. Se não for possível recrutar o perfil ideal, qualquer participante aproximado/proxy deve ser **justificado previamente e tratado como limitação**; não apresente o resultado como equivalente ao de especialistas reais.

O teste avalia a **interação com o protótipo**. Não é necessário que o participante valide o desempenho científico do algoritmo. Resultados simulados podem ser usados quando declarados e coerentes com a tarefa.

Tarefas podem envolver, por exemplo, interpretar um dashboard, configurar uma análise, encontrar uma execução no histórico usando filtros, comparar resultados, gerar relatório, revisar alerta ou administrar permissões.

## A. Fluxograma do processo — equipe

```text
Planejamento -> Recrutamento -> Consentimento -> Preparação/piloto
     -> Execução das tarefas e observação -> Pós-teste
     -> Consolidação e análise -> Recomendações -> Revisão e novo teste
```

O fluxograma deve representar, no mínimo: planejamento → recrutamento → consentimento → preparação → execução das tarefas/observação → pós-teste → consolidação/análise → recomendações.

## B. Procedimento de preparação e execução — equipe

### Passo 1 — Objetivos e versão avaliada

**Versão/Figma:** interface WorkSense exibida na gravação, com login, cadastro e telas de acompanhamento correspondentes a F06–F13. A identificação de uma versão congelada não foi informada. Não assumir que o arquivo Figma atual seja idêntico ao vídeo.

**Metas relacionadas:** MU01 (conclusão autônoma), MU02 (tempo), MU03 (satisfação), MU04 (reconhecimento da insuficiência) e MU05 (recuperação). MU06 (teclado) não foi avaliada nesta análise.

**Diferença entre planejamento e execução:** o roteiro previa tarefas delimitadas e satisfação de 1 a 5. Na gravação, a apresentação inicial é seguida de exploração com comentários contínuos; não se identifica na transcrição a leitura dos três enunciados padronizados. Por isso, esta sessão é analisada como exploração comentada, sem presumir execução formal de UT01–UT03.

### Passo 2 — Participantes

| ID | Perfil | Critérios que justificam participação | Integrante responsável |
|---|---|---|---|
| U01 | Pessoa convidada a explorar o papel de gestora; experiência profissional não informada | Relação real com gestão, idade adulta, não participação na criação e condição de participante final/piloto a confirmar | Caio Arnoni |

### Passo 3 — Consentimento e privacidade

- Termo/registro de consentimento: https://youtu.be/WtuprvRRVB4?si=fKXCTH8kL0X2RaO5
- Gravação de tela/áudio/vídeo: A gravação contém tela e imagem dos participantes; a transcrição contém suas falas. Finalidade: documentar a interação para a atividade acadêmica.
- Forma de anonimização: O relatório utiliza U01, sem reproduzir o nome real. O vídeo, porém, contém identificação visual e nominal: não é material anonimizado. A página o apresenta como não listado; essa condição não equivale a acesso privado.
- Local e período de armazenamento: Vídeo não listado de acesso restrito via link direto exclusivamente durante o semestre letivo de 2026.2 para avaliação docente, sendo removido após o encerramento da disciplina.

### Passo 4 — Teste piloto

**Data:** 25/11/2026  
**O que foi validado:** roteiro, duração, entendimento das instruções, protótipo, gravação.  
**Mudanças após piloto:** Após a gravação, não ocorreu mudanças no momento

### Passo 5 — Tarefas

| ID | Cenário/instrução apresentada | Critério de sucesso | Métricas | Ligação com modelo |
|---|---|---|---|---|
| UT01 | Previsto: consultar M. F. no ciclo 22/10–05/11, registrar próximo passo e conferir. Leitura desse enunciado não identificada; há exploração de sinalização, confiabilidade e registro entre aproximadamente 02:11 e 03:27. | Caso/período corretos, interpretação dos eixos, encaminhamento justificado e confirmação conferida | Sucesso, tempo, erros, ajudas e satisfação previstos; não aferidos de forma padronizada nesta sessão | T01/M01; F06–F11 |
| UT02 | Previsto: examinar outro caso, decidir e registrar. Há exploração da variante incompleta entre aproximadamente 03:31 e 04:04, sem enunciado formal identificado. | Reconhecer falta de dados, não concluir sobre a pessoa, registrar limitação e conferir | Evidência qualitativa de compreensão e ambiguidade; sem contagem validada de erros ou tempo de tarefa | T01/O08; F09/F12/F13 |
| UT03 | Previsto: concluir registro diante de falha simulada. Não foi identificada aplicação desse cenário na transcrição. | Reconhecer falha, recuperar e conferir sem ajuda | Não aferidas | T01/O10; estado de falha e recuperação |

### Passo 6 — Protocolo do moderador

1. Receber participante e explicar que **o produto está sendo avaliado, não a pessoa**.
2. Obter consentimento.
3. Aplicar perfil pré-teste mínimo necessário.
4. Ler instruções padronizadas.
5. Observar sem ensinar o caminho; registrar pedidos de ajuda separadamente.
6. Se usar *think aloud*, explicar e aplicar de forma consistente.
7. Após cada tarefa, registrar satisfação/SEQ ou escala definida.
8. Fazer pós-teste/entrevista breve.
9. Encerrar e explicar uso dos dados.

## C. Resultados — por participante

### U01 — {{perfil resumido}}

| Tarefa | Grau de sucesso | Erros | Tipos de erro/dificuldade | Ajudas | Tempo | Satisfação | Evidência/observação |
|---|---|---:|---|---:|---|---|---|
| UT01 — trecho relacionado | Não classificável pelos critérios completos | Não quantificados | Possível confusão entre magnitude das barras e quantidade de dias; confirmar em teste dirigido | Não quantificadas; sem orientação operacional explícita identificada na transcrição | Não aferido; 02:11–03:27 é intervalo de referência, não tempo de tarefa | Sem medida por tarefa | [02:17](https://www.youtube.com/watch?v=WtuprvRRVB4&t=137s): interpreta barras mencionando dias; [02:35](https://www.youtube.com/watch?v=WtuprvRRVB4&t=155s): reconhece limites não diagnósticos; [03:06](https://www.youtube.com/watch?v=WtuprvRRVB4&t=186s): descreve opções e registro. Não comprova preenchimento e conferência integral. |
| UT02 — trecho relacionado | Evidência parcial de compreensão; sucesso formal não classificável | Não quantificados | Reconhece falta de dados, mas interpreta apoiar e aguardar como opções disponíveis | Não quantificadas | Não aferido; referência 03:31–04:04 | Sem medida por tarefa | [03:31](https://www.youtube.com/watch?v=WtuprvRRVB4&t=211s): reconhece análise incompleta; [03:42](https://www.youtube.com/watch?v=WtuprvRRVB4&t=222s): menciona as duas opções. Conferência visual pontual em 03:55 mostra Apoiar e Aguardar dados selecionados. |
| UT03 | Aplicação não identificada | Não aferidos | Recuperação de falha não demonstrada nesta análise | Não aferidas | Não aferido | Não aferida | Não há evidência suficiente de falha simulada seguida de recuperação. |

**Link da gravação (se autorizado):** https://youtu.be/WtuprvRRVB4?si=fKXCTH8kL0X2RaO5 
**Resposta pós-teste:** entre 04:22 e 05:12, U01 avalia positivamente organização, quantidade de informação e padrões de cores. Em 05:01, atribui espontaneamente “nota 10”, sem escala formal aplicada. Não converter essa opinião em 5/5 nem em cumprimento de MU03. Entre 05:30 e 05:54, relata mudança de tamanho entre telas e botões que pareciam não permitir clique. Entre 05:54 e 06:19, explica que priorizaria casos sinalizados ou incompletos.

> Repita para U02, U03...

## D. Consolidação por tarefa

| Tarefa | Taxa de sucesso | Tempo típico | Erros recorrentes | Satisfação | Meta atendida? | Problemas prioritários |
|---|---:|---|---|---|---|---|
| UT01 | Não calculável | Não aferido | Recorrência não estimável com a sessão disponível | Avaliação geral positiva; sem escala por tarefa | Não demonstrado: MU01–MU03 | Conferir entendimento das barras e funcionamento dos controles |
| UT02 | Não calculável | Não aferido | Ambiguidade de opções evidenciada em um trecho de U01; sem recorrência entre usuários estabelecida | Sem medida específica | MU04 não demonstrada integralmente | Corrigir opções incompatíveis com análise incompleta |
| UT03 | Não calculável | Não aferido | Não observados neste cenário; não equivale a ausência de erros | Não aferida | MU05 não avaliada | Disponibilizar e testar falha/recuperação |

## E. Achados e recomendações

| ID | Achado | Evidência (quant. + qual.) | Impacto | Recomendação | Artefatos a revisar |
|---|---|---|---|---|---|
| AU01 | U01 interpreta Apoiar como opção na análise incompleta | Uma participante, no trecho 03:42–03:56, menciona apoiar e aguardar; imagem de 03:55 mostra ambas selecionadas. Não há taxa populacional ou contagem total de erros | Pode levar à interpretação de que um encaminhamento incompatível com insuficiência está permitido | Desmarcar/desabilitar Apoiar nesse estado e verificar se a confirmação preserva exclusivamente Aguardar dados | F12/F13, signos de seleção, M01/O08, HC01 |
| AU02 | Participante relata variação de tamanho entre telas | Relato de U01 em 05:30–05:41; dimensões exatas não medidas | Pode interromper continuidade visual e exigir readaptação | Padronizar frames e configuração de apresentação; percorrer os fluxos no mesmo dispositivo e zoom | Figma e configuração do protótipo |
| AU03 | Participante relata botões que pareciam não funcionar | Relato em 05:44–05:54; controles específicos não identificados na fala | Pode impedir exploração e criar dúvida sobre o resultado das ações | Localizar os controles com nova inspeção do percurso; conectar os previstos no teste e sinalizar claramente funções fora de escopo | Ligações do Figma, roteiro e cobertura da Entrega 11 |
| AU04 | Possível confusão na leitura das barras comparativas | Em 02:17–02:31, U01 descreve a diferença em termos de dias; é hipótese de interpretação, não erro confirmado | Pode distorcer a compreensão dos indicadores | Explicitar unidade e significado das barras; perguntar em nova tarefa o que cada valor representa, sem antecipar a resposta | F07, rótulos e modelo conceitual |
| AU05 | Boa recepção visual e reconhecimento de limites do sinal | Elogios em 00:48–01:13 e 04:22–05:12; em 02:35–02:45 distingue mudança de trabalho de interpretação de saúde | Indício favorável de compreensão local e aceitação; não comprova eficácia global | Preservar hierarquia, cores consistentes e explicações não diagnósticas; verificar com outros participantes | F07 e padrões visuais do protótipo |

## F. Comparação com a avaliação heurística

| Problema | Detectado na heurística? | Detectado por usuários? | O que aprendemos |
|---|---|---|---|
| HC01 — seleção simultânea em F12 | Sim, revisão preliminar assistida por IA | Há evidência de interpretação compatível: U01 considera as duas opções; não denuncia explicitamente o problema | O risco previsto aparece na leitura da participante, mesmo com avaliação geral positiva |
| HC02 — divergência entre escolha e confirmação | Sim, condicional ao mesmo fluxo | Não confirmado nesta análise | A exploração não basta para comprovar preservação da escolha; testar com registro específico |
| HC03 — ação “Está tudo certo” | Sim, revisão preliminar | Não relatado explicitamente | Ausência de crítica não elimina a ambiguidade identificada por inspeção |
| Mudança de tamanho e botões inativos | Não constavam entre HC01–HC03 | Relatados por U01 no pós-teste | A observação acrescenta problemas da apresentação interativa que capturas isoladas não permitem verificar |


## G. Conclusão

A conclusão deve responder:

1. Quais metas de usabilidade foram atingidas?
2. Quais problemas foram recorrentes e com quais perfis/tarefas?
3. O que surpreendeu a equipe?
4. Quais mudanças são prioritárias?
5. Que limitações do teste impedem generalizações amplas?

## Checklist

- [ ] Número de participantes finais atende ao enunciado.
- [ ] Participantes são representativos do público e não são membros da equipe.
- [ ] Se foram usados participantes proxy, a justificativa e a limitação estão explícitas.
- [ ] O teste avalia a interação; não confunde usabilidade do protótipo com desempenho técnico do TCC.
- [ ] Tarefas administrativas/analíticas usadas no teste são rastreáveis a objetivos e cenários.
- [ ] Há consentimento e anonimização.
- [ ] Foi realizado teste piloto.
- [ ] Tarefas têm critérios de sucesso definidos antes do teste.
- [ ] Moderadores não ensinaram o caminho durante a tarefa.
- [ ] Resultados estão separados por usuário e por tarefa.
- [ ] Foram registrados sucesso, erros, ajudas, tempo e satisfação quando aplicáveis.
- [ ] Conclusão combina evidência quantitativa e qualitativa.
- [ ] Achados geram recomendações e atualização da rastreabilidade.
