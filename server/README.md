# VCore Server

**Pacote local:** 0.8.0

**Estágio:** desenvolvimento local e laboratório; não é uma distribuição empresarial pronta.

## Papel

O Server organiza identidade, memória, relações e governança de ativos autorizados. O modelo diferencia dispositivo, instalação de produto, Avatar de máquina, pessoa, organização e ator. Projeções de Pulse e BlackBox só podem atravessar a fronteira com escopo e autorização explícitos.

## Capacidades presentes na fundação

- Cadastro e contexto de ativos, setores, salas, serviços e responsáveis.
- Linha do tempo, proveniência e estado de sinais de infraestrutura.
- Interfaces de operação e projeções organizacionais.
- Conectores explícitos de rede e gestão de contexto.
- Primeiro contato local do agente BlackBox pelo VLP.

Inventário declarado não é descoberta observada. Métrica ausente não é zero. Uma apresentação de agente não é uma matrícula.

## Stack observada

Node.js e JavaScript; APIs HTTP locais; SQLite legado e migrations aditivas; net-snmp para conectores definidos. As ações administrativas e o transporte remoto permanecem desabilitados por padrão. O perfil de laboratório não deve ser copiado para produção.

## Prontidão operacional

Ainda faltam login operacional, isolamento completo entre organizações, matrícula de múltiplos agentes, PKI operacional, instalação e atualização repetíveis, recuperação verificada e ingestão BlackBox autorizada. O padrão de laboratório usa consultas de leitura ou ações limitadas; não é um painel de segurança 24/7.

## Segurança

Não publique IPs, hostnames, portas de administração, credenciais, chaves, certificados, inventário, telemetria real ou bancos. O Server não deve executar shell remoto nem aceitar comandos arbitrários por VLP.

Para entender o protocolo e seus limites, veja a pasta [VLP](VLP/README.md).
