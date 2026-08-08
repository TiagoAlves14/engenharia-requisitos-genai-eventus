# Critérios de Aceitação

Os critérios usam o formato Dado/Quando/Então. Cenários dependentes de questões abertas são identificados como **bloqueados** ou **parciais**, evitando transformar uma hipótese da IA em regra do negócio.

## HU-01 - Consultar eventos

### CA-01.1 - Catálogo com eventos disponíveis

- **Dado** que existem eventos disponíveis para inscrição
- **Quando** o participante acessa o catálogo
- **Então** o sistema apresenta esses eventos em um único lugar
- **E** permite acessar as informações necessárias para decidir sobre a inscrição

### CA-01.2 - Catálogo sem eventos

- **Dado** que não existem eventos disponíveis
- **Quando** o participante acessa o catálogo
- **Então** o sistema informa que não há eventos disponíveis

## HU-02 - Criar evento

### CA-02.1 - Cadastro válido - parcial

- **Dado** que o usuário possui perfil de organizador
- **E** os campos obrigatórios do evento foram definidos pelo negócio
- **Quando** ele informa dados válidos e solicita a criação
- **Então** o sistema registra o evento e sua capacidade

> Os campos e estados de publicação ainda precisam ser refinados com os organizadores.

## HU-03 - Inscrever-se em evento ou atividade

### CA-03.1 - Inscrição em evento gratuito com vaga

- **Dado** que o evento é gratuito e possui vaga disponível
- **Quando** o participante solicita a inscrição
- **Então** o sistema registra a inscrição sem exigir pagamento
- **E** disponibiliza o comprovante previsto em RN-11

### CA-03.2 - Inscrição sujeita a pagamento - bloqueado

O resultado definitivo depende de Q-06, Q-10 e Q-12. É necessário definir quais inscrições aguardam pagamento, em que momento ocupam vaga e qual comprovante é emitido antes da confirmação.

### CA-03.3 - Evento sem vaga - parcial

- **Dado** que a capacidade foi atingida
- **Quando** o participante solicita a inscrição
- **Então** o sistema não cria uma inscrição confirmada acima da capacidade
- **E** aplica a política de lista de espera, se ela estiver habilitada

> A entrada e a posição na lista dependem de Q-03.

### CA-03.4 - Solicitações concorrentes

- **Dado** que resta uma única vaga
- **Quando** duas solicitações tentam confirmá-la simultaneamente
- **Então** no máximo uma inscrição é confirmada
- **E** o total de confirmados não ultrapassa a capacidade

## HU-04 - Acompanhar inscrições

### CA-04.1 - Consulta das próprias inscrições

- **Dado** que o participante possui inscrições registradas
- **Quando** acessa sua área de inscrições
- **Então** visualiza somente suas inscrições e seus estados atuais

## HU-05 - Cancelar inscrição

### CA-05.1 - Cancelamento permitido

- **Dado** que a política do evento permite o cancelamento naquela condição
- **Quando** o participante confirma a solicitação
- **Então** o sistema cancela a inscrição
- **E** registra a operação

### CA-05.2 - Cancelamento não permitido

- **Dado** que a política do evento não permite o cancelamento naquela condição
- **Quando** o participante tenta cancelar
- **Então** o sistema mantém a inscrição
- **E** informa de forma clara que o cancelamento não é permitido

### CA-05.3 - Reembolso e destino da vaga - bloqueado

O efeito financeiro e o destino da vaga dependem de Q-01, Q-02 e Q-13.

## HU-06 - Emitir certificado

### CA-06.1 - Certificado de participante elegível - parcial

- **Dado** que o evento foi encerrado
- **E** o participante atende à regra de elegibilidade aprovada
- **Quando** solicita o certificado
- **Então** o sistema disponibiliza o certificado correspondente

> A elegibilidade e a necessidade de presença dependem de Q-04.

## HU-07 - Participar de vários workshops no mesmo dia

### CA-07.1 - Workshops sem sobreposição

