# VCore Server — operação e prontidão

## Perfis

- **Desenvolvimento:** base local e fixtures controladas.
- **Laboratório:** alvos explicitamente configurados, dados de teste ou ativos autorizados, rede e certificados temporários dedicados.
- **Produção:** ainda não aprovada para o Server 0.8.0 descrito nesta documentação.

Não reutilize certificados ou arquivos de perfil de laboratório numa instalação de cliente. A comunicação precisa validar o pin e a identidade esperada do Server.

## O que precisa estar visível ao operador

- Estado de serviço separado de estado de cada agente.
- Último contato, cobertura e fonte do dado.
- Identidade observada separada de organização e dispositivo matriculados.
- Ações disponíveis, responsável, justificativa e resultado registrado.
- Falhas, lacunas, certificados expirados e recuperação necessária.

## Gate antes de produção

1. Autenticação de operador e autorização por organização/função.
2. Isolamento comprovado entre organizações em APIs, banco, logs e exports.
3. PKI, matrícula, rotação, expiração e revogação testadas em ambiente operacional.
4. Instalação, atualização, backup, restauração e rollback em máquina limpa.
5. Capacidade, retenção, alertas e resposta a incidente documentados.
6. Revisão independente de segurança e privacidade antes de armazenar evidências de clientes.

## Fronteira atual BlackBox

O Server reconhece a família BlackBox no primeiro contato de laboratório, com capacidades declaradas limitadas. O máximo confirmado é FOUND_UNTRUSTED. Não há ingestão operacional de evidências, autorização empresarial nem gestão de frota BlackBox nesse estado.
