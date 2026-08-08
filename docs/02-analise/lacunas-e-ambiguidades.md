# Lacunas, Ambiguidades e Informações a Esclarecer

As nove primeiras questões foram explicitamente registradas no documento de elicitação. As questões `Q-10` a `Q-14` resultam da análise cruzada das declarações e dos interesses dos stakeholders.

| ID | Origem | Lacuna ou ambiguidade | Pergunta objetiva aos stakeholders | Impacto se permanecer aberta | Consultar | Bloqueia o MVP? |
|---|---|---|---|---|---|:---:|
| Q-01 | O-01 | Não há prazo limite para cancelamento. | Até quanto tempo antes do evento o participante pode cancelar? A regra varia por evento? | Impede concluir fluxo de cancelamento e liberação de vaga. | Organizadores e financeiro | Sim |
| Q-02 | O-02 | Não estão definidas as situações de reembolso. | Quais condições, percentuais, prazos e meios de devolução se aplicam? | Gera risco financeiro e divergência com o participante. | Financeiro e organizadores | Sim |
| Q-03 | O-03 | O funcionamento da lista de espera não foi definido. | A ordem será cronológica? A promoção será automática? Haverá prazo para aceite? | Impede especificar estados, notificações e ocupação da vaga. | Organizadores | Sim, se a lista entrar no MVP |
| Q-04 | O-04 | A elegibilidade para certificado está indefinida. | O certificado depende de presença? Quem registra a presença e qual frequência mínima é exigida? | Pode permitir certificado indevido ou impedir emissão legítima. | Organizadores | Não para inscrição; sim para certificados |
| Q-05 | O-05 | Os canais de comprovantes e notificações não foram definidos. | Quais canais serão usados e quais comunicações são obrigatórias? | Afeta experiência, custo e rastreabilidade da comunicação. | Produto, organizadores e TI | Não para o fluxo básico |
| Q-06 | O-06 | O momento de reserva da vaga durante o pagamento está indefinido. | A vaga é reservada ao iniciar o pagamento ou apenas após confirmação? Se reservada, por quanto tempo? | Pode causar sobreocupação ou retenção indevida de vagas. | Financeiro, organizadores e TI | Sim |
| Q-07 | O-07, E-05, E-10 | É permitido haver workshops simultâneos, mas não se sabe como tratar a inscrição do mesmo participante em horários sobrepostos. | O sistema deve bloquear, alertar ou permitir o conflito? Como comparar intervalos parcialmente sobrepostos? | Pode gerar agenda inviável para o participante. | Organizadores e participantes | Sim para múltiplos workshops |
| Q-08 | O-08 | Os campos visíveis aos palestrantes não foram definidos. | Quais dados são estritamente necessários ao palestrante e por quanto tempo ficarão disponíveis? | Pode expor dados pessoais sem necessidade. | Organizadores, TI e responsável por privacidade | Sim para acesso do palestrante |
| Q-09 | O-09 | Não há metas de segurança, desempenho, disponibilidade, acessibilidade ou privacidade. | Quais volumes, janelas críticas, níveis de serviço e obrigações devem ser atendidos? | Impede validar qualidade e dimensionar a solução. | TI e responsáveis pelo negócio | Sim |
| Q-10 | E-02, E-13 | “Comprovante após inscrição” pode significar solicitação recebida ou inscrição confirmada. | Em evento pago, haverá comprovante de solicitação e confirmação separados? Qual deles ocupa a vaga? | Pode comunicar confirmação antes do pagamento. | Financeiro e organizadores | Sim |
| Q-11 | E-09 | “Tempo real” não possui medida objetiva. | Qual atraso máximo entre uma inscrição e a atualização do painel é aceitável? | Torna o requisito impossível de testar. | Organizadores e TI | Não, mas bloqueia a aceitação do painel |
| Q-12 | E-11, E-13 | Não está claro quais inscrições exigem confirmação financeira. | Todo evento pago exige confirmação? Existem gratuidades, cortesias ou confirmação automática? | Afeta estados, regras de vaga e integração financeira. | Financeiro e organizadores | Sim |
| Q-13 | E-03, E-07 | Não foi definido o destino da vaga após cancelamento. | A vaga volta diretamente ao público ou deve ser oferecida ao primeiro da lista de espera? | Pode quebrar a ordem definida para a lista de espera. | Organizadores | Sim, se houver lista de espera |
| Q-14 | S-02 | “Gerenciar participantes” não define quais operações o organizador pode realizar. | O organizador pode apenas consultar ou também confirmar, cancelar, transferir e corrigir dados de inscrições? | Pode conceder poderes excessivos ou deixar a operação sem funções necessárias. | Organizadores e responsável por privacidade | Sim para RF-18 |

## Tensões entre declarações

### Comprovante imediato versus confirmação financeira

`E-02` pede comprovante logo após a inscrição, enquanto `E-13` exige confirmação do pagamento antes de liberar determinadas inscrições. A especificação não escolhe uma interpretação; Q-10 e Q-12 devem ser respondidas.

### Múltiplos workshops versus simultaneidade

`E-05` permite vários workshops no mesmo dia e `E-10` permite workshops simultâneos. Nenhuma das declarações informa se o mesmo participante pode ocupar atividades sobrepostas. A decisão permanece em Q-07.

### Autonomia de cancelamento versus política do evento

`E-03` pede cancelamento sem contato manual e `E-08` informa que nem todo evento permite cancelar. O sistema deve permitir a solicitação apenas quando a política autorizar e explicar a restrição, mas prazo e consequências permanecem em Q-01 e Q-02.

## Tratamento adotado

Nenhuma questão foi respondida pela IA. Quando um artefato depende de uma dessas decisões, ele referencia o identificador `Q-nn` e sinaliza que o cenário está bloqueado ou provisório.
