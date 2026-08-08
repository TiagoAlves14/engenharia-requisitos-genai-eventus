# Resultado da atividade prática - Sistema de Gestão de Eventos Eventus

**Link do repositório no GitHub:**  
https://github.com/TiagoAlves14/engenharia-requisitos-genai-eventus

## Artefatos de especificação escolhidos

Após analisar o documento de elicitação, decidi produzir histórias de usuário, critérios de aceitação no formato Dado/Quando/Então, casos de uso para os fluxos de maior complexidade, protótipos de baixa fidelidade e uma matriz de rastreabilidade. A análise de apoio foi organizada em requisitos funcionais, propostas de requisitos não funcionais, regras de negócio e dúvidas e lacunas.

Os casos de uso foram limitados aos fluxos de inscrição e confirmação de pagamento, cancelamento e possível reembolso e gerenciamento da lista de espera. Assim, eles detalham as situações com mais atores, decisões e exceções sem duplicar todas as histórias de usuário.

## Por que esses artefatos foram considerados adequados

As histórias de usuário representam as necessidades dos diferentes perfis - participantes, organizadores, equipe financeira e palestrantes - de forma simples e orientada ao valor. Os critérios de aceitação tornam essas histórias verificáveis e explicitam condições relacionadas a vagas, pagamento, cancelamento, reembolso, certificado e conflitos de horário.

Os casos de uso preservam a sequência e os fluxos alternativos das operações mais complexas. Os protótipos de baixa fidelidade apoiam a validação antecipada das telas e da navegação. A matriz de rastreabilidade relaciona cada necessidade da elicitação aos requisitos e artefatos correspondentes, ajudando a identificar omissões e a evitar a inclusão de funcionalidades sem origem no documento.

## Como a Inteligência Artificial Generativa apoiou a atividade

A ferramenta utilizada foi o **ChatGPT, da OpenAI**. A IA apoiou a extração e classificação das informações, a identificação de requisitos, regras, lacunas e ambiguidades, a sugestão dos artefatos mais adequados e a elaboração de versões iniciais das histórias, critérios, casos de uso e protótipos.

Também foi utilizada para sugerir perguntas de esclarecimento e revisar a coerência entre os documentos. Cada saída foi conferida com a elicitação original. A IA foi utilizada como apoio à análise e não como substituta da validação com os stakeholders.

## Sugestões da IA aproveitadas

Foram aproveitadas a separação entre requisitos funcionais, requisitos não funcionais, regras de negócio e questões abertas; a utilização de identificadores rastreáveis; as histórias de usuário acompanhadas de critérios em Dado/Quando/Então; a produção seletiva de casos de uso; os protótipos de baixa fidelidade; e a matriz de rastreabilidade.

## Sugestões modificadas ou descartadas

A sugestão de produzir casos de uso para todas as funcionalidades foi modificada: somente os três fluxos mais complexos foram detalhados. Como segurança, desempenho, disponibilidade, acessibilidade e privacidade não foram levantados na elicitação, os requisitos não funcionais sugeridos foram registrados como **propostos - a validar**, sem serem apresentados como decisões já aprovadas.

As soluções sugeridas para prazo de cancelamento, reembolso, lista de espera, reserva de vaga durante o pagamento, conflitos de horário, emissão de certificados, canais de notificação e dados acessíveis aos palestrantes também não foram transformadas em regras definitivas. Permaneceram como questões a esclarecer com os stakeholders.

Foram descartadas funcionalidades sem origem no documento, como login social, check-in por QR Code, notificações obrigatórias por WhatsApp, recomendação personalizada de eventos e relatórios avançados. Protótipos de alta fidelidade, modelo físico de banco de dados e decisões de arquitetura também foram deixados para etapas posteriores.

Um exemplo de ambiguidade preservada foi o comprovante solicitado logo após a inscrição: em eventos pagos, ainda é necessário definir se ele representa apenas o recebimento da solicitação ou a confirmação definitiva após o pagamento. Dessa forma, a especificação distingue claramente o que foi solicitado, o que foi derivado e o que ainda precisa de validação.
