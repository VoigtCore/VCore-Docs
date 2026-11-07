# Guia rápido — VCore Pulse IA Monitor

## Versão

O perfil público da VoigtCore informa Pulse 2.1.1 como ciclo estável e Pulse 2.2 em desenvolvimento. Baixe o pacote e confira os sistemas suportados na [página oficial](https://www.voigtcore.com.br/). Um número de versão no checkout não substitui uma release publicada.

## Primeira leitura

1. Instale o pacote oficial compatível com o sistema.
2. Abra o painel e confira quais sensores estão disponíveis.
3. Dê tempo para o histórico amadurecer; um período sem dados deve aparecer como lacuna, não como zero real.
4. Abra o detalhe de um indicador para identificar período, fonte e cobertura.
5. Use relatórios históricos como contexto, não como diagnóstico determinístico de falha.

## Monitoramento de IA

O monitor pode organizar sinais de processos, aplicações e recursos, de acordo com a cobertura instalada. A presença de um processo ou de um modelo não prova que houve uma inferência nem identifica, sozinha, a pessoa responsável.

## Privacidade e armazenamento

O escopo de coleta depende da versão e da configuração. Métricas de processos podem revelar uso e contexto. Antes de uso empresarial, explique fontes e retenção aos usuários e defina quem pode consultar e exportar os registros.

SQLCipher aparece em caminhos de engenharia Windows, mas os relatórios consultados não demonstram que todo banco do runtime entregue é cifrado. Consulte [Segurança, dados e SQLCipher](SECURITY_AND_DATA.md) antes de fazer uma promessa de proteção em repouso.

## Ajuda

Para disponibilidade, licenças, planos e contatos, use o [site oficial da VoigtCore](https://www.voigtcore.com.br/).
