# BlackBox Governance

O BlackBox organiza memória operacional local para que uma equipe possa investigar o que foi observado durante o trabalho de agentes de IA: sessões, chamadas, ações, contexto, arquivos relacionados, trajetórias e consumo quando há uma fonte disponível.

## Estágio atual

O checkout identificado como **2.1.0** sustenta uma **demonstração assistida em Windows**. A revisão de lançamento de 3–4 de novembro de 2026 não aprovou venda aberta. Um piloto comercial ainda depende de instalação limpa e licenciada, captura repetível, atendimento de falhas de sinal e reconciliação comercial.

## O que a investigação apresenta

- Linha do tempo de sessões e turnos observados.
- Contexto de aplicação e referências de arquivos quando a fonte registra esses fatos.
- Ações observadas separadas de correlações temporais e hipóteses.
- Tokens e cotas conforme a fonte e o período informados; cobrança do provedor somente quando confirmada por uma fonte apropriada.
- Histórico local e rankings de recorrência, com cobertura e lacunas visíveis.
- Primeiro contato VLP com o VCore Server em perfil de laboratório.

Um caminho declarado pela sessão não é prova do percurso completo. Proximidade de horário não comprova que uma IA alterou um arquivo. Uma lista de arquivos ou aplicações recorrentes não mede produtividade nem valor econômico. O produto deve dizer “desconhecido” quando a evidência não decide.

## Stack observada

Node.js, React/Vite, SQLite, integração local com sistema de arquivos e sensores de aplicação. Há serviços separados para API, eventos, interface e notificações. A arquitetura mantém a memória detalhada nesta máquina por padrão; qualquer envio para o Server precisa de contrato, finalidade e autorização próprios.

## Segurança e limites de cobertura

- A demonstração de primeiro contato BlackBox↔Server em loopback alcançou o estado “FOUND_UNTRUSTED”. Não representa matrícula, autorização empresarial, transmissão de trajetórias ou coleta contínua pelo Server.
- A revisão mais recente de banco encontrada, de 13/10, registrou que a instalação ativa usava SQLite sem SQLCipher enquanto o checkout tinha um caminho SQLCipher diferente. Não há evidência posterior de migração segura do banco ativo. A distribuição não deve prometer cifragem integral em repouso até isso ser verificado.
- A memória pode ter lacunas, fontes atrasadas e limites de histórico. Reiniciar captura não recupera fatos que não foram registrados.
- Custo estimado, cota da conta, tokens observados e cobrança do provedor são medidas diferentes.
- Arquivos, títulos de janela e nomes de processos podem conter dados pessoais ou de negócio. Configure acesso, retenção e compartilhamento antes de qualquer piloto.

## Próximo gate para clientes

Demonstrar numa instalação candidata uma sessão autorizada que percorra sessão → chamada → ação → artefato → evidência → exportação, incluindo pelo menos um caso de lacuna e um reinício. Reconciliar a cobrança com uma fonte autorizada. Validar isolamento entre organizações antes de oferecer gestão centralizada de frota.

## Referências

- [Visão pública do BlackBox](https://www.voigtcore.com.br/)
- [Protocolo VLP/1](VLP_PROTOCOL.md)
- [Segurança, dados e SQLCipher](SECURITY_AND_DATA.md)
