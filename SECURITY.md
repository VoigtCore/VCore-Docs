# Segurança

Esta página descreve o estado conhecido dos componentes VCore e evita transformar controles parciais em promessas absolutas.

## Comunicação de vulnerabilidades

Envie uma descrição não sensível pelo [canal de contato da VoigtCore](https://www.voigtcore.com.br/). Não anexe segredos, dados de cliente ou cópias de bancos operacionais em mensagens públicas. A equipe deve coordenar recebimento, triagem, correção e divulgação.

## Limites declarados

- SQLCipher não está comprovadamente habilitado em todos os bancos e plataformas.
- TLS/mTLS e assinaturas foram exercitados em contextos específicos; isso não certifica a operação de produção.
- VLP não autoriza por si só acesso ou execução.
- O Native Container e o Studio são experimentais; o Studio não é sandbox.
- Não há neste catálogo declaração de certificação ISO, SOC 2, teste de penetração independente ou SLA.

Leia [Segurança, dados e SQLCipher](SECURITY_AND_DATA.md) e [VLP/1](VLP_PROTOCOL.md) para o estado por produto.
