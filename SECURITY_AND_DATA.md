# Segurança, dados e SQLCipher

**Revisto em 7 de novembro de 2026.** Esta página distingue um recurso presente no código de um controle habilitado na versão que o cliente instala.

## Resumo por produto

| Produto | Estado documentado | O que não devemos prometer |
|---|---|---|
| Pulse IA Monitor | Há código e testes de lifecycle SQLCipher em Windows; os relatórios consultados dizem que o executor não estava ligado ao runtime padrão. SQLCipher para Linux não estava disponível nos relatórios. | “Todo banco Pulse é cifrado em repouso em qualquer plataforma.” |
| BlackBox Governance | A auditoria explícita de 13/10 encontrou SQLite sem SQLCipher na instalação ativa e um caminho SQLCipher separado no checkout. Não foi localizada evidência posterior de migração da instalação ativa. | “O banco operacional atual sempre usa SQLCipher.” |
| VCore Server | O pacote documenta SQLite legado e migrations locais. Não foi encontrada evidência de SQLCipher no runtime. | “A base do Server está cifrada por SQLCipher.” |
| Native Container | Journal SQLite e mecanismos experimentais de identidade/execução. O modo criptográfico descrito tem gates parciais/desligados por padrão. | “O Container cifra automaticamente qualquer pacote, journal ou código.” |
| VLP | Assinatura e transporte mTLS foram exercitados localmente; a PKI operacional e o ciclo comercial completo ainda não estão prontos. | “VLP é certificado por terceiros ou garante comunicação de produção.” |

SQLCipher é uma implementação de SQLite com cifragem. Testes em banco temporário, disponibilidade de um binário ou armazenamento cifrado de backup não provam que a base ativa da instalação está cifrada. A confirmação precisa identificar versão, sistema operacional, runtime e banco consultado.

## Dados que merecem tratamento

Pulse observa métricas operacionais e contexto de processos. BlackBox pode relacionar sessões e ações com aplicações, títulos de janela, caminhos e metadados de arquivos. Mesmo quando não há conteúdo do arquivo, nomes e títulos podem revelar informação pessoal ou comercial.

Antes de um piloto empresarial, defina e explique finalidade, fontes, acesso por função, retenção, exportação, exclusão, resposta a incidentes e compartilhamento com o Server. Não use a cobertura parcial como base para avaliação automática de produtividade ou autoria.

## Princípios de engenharia

- Minimização e finalidade explícita.
- Separar o registro local detalhado das projeções enviadas a serviços.
- Mostrar origem, tempo, cobertura e incerteza em cada inferência.
- Negar compartilhamento ou ação quando identidade e autorização não forem verificadas.
- Manter segredos, chaves privadas, dados de clientes e artefatos administrativos fora do GitHub público.
- Não declarar certificações ISO, SOC 2, LGPD ou testes independentes sem evidência formal correspondente.

## Divulgação de vulnerabilidades

Não publique credenciais, material de certificado, hashes de registro, dados de cliente ou instruções exploráveis em issues públicas. Use o canal de contato publicado em [voigtcore.com.br](https://www.voigtcore.com.br/) para coordenar uma comunicação responsável.
