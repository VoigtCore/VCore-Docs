# VLP — primeiro contato BlackBox/Server

## O que foi demonstrado

No ambiente de homologação local, o Server reconhece a família BlackBox, valida um descriptor assinado e o canal mTLS do perfil de laboratório. O resultado máximo é FOUND_UNTRUSTED.

## O que esse resultado significa

Confirma somente que o primeiro contato correspondeu à identidade e ao canal esperados dentro daquele ensaio. Não significa:

- organização ou dispositivo matriculados;
- confiança promovida;
- autorização para ler dados da máquina;
- heartbeat contínuo;
- ingestão de tokens, chamadas, arquivos, ações ou trajetórias;
- controle ou execução remota.

## Próximo gate

Definir finalidade, minimização, consentimento/autoridade, tenant, retenção e esquema autorizado; implementar matrícula e ciclo de certificados; provar isolamento e revogação; manter a evidência primária no BlackBox local; só então aprovar uma integração de dados.

Enquanto esses gates não forem concluídos, a UI e a documentação devem chamar esse estado de “primeiro contato de laboratório”, não de conexão empresarial pronta.
