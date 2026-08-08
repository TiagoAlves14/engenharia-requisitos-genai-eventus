# Casos de Uso Seletivos

Foram escolhidos somente três fluxos com múltiplas decisões e exceções. Funcionalidades simples permanecem representadas por histórias e critérios de aceitação.

## UC-01 - Solicitar inscrição

| Campo | Descrição |
|---|---|
| Objetivo | Registrar a solicitação de participação em evento ou atividade sem ultrapassar a capacidade. |
| Ator principal | Participante. |
| Atores de apoio | Equipe financeira, quando houver confirmação manual de pagamento. |
| Pré-condições | Evento disponível; participante apto a solicitar inscrição. |
| Pós-condição mínima | Solicitação registrada em estado coerente, sem exceder a capacidade. |
| Requisitos | RF-04, RF-06, RF-09, RF-10, RF-14, RF-15, RF-21. |
| Questões bloqueantes | Q-03, Q-06, Q-07, Q-10 e Q-12. |

### Fluxo principal provisório

1. O participante consulta o catálogo e seleciona um evento ou atividade.
2. O sistema apresenta as informações disponíveis para a decisão.
3. O participante solicita a inscrição.
4. O sistema verifica a política de conflito de horário, quando aplicável.
5. O sistema verifica a capacidade.
6. O sistema identifica se a inscrição é gratuita ou sujeita a pagamento e confirmação financeira.
7. O sistema registra a solicitação no estado definido pela política aprovada.
8. O sistema disponibiliza o comprovante correspondente.

### Fluxos alternativos e exceções

- **A1 - Capacidade atingida:** aplicar lista de espera, se habilitada; detalhes dependem de Q-03.
- **A2 - Conflito de horário:** o resultado depende de Q-07.
- **A3 - Confirmação financeira necessária:** estado, reserva e comprovante dependem de Q-06, Q-10 e Q-12.
- **A4 - Concorrência pela última vaga:** somente uma solicitação pode resultar em confirmação.

## UC-02 - Cancelar inscrição e tratar efeitos

| Campo | Descrição |
|---|---|
| Objetivo | Permitir cancelamento autônomo quando autorizado e encaminhar corretamente seus efeitos. |
| Ator principal | Participante. |
| Ator de apoio | Equipe financeira, quando houver reembolso. |
| Pré-condições | Inscrição pertencente ao participante e política de cancelamento disponível. |
| Pós-condição mínima | Inscrição mantida ou cancelada de forma rastreável. |
| Requisitos | RF-07, RF-10, RF-16. |
| Questões bloqueantes | Q-01, Q-02 e Q-13. |

### Fluxo principal provisório

1. O participante acessa suas inscrições.
2. Seleciona a inscrição e solicita o cancelamento.
3. O sistema verifica se a política permite a operação naquela condição.
4. O participante confirma a solicitação.
5. O sistema registra o cancelamento.
6. O sistema aplica o tratamento de vaga definido em Q-13.
7. Quando aplicável, o sistema encaminha ou registra o reembolso conforme Q-02.

### Fluxos alternativos e exceções

- **A1 - Cancelamento proibido:** manter a inscrição e informar a restrição.
- **A2 - Prazo encerrado:** comportamento depende de Q-01.
- **A3 - Sem direito a reembolso:** informar a regra aprovada sem alterar indevidamente o pagamento.

## UC-03 - Oferecer vaga à lista de espera

| Campo | Descrição |
|---|---|
| Objetivo | Preencher uma vaga liberada respeitando a política de lista de espera. |
| Ator principal | Organizador, responsável pela política de ocupação do evento. |
| Ator secundário | Participante em espera; o fluxo pode ser iniciado automaticamente pela liberação de uma vaga. |
| Pré-condições | Lista de espera habilitada, candidato aguardando e vaga disponível. |
| Pós-condição mínima | Vaga oferecida ou liberada sem violar a ordenação aprovada. |
| Requisitos | RF-10, RF-11, RF-19. |
| Questões bloqueantes | Q-03, Q-05 e Q-13. |

### Fluxo provisório

1. Uma vaga é liberada.
2. O sistema identifica o próximo candidato conforme a ordenação aprovada.
3. O sistema comunica a oferta pelo canal definido.
4. O candidato aceita ou deixa expirar o prazo.
5. Em caso de aceite, o sistema aplica a política de pagamento e confirmação.
6. Em caso de recusa ou expiração, o sistema passa ao próximo candidato.

> Este caso de uso registra a estrutura necessária, mas não pode ser finalizado antes das respostas a Q-03, Q-05 e Q-13.
