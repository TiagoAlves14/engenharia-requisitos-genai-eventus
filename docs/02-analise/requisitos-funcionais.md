# Requisitos Funcionais

## Critérios de classificação

- **Confirmado:** sustentado diretamente por interesse ou declaração da elicitação.
- **Derivado:** necessário para viabilizar uma necessidade confirmada; a justificativa é informada.
- **A validar:** comportamento sugerido que depende de decisão dos stakeholders.

A prioridade MoSCoW é **preliminar** e precisa ser validada. Um requisito confirmado pode manter detalhes pendentes nas [questões abertas](lacunas-e-ambiguidades.md).

## Catálogo

| ID | Requisito | Origem | Situação | Prioridade preliminar | Observação |
|---|---|---|---|---|---|
| RF-01 | O sistema deve apresentar um catálogo unificado dos eventos disponíveis. | E-01 | Confirmado | Must | Critérios de disponibilidade e filtros não foram definidos. |
| RF-02 | O sistema deve permitir que organizadores criem eventos. | S-02 | Confirmado | Must | Campos obrigatórios e fluxo de publicação precisam de validação. |
| RF-03 | O sistema deve apresentar as informações necessárias para que o participante decida sobre a inscrição. | E-01, S-01 | Derivado | Must | Derivado porque não é possível escolher e se inscrever sem identificar o evento e sua programação. |
| RF-04 | O sistema deve permitir que participantes se inscrevam em eventos e atividades disponíveis. | S-01, E-05 | Confirmado | Must | A confirmação pode depender de vaga e pagamento. |
| RF-05 | O sistema deve permitir que o participante acompanhe suas inscrições e respectivos estados. | S-01 | Confirmado | Must | Os estados ainda precisam ser definidos. |
| RF-06 | O sistema deve disponibilizar um comprovante após a inscrição. | E-02 | Confirmado | Must | O significado do comprovante em eventos pagos está em Q-10. |
| RF-07 | O sistema deve permitir que o participante solicite o cancelamento da própria inscrição sem contato manual com a organização, quando a política do evento permitir. | E-03, E-08 | Confirmado | Should | Prazo e efeitos financeiros estão em Q-01 e Q-02. |
| RF-08 | O sistema deve permitir que o participante elegível emita certificado depois do evento. | E-04 | Confirmado | Should | A condição de elegibilidade está em Q-04. |
| RF-09 | O sistema deve permitir a inscrição do participante em vários workshops realizados no mesmo dia. | E-05 | Confirmado | Should | O tratamento de sobreposição de horários está em Q-07. |
| RF-10 | O sistema deve controlar automaticamente a ocupação e as vagas de cada evento ou atividade. | E-06 | Confirmado | Must | A reserva durante pagamento está em Q-06. |
| RF-11 | O sistema deve suportar lista de espera quando um evento ou atividade atingir a capacidade. | E-07 | Confirmado quanto à necessidade | Should | Ordenação, aceite e promoção estão em Q-03. |
| RF-12 | O sistema deve permitir que organizadores acompanhem a quantidade de inscritos em tempo real. | E-09 | Confirmado | Should | O significado mensurável de “tempo real” está em Q-11. |
| RF-13 | O sistema deve permitir que workshops com horários coincidentes sejam programados simultaneamente. | E-10 | Confirmado | Should | Isso não define se um participante pode escolher workshops sobrepostos. |
| RF-14 | O sistema deve permitir a configuração de eventos gratuitos e pagos. | E-11 | Confirmado | Must | Formas e processo de pagamento não foram definidos. |
| RF-15 | O sistema deve registrar e permitir que a equipe financeira confirme pagamentos das inscrições para as quais essa confirmação seja exigida. | E-13 | Confirmado | Must | O conjunto de inscrições aplicáveis está em Q-12. |
| RF-16 | O sistema deve permitir que a equipe financeira registre e acompanhe reembolsos. | S-03, E-12 | Confirmado quanto à necessidade | Should | Critérios, valores e prazos estão em Q-02. |
| RF-17 | O sistema deve permitir que palestrantes consultem sua programação e a lista de participantes de suas próprias atividades. | S-04, E-14 | Confirmado | Should | Os campos visíveis estão em Q-08. |
| RF-18 | O sistema deve permitir que organizadores acompanhem e gerenciem os participantes de seus eventos. | S-02 | Confirmado quanto à necessidade | Should | As operações permitidas precisam ser detalhadas em Q-14. |
| RF-19 | O sistema deve enviar comprovantes e notificações pelos canais aprovados pelo negócio. | O-05 | A validar | Could | Canais, gatilhos e conteúdo estão em Q-05. |
| RF-20 | O sistema deve registrar presença quando essa informação for exigida para emissão de certificados. | O-04 | A validar | Could | Só será necessário se a resposta de Q-04 vincular certificado à presença. |
| RF-21 | O sistema deve aplicar a política definida para tentativas de inscrição em atividades com horários conflitantes. | O-07 | A validar | Should | Bloqueio, alerta ou permissão dependem de Q-07. |

## Verificação de escopo

- Todos os requisitos possuem origem rastreável.
- Os itens `RF-19` a `RF-21` não são decisões aprovadas; representam capacidades condicionadas às questões abertas.
- Não foram incluídos login social, QR Code, aplicativo móvel, recomendações ou relatórios avançados, pois não possuem origem na elicitação.
