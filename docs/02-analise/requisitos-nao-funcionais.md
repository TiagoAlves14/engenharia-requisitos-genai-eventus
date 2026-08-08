# Requisitos Não Funcionais Propostos

## Aviso de procedência

A observação `O-09` afirma que segurança, desempenho, disponibilidade, acessibilidade e privacidade **não foram levantados**. Portanto, os itens abaixo são propostas técnicas para discussão, não requisitos acordados com a Eventus.

As métricas também são pontos de partida e devem ser ajustadas com a equipe de TI e os responsáveis pelo negócio.

| ID | Categoria | Proposta | Critério de verificação proposto | Situação |
|---|---|---|---|---|
| RNF-01 | Autenticação e autorização | Operações protegidas devem exigir identidade autenticada e permissão compatível com participante, organizador, financeiro ou palestrante. | Testes de autorização devem negar todas as combinações de perfil e operação não permitidas. | A validar |
| RNF-02 | Segurança | Credenciais e dados pessoais devem ser protegidos em armazenamento e trânsito segundo os padrões aprovados pela equipe de TI. | Revisão de segurança deve comprovar ausência de senha em texto puro e proteção das comunicações externas. | A validar |
| RNF-03 | Privacidade | O tratamento de dados deve respeitar finalidade, necessidade e menor privilégio, especialmente no acesso de palestrantes. | A consulta do palestrante deve retornar somente os campos aprovados em Q-08 e apenas para suas atividades. | A validar |
| RNF-04 | Auditabilidade | Confirmações de pagamento, cancelamentos, reembolsos e alterações de capacidade devem registrar autor, data, hora e resultado. | Amostra de operações deve possuir trilha completa e não editável pelos perfis operacionais. | A validar |
| RNF-05 | Desempenho | O catálogo de eventos deve responder em até 2 segundos no percentil 95 sob a carga acordada. | Teste de carga com volume definido pela Eventus e resultado p95 menor ou igual a 2 segundos. | A validar |
| RNF-06 | Desempenho | A solicitação de inscrição deve responder em até 3 segundos no percentil 95, desconsiderando indisponibilidade de serviços externos. | Teste de carga com resultado p95 menor ou igual a 3 segundos. | A validar |
| RNF-07 | Confiabilidade e concorrência | Inscrições simultâneas nunca devem produzir quantidade de confirmados superior à capacidade. | No pico de concorrência acordado, o total confirmado deve permanecer menor ou igual à capacidade em 100% das execuções. | Derivado de E-06; validar a carga |
| RNF-08 | Disponibilidade | O serviço deve manter disponibilidade mensal de 99,5% durante janelas publicadas de inscrição. | Relatório mensal de monitoramento, excluindo apenas manutenções previamente acordadas. | A validar |
| RNF-09 | Acessibilidade | As jornadas principais devem atender ao nível AA das diretrizes WCAG 2.2. | Auditoria automática e manual deve verificar teclado, foco, contraste, rótulos e compatibilidade com leitor de tela. | A validar |
| RNF-10 | Usabilidade | Pelo menos 90% dos participantes do teste devem concluir inscrição e cancelamento permitido sem ajuda. | Teste moderado com público representativo e registro da taxa de conclusão e erros críticos. | A validar |
| RNF-11 | Confiabilidade de notificações | Falhas temporárias no canal de comunicação não devem perder comprovantes ou notificações. | Mensagens com falha devem ser reenviadas sem duplicidade e possuir estado consultável. | A validar |
| RNF-12 | Manutenibilidade | Regras de negócio e critérios de aceitação devem permanecer vinculados por identificadores estáveis. | Revisão de cada mudança deve demonstrar a atualização dos artefatos afetados na matriz de rastreabilidade. | A validar |

## Decisões necessárias

Antes de transformar estas propostas em requisitos aprovados, é necessário responder Q-08, Q-09 e Q-11, conhecer volume, horários críticos, classificação dos dados e capacidade operacional da equipe de TI.