- **Dado** que o participante já está inscrito em um workshop
- **E** outro workshop ocorre no mesmo dia sem sobreposição de horário
- **Quando** solicita a segunda inscrição
- **Então** o sistema permite prosseguir, respeitando vaga e pagamento

### CA-07.2 - Workshops sobrepostos - bloqueado

O sistema não deve bloquear, alertar ou permitir a inscrição até que Q-07 defina a política de conflito.

## HU-08 - Controlar vagas

### CA-08.1 - Limite da capacidade

- **Dado** que um evento possui capacidade configurada
- **Quando** inscrições são confirmadas
- **Então** o total confirmado permanece menor ou igual à capacidade

### CA-08.2 - Atualização da ocupação - parcial

- **Dado** que uma inscrição muda de estado
- **Quando** a mudança passa a ocupar ou liberar vaga conforme a política aprovada
- **Então** o sistema atualiza a ocupação de forma consistente

> Reserva durante pagamento e liberação após cancelamento dependem de Q-06 e Q-13.

## HU-09 - Gerenciar lista de espera

### CA-09.1 - Entrada na lista - parcial

- **Dado** que a capacidade foi atingida
- **E** a lista de espera está habilitada
- **Quando** o participante manifesta interesse
- **Então** o sistema registra sua entrada sem criar inscrição confirmada

> A ordenação ainda depende de Q-03.

### CA-09.2 - Promoção para vaga - bloqueado

Promoção, prazo de aceite, notificação e tratamento de ausência de resposta dependem de Q-03, Q-05 e Q-13.

## HU-10 - Acompanhar quantidade de inscritos

### CA-10.1 - Total coerente - parcial

- **Dado** que existem inscrições registradas
- **Quando** o organizador consulta o painel
- **Então** o sistema apresenta a quantidade de inscritos conforme os estados definidos pelo negócio

> Q-11 deve definir quais estados compõem o indicador.

### CA-10.2 - Atualização em tempo real - bloqueado

O atraso máximo de atualização e o volume de referência dependem de Q-11 e Q-09.

## HU-11 - Confirmar pagamento

### CA-11.1 - Confirmação financeira - parcial

- **Dado** que uma inscrição exige confirmação financeira
- **E** o pagamento está pendente
- **Quando** a equipe financeira confirma o recebimento
- **Então** o sistema registra a confirmação
- **E** aplica a regra aprovada para liberação e ocupação da vaga

> A mudança de estado depende de Q-06, Q-10 e Q-12.

### CA-11.2 - Confirmação repetida

- **Dado** que o mesmo pagamento já foi confirmado
- **Quando** a confirmação é recebida novamente
- **Então** o sistema não cria nova inscrição nem duplica a ocupação da vaga

## HU-12 - Controlar reembolso

### CA-12.1 - Aplicação da política - bloqueado

Motivo elegível, valor, prazo, aprovador e estado do reembolso dependem integralmente de Q-02.

## HU-13 - Consultar programação e participantes

### CA-13.1 - Restrição às próprias atividades

- **Dado** que o palestrante está associado a uma atividade
- **Quando** consulta sua programação e participantes
- **Então** visualiza somente suas próprias atividades
- **E** não acessa participantes de atividades de outros palestrantes

### CA-13.2 - Campos visíveis - bloqueado

A lista de dados pessoais permitidos e o período de acesso dependem de Q-08.

## HU-14 - Gerenciar participantes do evento

### CA-14.1 - Restrição aos próprios eventos

- **Dado** que o organizador está associado a um evento
- **Quando** consulta seus participantes
- **Então** visualiza somente inscrições dos eventos sob sua responsabilidade

### CA-14.2 - Operações permitidas - bloqueado

As operações que o organizador poderá realizar e os dados que poderá alterar dependem de Q-14.

## Definição de pronto

Uma história só pode ser considerada pronta quando:

1. suas questões abertas bloqueantes foram respondidas;
2. todos os critérios deixaram de estar marcados como bloqueados ou parciais;
3. requisitos e regras referenciados estão aprovados;
4. critérios não funcionais aplicáveis possuem métricas validadas;
5. a matriz de rastreabilidade foi atualizada.
