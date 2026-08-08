# Histórias de Usuário

## Priorização

A classificação MoSCoW abaixo é uma proposta para organizar o trabalho. Ela não representa uma priorização aprovada pelos stakeholders.

## Participante

### HU-01 - Consultar eventos

**Como** participante,  
**quero** visualizar os eventos disponíveis em um único catálogo,  
**para** encontrar opções de participação.

- Origem: E-01
- Requisitos: RF-01, RF-03
- Prioridade preliminar: Must
- Critérios: CA-01.1 e CA-01.2

### HU-03 - Inscrever-se em evento ou atividade

**Como** participante,  
**quero** solicitar minha inscrição em um evento ou atividade,  
**para** participar da programação escolhida.

- Origem: S-01, E-02, E-11, E-13
- Requisitos: RF-04, RF-06, RF-10, RF-14, RF-15, RF-19
- Regras: RN-01, RN-02, RN-03, RN-11
- Prioridade preliminar: Must
- Questões: Q-05, Q-06, Q-10 e Q-12
- Critérios: CA-03.1 a CA-03.4

### HU-04 - Acompanhar inscrições

**Como** participante,  
**quero** consultar minhas inscrições e seus estados,  
**para** saber se estão pendentes, confirmadas ou canceladas.

- Origem: S-01
- Requisito: RF-05
- Prioridade preliminar: Must
- Critério: CA-04.1

### HU-05 - Cancelar inscrição

**Como** participante,  
**quero** solicitar o cancelamento da minha inscrição pelo próprio sistema,  
**para** não depender de contato manual com a organização.

- Origem: E-03, E-08
- Requisito: RF-07
- Regras: RN-04, RN-05, RN-12
- Prioridade preliminar: Should
- Questões: Q-01, Q-02 e Q-13
- Critérios: CA-05.1 a CA-05.3

### HU-06 - Emitir certificado

**Como** participante elegível,  
**quero** emitir meu certificado depois do evento,  
**para** comprovar minha participação.

- Origem: E-04
- Requisitos: RF-08, RF-20
- Regra: RN-06
- Prioridade preliminar: Should
- Questão: Q-04
- Critério: CA-06.1

### HU-07 - Participar de vários workshops no mesmo dia

**Como** participante,  
**quero** me inscrever em vários workshops realizados no mesmo dia,  
**para** aproveitar diferentes atividades da programação.

- Origem: E-05, E-10
- Requisitos: RF-09, RF-13, RF-21
- Regras: RN-07, RN-08
- Prioridade preliminar: Should
- Questão: Q-07
- Critérios: CA-07.1 e CA-07.2

## Organizador

### HU-02 - Criar evento

**Como** organizador,  
**quero** criar um evento no sistema,  
**para** disponibilizá-lo aos participantes e administrar suas inscrições.

- Origem: S-02
- Requisito: RF-02
- Prioridade preliminar: Must
- Critério: CA-02.1

### HU-08 - Controlar vagas

**Como** organizador,  
**quero** que o sistema controle automaticamente a ocupação,  
**para** impedir confirmações acima da capacidade.

- Origem: E-06
- Requisito: RF-10
- Regra: RN-01
- Prioridade preliminar: Must
- Questão: Q-06
- Critérios: CA-08.1 e CA-08.2

### HU-09 - Gerenciar lista de espera

**Como** organizador,  
**quero** utilizar uma lista de espera quando não houver vagas,  
**para** organizar a demanda excedente.

- Origem: E-07
- Requisitos: RF-11, RF-19, RF-21
- Regras: RN-10, RN-12
- Prioridade preliminar: Should
- Questões: Q-03, Q-05 e Q-13
- Critérios: CA-09.1 e CA-09.2

### HU-10 - Acompanhar quantidade de inscritos

**Como** organizador,  
**quero** acompanhar a quantidade de inscritos em tempo real,  
**para** controlar a ocupação do evento.

- Origem: E-09
- Requisito: RF-12
- Prioridade preliminar: Should
- Questão: Q-11
- Critérios: CA-10.1 e CA-10.2

### HU-14 - Gerenciar participantes do evento

**Como** organizador,  
**quero** acompanhar e realizar as operações autorizadas sobre os participantes dos meus eventos,  
**para** administrar a participação sem acessar ou alterar informações indevidas.

- Origem: S-02
- Requisito: RF-18
- Prioridade preliminar: Should
- Questão: Q-14
- Critérios: CA-14.1 e CA-14.2

## Equipe financeira

### HU-11 - Confirmar pagamento

**Como** integrante da equipe financeira,  
**quero** confirmar o pagamento de uma inscrição aplicável,  
**para** permitir sua liberação conforme a regra do evento.

- Origem: E-13
- Requisito: RF-15
- Regra: RN-03
- Prioridade preliminar: Must
- Questões: Q-06, Q-10 e Q-12
- Critérios: CA-11.1 e CA-11.2

### HU-12 - Controlar reembolso

**Como** integrante da equipe financeira,  
**quero** registrar e acompanhar reembolsos,  
**para** aplicar a política definida para cada situação.

- Origem: S-03, E-12
- Requisito: RF-16
- Regra: RN-05
- Prioridade preliminar: Should
- Questão: Q-02
- Critério: CA-12.1

## Palestrante

### HU-13 - Consultar programação e participantes

**Como** palestrante,  
**quero** consultar minha programação e os participantes das minhas atividades,  
**para** preparar e conduzir cada sessão.

- Origem: S-04, E-14
- Requisito: RF-17
- Regra: RN-09
- Prioridade preliminar: Should
- Questão: Q-08
- Critérios: CA-13.1 e CA-13.2

## Condição para refinamento

Histórias vinculadas a uma questão `Q-nn` não podem ser consideradas prontas para desenvolvimento enquanto a decisão necessária não estiver registrada e seus critérios de aceitação não forem atualizados.
