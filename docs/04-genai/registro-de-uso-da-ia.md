# Registro de Uso da Inteligência Artificial Generativa

## Ferramenta

Foi utilizado o **ChatGPT, da OpenAI**.

O material de entrada principal foi o documento de elicitação apresentado no exercício prático da Unidade III. Repositórios públicos indicados como exemplo foram consultados apenas como referência de organização; toda a análise foi refeita a partir da elicitação da Eventus.

## Como a IA foi utilizada

| Etapa | Apoio solicitado à IA | Revisão humana realizada |
|---|---|---|
| 1. Estruturação da fonte | Identificar stakeholders, declarações e observações e atribuir códigos. | Conferência de cada item com o documento original. |
| 2. Análise | Sugerir requisitos funcionais, não funcionais, regras, lacunas e possíveis tensões. | Remoção de itens sem origem e separação entre confirmado, derivado e a validar. |
| 3. Esclarecimento | Formular perguntas objetivas para os pontos indefinidos. | Verificação de que nenhuma pergunta já possuía resposta na elicitação. |
| 4. Seleção | Recomendar artefatos e justificar sua utilidade. | Avaliação por leitor, finalidade, redundância e custo de manutenção. |
| 5. Elaboração | Produzir versões iniciais de histórias, critérios, casos de uso, fluxos e protótipos. | Revisão de linguagem, origem, exceções e dependências de questões abertas. |
| 6. Consistência | Cruzar IDs e procurar requisitos sem origem, regras órfãs e necessidades não tratadas. | Conferência da matriz, links e cobertura das 14 declarações e nove observações. |

## Sugestões aproveitadas

| Sugestão | Motivo da aceitação |
|---|---|
| Identificar fontes com `S-nn`, `E-nn` e `O-nn`. | Permite rastrear cada requisito até a informação que o sustenta. |
| Separar requisitos funcionais, não funcionais, regras e questões. | Evita misturar capacidade do sistema, política do negócio e qualidade. |
| Usar histórias acompanhadas de critérios Dado/Quando/Então. | Une linguagem compreensível a condições verificáveis. |
| Marcar critérios dependentes de decisão como bloqueados ou parciais. | Impede que lacunas sejam escondidas por redação aparentemente completa. |
| Produzir casos de uso para fluxos complexos. | Preserva sequência, alternativas e atores onde a história isolada é insuficiente. |
| Criar protótipos de baixa fidelidade. | Permite validar conteúdo e navegação com baixo custo de mudança. |
| Criar matriz de rastreabilidade. | Verifica cobertura e combate inflação de escopo. |
| Tratar RNFs como propostas a validar. | Respeita O-09, que informa que esses requisitos não foram levantados. |

## Sugestões modificadas

| Sugestão inicial | Modificação | Justificativa |
|---|---|---|
| Produzir casos de uso para todas as funcionalidades. | Restringir a UC-01, UC-02 e UC-03. | Casos simples duplicariam histórias e critérios sem acrescentar decisão. |
| Apresentar metas de desempenho e disponibilidade como requisitos. | Manter métricas com situação `A validar`. | Nenhum volume ou nível de serviço foi acordado. |
| Resolver lista de espera com ordem cronológica e promoção automática. | Registrar Q-03 sem escolher solução. | A IA não pode definir política comercial no lugar dos organizadores. |
| Reservar vaga ao iniciar pagamento por tempo fixo. | Registrar Q-06. | Momento e duração da reserva afetam receita e capacidade e exigem decisão conjunta. |
| Bloquear automaticamente workshops sobrepostos. | Registrar Q-07. | O documento permite simultaneidade, mas não determina o comportamento para o mesmo participante. |
| Vincular certificado automaticamente à presença. | Condicionar RF-20 e CA-06.1 a Q-04. | A confirmação de presença é uma possibilidade, não uma decisão. |
| Usar MoSCoW como priorização definitiva. | Indicar toda prioridade como preliminar. | Não houve sessão de priorização nem informação de capacidade da equipe. |
| Produzir protótipos visuais detalhados. | Usar tabelas de conteúdo e um fluxo Mermaid. | O objetivo atual é validar requisitos, não identidade visual. |

## Sugestões descartadas

| Sugestão da IA | Motivo do descarte |
|---|---|
| Login por redes sociais | Não foi solicitado e pressupõe solução de autenticação específica. |
| Check-in por QR Code | Não aparece na elicitação; a presença ainda depende de Q-04. |
| Notificações obrigatórias por WhatsApp ou SMS | O canal está explicitamente aberto em O-05. |
| Recomendação personalizada de eventos | Não possui stakeholder, objetivo ou origem no documento. |
| Relatórios analíticos avançados | E-09 pede quantidade de inscritos, não uma plataforma analítica. |
| Gateway de pagamento definido pela especificação | A elicitação não informa meios, fornecedor ou modelo de integração. |
| Aplicativo móvel nativo | Não existe requisito de canal ou plataforma. |
| Protótipo de alta fidelidade | Anteciparia decisões de design sujeitas a mudanças após a validação. |
| Banco de dados físico e arquitetura | Pertencem à etapa de projeto e exigem requisitos não funcionais validados. |

## Principais contribuições da IA

### Identificação da ambiguidade do comprovante

A leitura cruzada de E-02 e E-13 revelou que “comprovante após a inscrição” pode significar recebimento da solicitação ou confirmação definitiva. A especificação criou Q-10 em vez de escolher silenciosamente uma interpretação.

### Identificação da tensão de horários

E-05 permite vários workshops no mesmo dia e E-10 permite simultaneidade, mas não define conflito para o mesmo participante. A IA ajudou a localizar a tensão; a decisão permaneceu em Q-07.

### Cobertura de concorrência

O controle automático de vagas exige que solicitações simultâneas não ultrapassem a capacidade. Essa consequência foi registrada como requisito derivado e critério verificável, sem inventar volume de carga.

## Limitações e julgamento humano

A IA tende a completar lacunas com soluções comuns de mercado. Esse comportamento produz documentação convincente, mas pode atribuir ao cliente decisões que ele nunca tomou. Por isso, toda sugestão foi submetida a três perguntas:

1. existe origem na elicitação?
2. é uma consequência necessária ou apenas uma possibilidade?
3. depende de decisão de stakeholder?

O resultado mantém 14 questões abertas. Isso não é uma falha da documentação: é o registro honesto do conhecimento disponível e do trabalho de elicitação que ainda precisa ser realizado.
