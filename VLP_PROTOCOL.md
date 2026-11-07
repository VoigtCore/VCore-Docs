# VLP/1 — VCore Link Protocol

O VLP é o protocolo semântico de identidade, declaração, observação controlada e mensagens estruturadas entre componentes VCore. Ele organiza identidade, versão, sequência, proveniência e autorização; TLS é o transporte, não o significado da mensagem.

## Identidades e limites

O protocolo diferencia dispositivo, instalação de produto, máquina/Avatar, organização, chave e ator. Descoberta não significa confiança; confiança não significa autorização; autorização não significa acesso a todos os dados.

O contrato define envelopes assinados, identificadores de mensagem, sequência, horário de ocorrência e observação, schema e classificação. A finalidade é transportar somente projeções explicitamente autorizadas. O protocolo não é shell remoto, VPN, telemetria obrigatória nem mecanismo para executar comandos arbitrários.

## Segurança implementada e estágio

- Descritores de identidade e envelopes assinados com Ed25519.
- Controles de nonce, sequência, idempotência, replay e tolerância temporal.
- Ensaios locais de transporte TLS 1.3 com autenticação mútua.
- Primeiro contato entre BlackBox e Server em loopback de laboratório; a resposta máxima descrita é FOUND_UNTRUSTED.
- O material de teste e certificados locais não são uma PKI de produção.
- Matrícula empresarial, ciclo completo de certificado, rotação/revogação operacional, autorização de dados e ingestão contínua permanecem pendentes ou desabilitados.

## Registro no INPI

O certificado administrativo consultado identifica **VCore VLP/1**, processo **BR512026007083-0**, como registro de programa de computador, emitido em **1º de setembro de 2026**. O registro não é patente do protocolo, certificação de segurança, certificação de conformidade ou garantia de interoperabilidade.

Não publicamos o hash do código-fonte depositado, material de chave, certificado privado nem pacote técnico de registro. O [INPI descreve o registro de programa de computador](https://www.gov.br/inpi/pt-br/assuntos/programas-de-computador) como proteção referente ao programa identificado no pedido.

## Integrações

O [BlackBox](BLACKBOX_GOVERNANCE.md) pode apresentar uma identidade e capacidades declaradas no ambiente de laboratório. A [documentação do Server](VCORE_SERVER.md) explica os limites do primeiro contato. O estado do protocolo deve permanecer visível no produto: contato, confiança, matrícula e autorização são etapas diferentes.
