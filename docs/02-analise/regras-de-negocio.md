# Regras de Negócio

## Legenda

- **Confirmada:** declarada diretamente na elicitação.
- **Parcial:** o princípio foi declarado, mas faltam parâmetros ou exceções.
- **Pendente:** depende de decisão do negócio e não deve ser implementada como regra definitiva.

| ID | Regra | Origem | Situação | Questão relacionada |
|---|---|---|---|---|
| RN-01 | A quantidade de inscrições confirmadas não pode ultrapassar a capacidade configurada do evento ou atividade. | E-06 | Confirmada | Q-06 |
| RN-02 | Eventos podem ser gratuitos ou pagos; eventos gratuitos não dependem de pagamento. | E-11 | Confirmada | Q-12 |
| RN-03 | Uma inscrição sujeita à confirmação financeira só pode ser liberada depois que o pagamento for confirmado. | E-13 | Confirmada para inscrições aplicáveis | Q-12 |
| RN-04 | O participante só pode cancelar a inscrição quando a política do evento permitir. | E-03, E-08 | Confirmada | Q-01 |
| RN-05 | O direito a reembolso depende das condições definidas para o evento e para o cancelamento. | E-12 | Parcial | Q-02 |
| RN-06 | Certificados ficam disponíveis depois do evento apenas para participantes considerados elegíveis. | E-04 | Parcial | Q-04 |
| RN-07 | Um participante pode se inscrever em vários workshops realizados no mesmo dia. | E-05 | Confirmada | Q-07 |
| RN-08 | A programação pode conter workshops simultâneos. | E-10 | Confirmada | Q-07 |
| RN-09 | Palestrantes só podem consultar participantes de suas próprias atividades. | E-14 | Confirmada quanto ao escopo | Q-08 |
| RN-10 | A lista de espera pode ser utilizada quando a capacidade for atingida. | E-07 | Parcial | Q-03 |
| RN-11 | A inscrição deve produzir um comprovante para o participante. | E-02 | Confirmada quanto à necessidade | Q-10 |
| RN-12 | O destino de uma vaga liberada por cancelamento deve seguir a política de lista de espera do evento. | E-03, E-07 | Pendente | Q-13 |

## Regras não assumidas

Não foram definidos pela elicitação:

- prazo padrão de cancelamento;
- percentual ou prazo de reembolso;
- ordem da lista de espera;
- tempo de reserva de vaga durante pagamento;
- obrigatoriedade de confirmação de presença;
- canais de notificação;
- bloqueio ou alerta para conflito de horário.

Esses pontos permanecem em [lacunas e ambiguidades](lacunas-e-ambiguidades.md).
