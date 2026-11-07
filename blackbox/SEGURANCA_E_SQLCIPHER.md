# BlackBox — segurança, privacidade e SQLCipher

## Dados locais

O BlackBox pode associar sessões a aplicações, títulos de janela, caminhos e metadados de arquivos. Mesmo sem guardar o corpo do documento, um nome de arquivo ou título de janela pode revelar um projeto ou dado pessoal. Informar os usuários, limitar acesso e definir retenção antes do piloto.

## Banco e cifragem

A revisão técnica explícita de 13 de outubro de 2026 encontrou SQLite sem SQLCipher na instalação ativa e um caminho SQLCipher separado no checkout. Não foi localizada prova posterior da migração do banco ativo. Por isso, esta documentação não promete cifragem integral em repouso para a instalação atual.

SQLCipher no checkout foi direcionado a Windows x64 e Node-API específico. Testes de banco temporário, backup cifrado ou presença de um runtime não comprovam que o banco que o cliente usa está cifrado.

## Compartilhamento com o Server

O primeiro contato VLP BlackBox↔Server em loopback chegou a FOUND_UNTRUSTED. Ele não matricula a instalação, não autoriza acesso aos dados e não envia evidências ou trajetórias. O compartilhamento deve ficar negado até haver escopo, finalidade, autorização e contrato operacional próprios.

## Preparação para piloto

- Conferir a build e o banco realmente instalados.
- Restringir as pastas de dados ao usuário e às contas de serviço necessárias.
- Validar backup e restauração em cópia isolada.
- Mostrar estado da captura, última observação e lacunas na interface.
- Não usar o registro para decidir produtividade nem como prova de autoria sem validação independente.

Veja [Segurança e dados do ecossistema](../SECURITY_AND_DATA.md) para os limites por produto.
