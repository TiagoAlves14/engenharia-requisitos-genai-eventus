# Matriz de Rastreabilidade

A matriz permite navegar da necessidade original até sua especificação e também verificar se um requisito apareceu sem fonte.

## Necessidades elicitadas

| Origem | Necessidade | Requisitos | Regras | História | Critérios principais | Questão aberta |
|---|---|---|---|---|---|---|
| E-01 | Catálogo unificado de eventos | RF-01, RF-03 | - | HU-01 | CA-01.1, CA-01.2 | - |
| E-02 | Comprovante após inscrição | RF-06 | RN-11 | HU-03 | CA-03.1, CA-03.2 | Q-10 |
| E-03 | Cancelamento autônomo | RF-07 | RN-04, RN-12 | HU-05 | CA-05.1, CA-05.2 | Q-01, Q-02, Q-13 |
| E-04 | Certificado após evento | RF-08, RF-20 | RN-06 | HU-06 | CA-06.1 | Q-04 |
| E-05 | Vários workshops no mesmo dia | RF-04, RF-09, RF-21 | RN-07 | HU-07 | CA-07.1, CA-07.2 | Q-07 |
| E-06 | Controle automático de vagas | RF-10 | RN-01 | HU-08 | CA-08.1, CA-08.2 | Q-06 |
| E-07 | Lista de espera | RF-11, RF-21 | RN-10, RN-12 | HU-09 | CA-09.1, CA-09.2 | Q-03, Q-13 |
| E-08 | Eventos que não permitem cancelamento | RF-07 | RN-04 | HU-05 | CA-05.2 | Q-01 |
| E-09 | Quantidade de inscritos em tempo real | RF-12 | - | HU-10 | CA-10.1, CA-10.2 | Q-11 |
| E-10 | Workshops simultâneos | RF-13, RF-21 | RN-08 | HU-07 | CA-07.2 | Q-07 |
| E-11 | Eventos gratuitos e pagos | RF-14 | RN-02 | HU-03 | CA-03.1, CA-03.2 | Q-12 |
| E-12 | Situações com e sem reembolso | RF-16 | RN-05 | HU-12 | CA-12.1 | Q-02 |
| E-13 | Confirmação financeira antes da liberação | RF-15 | RN-03 | HU-11 | CA-11.1, CA-11.2 | Q-06, Q-10, Q-12 |
| E-14 | Lista de participantes para palestrante | RF-17 | RN-09 | HU-13 | CA-13.1, CA-13.2 | Q-08 |

## Interesses complementares dos stakeholders

| Origem | Interesse | Requisitos | História |
|---|---|---|---|
| S-01 | Inscrever-se, acompanhar, cancelar e emitir certificado | RF-04, RF-05, RF-07, RF-08 | HU-03, HU-04, HU-05, HU-06 |
| S-02 | Criar eventos, controlar vagas e gerenciar participantes | RF-02, RF-10, RF-12, RF-18 | HU-02, HU-08, HU-10, HU-14; o detalhamento de gestão depende de Q-14. |
| S-03 | Confirmar pagamentos e controlar reembolsos | RF-15, RF-16 | HU-11, HU-12 |
| S-04 | Consultar programação e participantes | RF-17 | HU-13 |
| S-05 | Desenvolver e manter o sistema | Não confirma requisitos específicos | Stakeholder técnico a consultar na validação das propostas RNF-01 a RNF-12, cuja lacuna foi registrada em O-09. |

## Requisitos derivados ou condicionais

| Requisito | Origem | Justificativa | Tratamento |
|---|---|---|---|
| RF-03 | E-01, S-01 | A decisão de inscrição exige informações do evento e da programação. | Mantido como derivado. |
| RF-19 | O-05 | A elicitação menciona envio, mas não define canal nem gatilhos. | Condicionado a Q-05. |
| RF-20 | O-04 | Registro de presença só é necessário se definir elegibilidade para certificado. | Condicionado a Q-04. |
| RF-21 | O-07 | O sistema precisará aplicar a política escolhida para conflitos. | Condicionado a Q-07. |
| RNF-01 a RNF-12 | O-09 | A ausência de RNFs é uma lacuna explícita. | Propostas, todas marcadas para validação. |

## Verificação de cobertura

- As 14 declarações de entrevista possuem requisito e história correspondentes.
- As nove observações originais aparecem nas questões Q-01 a Q-09.
- As cinco ambiguidades adicionais aparecem em Q-10 a Q-14.
- Nenhum item condicional é apresentado como requisito confirmado.
