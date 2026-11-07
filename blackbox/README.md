# BlackBox Governance

**Revisão:** 7 de novembro de 2026

**Checkout identificado:** 2.1.0

**Estágio:** demonstração assistida em Windows; venda aberta não aprovada.

## Para que serve

O BlackBox organiza a memória operacional local para investigar atividade de agentes de IA. A pessoa responsável começa por um intervalo ou sessão, segue as chamadas e ações que tenham evidência, examina artefatos relacionados e confere o consumo com a fonte que o produziu.

O produto deve responder, de forma simples: o que foi observado, em que horário, por qual fonte, quais arquivos aparecem, o que foi ação confirmada e quanto do consumo é medido, estimado ou indisponível.

## Funções em desenvolvimento

- Histórico por sessão, turno, intervalo e dia.
- Atividade e contexto de aplicação observados localmente.
- Relações com arquivos e artefatos quando existe uma referência de evidência.
- Tokens por período e saldo de cota da conta em leituras separadas.
- Rankings locais de artefatos e trajetórias recorrentes.
- Primeiro contato VLP com o VCore Server em perfil de laboratório.

Essas funções não provam que toda a atividade foi capturada. Uma fonte indisponível, um intervalo vazio ou um caminho declarado devem continuar identificados como lacunas.

## Estado de lançamento

A revisão de lançamento de 3–4 de novembro considera a demonstração assistida adequada, mas mantém a venda aberta bloqueada. Antes de piloto pago, ainda é preciso repetir numa instalação limpa e licenciada o caminho sessão → chamada → ação → arquivo → evidência → exportação, inclusive após falha de fonte e reinício. Também faltam reconciliação de cobrança por provedor e consistência dos termos comerciais.

## Stack

Node.js no supervisor, API e coletores; React e Vite na interface; SQLite na instalação observada; coleta local de contexto de aplicações e metadados de arquivos. O sistema separa supervisor e página web. Na homologação, fechar a aba não deve parar os coletores; o comando de saída da bandeja encerra o produto.

## Privacidade e segurança

O escopo local pode conter títulos de janela, caminhos e metadados de arquivos, nomes de processos e relações temporais. Esses dados podem revelar informações pessoais ou comerciais. A página [Investigação, consumo e evidências](INVESTIGACAO_E_CUSTOS.md) descreve como ler a fonte; [Segurança e SQLCipher](SEGURANCA_E_SQLCIPHER.md) diferencia a base ativa do código de desenvolvimento.

Não use esta versão para avaliação automática de produtividade, comprovação jurídica de autoria ou gestão centralizada entre clientes. O VLP de laboratório não habilita ingestão de evidências.

## Próximas validações

1. Instalação limpa em Windows 10 e 11, retomada e saída pela bandeja.
2. Captura repetível de sessão, chamadas, ações e arquivos com cobertura visível.
3. Custos reconciliados com uma cobrança autorizada; cotas e tokens permanecem métricas distintas.
4. Backup, recuperação, retenção e banco ativo identificados por versão.
5. Responsável, política e isolamento organizacional antes de gestão empresarial.
