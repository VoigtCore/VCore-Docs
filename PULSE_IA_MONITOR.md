# VCore Pulse IA Monitor

O Pulse acompanha a saúde e o comportamento operacional da própria máquina ao longo do tempo. O monitor de IA organiza sinais de processos e recursos disponíveis; uma aplicação ou modelo reconhecido não prova, por si só, que uma inferência ocorreu.

## Estágio

- **Versão pública informada no perfil da VoigtCore:** 2.1.1, ciclo estável.
- **Evolução em desenvolvimento:** Pulse 2.2. O metadado 2.2.0 do checkout local não é um release público.
- A lista de sistemas e instaladores deve ser confirmada na página de download antes de anunciar suporte a uma plataforma.

## O que oferece

- Histórico temporal de saúde, recursos e eventos operacionais da máquina.
- Contexto sobre processos e aplicações, sujeito às fontes habilitadas e à cobertura de cada host.
- Relatórios e leitura de tendências com períodos e evidências de origem.
- Integrações locais e serviços comerciais separados do armazenamento operacional.

Valores ausentes, fontes degradadas e dados estimados precisam continuar identificados como tais. O produto não deve transformar falta de sinal em “máquina parada” nem sugerir causalidade que os dados não provam.

## Stack observada

Node.js no runtime e serviços; React e Vite na interface; bibliotecas de telemetria local e visualização; PostgreSQL nos serviços comerciais. O código possui um caminho SQLCipher para Windows, além de caminhos SQLite sem cifragem. Essas configurações não são equivalentes.

## Segurança e limites

O material de engenharia consultado registra testes do SQLCipher em bancos temporários no Windows e aponta que o executor ainda não estava ligado ao runtime padrão; o runtime SQLCipher para Linux também não estava disponível. Portanto, não se deve anunciar “banco sempre cifrado em repouso” sem confirmar a versão, o sistema operacional e o banco do instalador entregue.

O Pulse não substitui EDR, antivírus, monitoramento corporativo certificado ou diagnóstico físico. Integrações, alertas e serviços externos dependem da política e configuração correspondentes.

## Referências

- [Site e downloads do Pulse](https://www.voigtcore.com.br/)
- [Catálogo e estágio do ecossistema](PRODUCT_CATALOG.md)
- [Segurança, dados e SQLCipher](SECURITY_AND_DATA.md)
