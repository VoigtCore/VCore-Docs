# Catálogo de produtos e estágio

**Revisado em 7 de novembro de 2026.** O estágio abaixo se baseia nas versões públicas e nas evidências de engenharia disponíveis nesta data. Não é uma certificação, auditoria independente nem promessa de lançamento.

| Produto | Estágio atual | Tecnologia principal observada | Próximo gate de confiança |
|---|---|---|---|
| VCore Pulse IA Monitor | 2.1.1 é descrito como ciclo estável público; 2.2 está em desenvolvimento | Node.js, React, Vite, instrumentação local, SQLite/SQLCipher em caminhos distintos e serviços PostgreSQL no plano comercial | Release reprodutível, assinatura e cobertura por plataforma; validar cifragem do banco do runtime por versão |
| BlackBox Governance | 2.1.0 no checkout; demonstração assistida em Windows. Venda aberta bloqueada | Node.js, React, Vite, SQLite, coleta local e memória temporal | Instalação limpa, captura repetível, trilha sessão→chamada→ação→artefato, cobrança reconciliada e política comercial consistente |
| VCore Server | 0.8.0; desenvolvimento local e integração de laboratório | Node.js, JavaScript, SQLite legado, HTTP local e conectores explícitos de rede, incluindo net-snmp | Login, isolamento por organização, instalação/recuperação e ciclo de identidade/certificados de produção |
| VCore Link Protocol (VLP/1) | Núcleo 1.0 implementado; integração de primeiro contato limitada | JavaScript/Node.js, Ed25519, TLS 1.3/mTLS nos ensaios locais | PKI operacional, matrícula, rotação e revogação, autorização e fila durável em ambiente de cliente |
| VCore Native Container | 0.1.0-experimental; engenharia | Node.js, JavaScript, SDK/CLI, AppContainer no Windows e journal SQLite | Gates de instalação e reinício em máquina limpa, isolamento completo, assinatura da distribuição e revisão independente |
| VCore Engine Studio | 0.2.0-experimental; interface Windows x64 dentro do pacote Native Container | C#/.NET WinForms e CLI Node.js incluída no kit | Assinatura Authenticode, testes de instalação e acessibilidade; deixar explícito que a GUI não é sandbox |

## Pulse IA Monitor

O perfil público da VoigtCore informa que a versão **2.1.1** é o ciclo estável e que a evolução **2.2** está em desenvolvimento. O checkout local usa metadados 2.2.0; esse número de desenvolvimento não deve ser apresentado como release publicado.

## BlackBox Governance

O BlackBox reúne sinais locais para investigar sessões de IA, atividade, trajetórias, arquivos e consumo. A revisão de lançamento de 3–4 de novembro conclui que há maturidade para demonstração assistida, mas mantém bloqueada a venda aberta. O piloto depende de instalação independente, captura verificável, licença e preço coerentes, e evidência ponta a ponta.

## VCore Server e VLP

O Server tem cadastro e memória de ativos, linha do tempo, proveniência e telas de operação em desenvolvimento. O primeiro contato do BlackBox no laboratório pode alcançar o estado “FOUND_UNTRUSTED”: isso confirma contato autenticado dentro daquele ensaio, mas não matrícula, confiança empresarial, autorização nem ingestão contínua de dados.

## Native Container e Studio

O Native Container e o Studio são ferramentas de engenharia. O Studio está dentro do pacote de distribuição do Native Container e não é um runtime separado. Seu manifesto local declara versão experimental, pacote sem assinatura Authenticode e estado production-ready falso.

## Sobre as tecnologias citadas

SQLite, SQLCipher, TLS, Ed25519, AES-GCM e AppContainer descrevem componentes ou caminhos específicos. A presença de um componente no código ou em testes não significa que esteja habilitado no instalador ou banco ativo de todas as plataformas. Veja [Segurança, dados e SQLCipher](SECURITY_AND_DATA.md).
