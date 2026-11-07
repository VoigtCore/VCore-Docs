# VCore Server

O VCore Server é a camada de identidade, memória, relação e governança de ativos autorizados do ecossistema. Seu papel é reunir projeções controladas de máquinas e serviços sem confundir um dispositivo, uma instalação de produto, uma pessoa e uma organização.

## Estágio

O pacote local está identificado como **0.8.0**. A documentação de engenharia descreve uma fundação em desenvolvimento, com cadastro de ativos, linha do tempo, proveniência, supervisão e telas de operação. Não é uma edição empresarial pronta para instalação em frota.

O perfil padrão mantém ações administrativas e transporte remoto desabilitados. O login operacional, o isolamento de organizações, a matrícula de vários agentes, a instalação, a atualização e a restauração repetíveis ainda precisam de gates próprios.

## Stack observada

Node.js e JavaScript no backend e nas ferramentas locais, APIs HTTP, SQLite legado com migrations aditivas e conectores explícitos. Há uso de net-snmp para um conector de rede; a descoberta e as consultas são limitadas ao plano autorizado e não equivalem a varredura irrestrita.

## Segurança e operação

- As identidades de máquina, instalação, produto, usuário e organização são tratadas como entidades distintas.
- O modo padrão é local e controlado; a integração Pulse usa projeções limitadas.
- A apresentação do BlackBox ao Server não habilita ingestão operacional de evidências.
- A leitura de uma rede real deve ser explicitamente configurada. Inventário declarado não é uma observação de rede.
- Não publique endereços, portas, nomes de host, credenciais, topologia detalhada, identificadores de clientes nem arquivos de runtime.

Veja [Visão pública da infraestrutura](SERVER_INFRASTRUCTURE.md) e [VLP/1](VLP_PROTOCOL.md).
