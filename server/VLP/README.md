# VLP/1 — protocolo e identidade

VLP significa VCore Link Protocol. É a camada semântica que organiza identidade, versão, sequência, proveniência e autorização entre componentes VCore; HTTPS/TLS é um transporte, não a autoridade sobre os dados.

## Identidades distintas

O contrato diferencia node, device, instalação de produto, Avatar, organização, chave e ator. Descoberta não significa confiança; confiança não significa autorização; autorização não concede acesso irrestrito.

## Mensagem e segurança

As mensagens carregam identificador, schema versionado, sequência, horários de ocorrência e observação, classificação e origem. A fundação documenta Ed25519 para descritores e envelopes, proteção contra repetição e ensaios TLS 1.3/mTLS locais.

O protocolo não é VPN, shell remoto, canal para comandos arbitrários ou telemetria obrigatória. Dados permanecem negados por padrão e devem ser minimizados.

## Estágio

- Núcleo VLP/1.0 e contratos foram implementados no checkout.
- O contato local BlackBox↔Server alcança FOUND_UNTRUSTED em ensaio de loopback.
- O perfil e os certificados usados em laboratório são temporários e não são PKI de produção.
- Matrícula real, ciclo de certificado empresarial, rotação/revogação, autorização de dados e ingestão contínua seguem pendentes/desabilitados.

## Registro no INPI

O certificado administrativo consultado identifica VCore VLP/1, processo BR512026007083-0, como registro de programa de computador, emitido em 1º de setembro de 2026. O registro não é patente do protocolo, certificação de segurança, conformidade ou interoperabilidade.

Não publicar hash do código registrado, chaves, certificados privados nem documentação técnica reservada. Veja a orientação oficial do [INPI para programas de computador](https://www.gov.br/inpi/pt-br/assuntos/programas-de-computador).
