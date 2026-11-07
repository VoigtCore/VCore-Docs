# BlackBox — investigação, artefatos e consumo

## Fluxo de investigação

1. Selecione o dia e o intervalo de interesse.
2. Abra a sessão ou trajetória observada.
3. Siga cada chamada até a ação e o artefato somente quando houver uma referência que ligue esses registros.
4. Abra a fonte técnica quando precisar confirmar identificadores, tempos ou limites da consulta.
5. Exporte a evidência com sua origem, janela de tempo e lacunas.

Uma pasta declarada pela sessão não é o caminho percorrido. Um foco de janela mede contexto observado, não leitura de arquivo. Coincidência temporal entre IA e escrita não comprova autoria.

## Quatro estados de evidência

- **Observado:** a fonte local registrou o evento ou metadado descrito.
- **Declarado:** um agente, integração ou usuário informou o valor; não equivale a verificação independente.
- **Relacionado:** registros compartilham uma referência ou janela, mas a relação pode não provar causalidade.
- **Desconhecido ou sem sinal:** a fonte não permite concluir; não converter em zero, sucesso ou ausência de atividade.

## Tokens, porcentagens e cobrança

São leituras distintas:

- **Tokens medidos no dia:** soma de registros de uso associados à máquina no período.
- **Cota da conta:** saldo consultado no provedor em um momento. Se o saldo cai de X% para Y%, a variação atribuída ao intervalo é X − Y pontos percentuais, desde que haja snapshots comparáveis nos limites do intervalo.
- **Cobrança:** valor cobrado pelo provedor, exibido apenas quando a fonte confirma moeda, período e conta.
- **Estimativa:** cálculo baseado em preço por modelo ou volume; deve aparecer como estimativa.

Um saldo consultado agora não reconstrói automaticamente os saldos no início e no fim de cada hora. Para isso, o produto precisa guardar snapshots com horário e conta, ou obter os dados históricos oficiais do provedor. Nunca preencher a lacuna com um percentual inventado.

## Artefatos e recorrência

Rankings diários podem contar registros e dias distintos de recorrência. Repetir um acesso várias vezes no mesmo dia não deve aumentar o número de dias recorrentes. “Mais visitado” exige uma fonte de visita; “mais trabalhado” e “mais evoluído” exigem critérios e evidências adicionais.

## Limites da página de detalhes

Identificadores, hashes e logs pertencem às referências técnicas recolhidas. A leitura principal deve mostrar primeiro tempo, caminho, ação e custo; só então deve abrir a instrumentação detalhada. A duração de arquivo precisa vir de uma fonte de foco/abertura explícita e não deve ser inferida só pelo caminho encontrado.
