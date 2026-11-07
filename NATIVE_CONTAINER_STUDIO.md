# VCore Native Container e VCore Engine Studio

O Native Container é uma plataforma de engenharia para empacotar, identificar, admitir e executar componentes VCore sob contratos e limites explícitos. O VCore Engine Studio é a interface visual de engenharia incluída no kit do Container; ele não é um produto autônomo de runtime.

## Estágio

- **Native Container:** pacote local 0.1.0-experimental.
- **VCore Engine Studio:** 0.2.0-experimental, interface Windows x64.
- Os manifests locais informam que a distribuição do Studio não inclui runtime privado, está sem assinatura Authenticode e não é production-ready.
- Não existe backend OCI completo nem distribuição multiplataforma pronta para cliente.

## Capacidades observadas

- Inspeção e organização de pacotes e workspaces.
- CLI local para admissão, execução e consulta de estado.
- Verificações de identidade, manifesto e integridade do kit antes de encaminhar ações para a CLI.
- Fronteiras explícitas para caminhos, argumentos e capacidades.
- Journal local e modelo de identidade para o runtime.

## O que o Studio não faz

O Studio não é sandbox para código de projeto, não substitui a authority/runtime, não cria por si só confiança de publisher e não concede admission. A execução continua sob responsabilidade do runtime e do sistema operacional. Testes selecionados em fixtures não equivalem à aceitação de uma instalação limpa.

## Stack observada

JavaScript/Node.js e SDK/CLI no Native Container; journal SQLite e adaptadores nativos. O Studio usa interface WinForms em C#/.NET para Windows x64 e se comunica com a CLI incluída no kit.

## Roadmap de confiança

Concluir assinatura da distribuição, instalação e recuperação em Windows limpo, gates de isolamento, operação em reinícios, validação multiplataforma e revisão independente das fronteiras antes de anunciar prontidão comercial.
