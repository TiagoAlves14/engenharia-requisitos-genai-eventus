# Engenharia de Requisitos com GenAI - Eventus

Este repositório apresenta a análise e a especificação de requisitos do **Sistema de Gestão de Eventos da Eventus**, produzidas a partir do documento de elicitação fornecido na atividade prática da Unidade III do curso *Engenharia de Requisitos com Inteligência Artificial Generativa*.

O trabalho utiliza a IA como apoio à análise, ao refinamento e à elaboração inicial dos artefatos. Nenhuma sugestão da IA foi tratada automaticamente como decisão do negócio.

## Referências estruturais

Foram consultados, como exemplos de organização, os repositórios públicos [aersouza/engenharia-requisitos-genai](https://github.com/aersouza/engenharia-requisitos-genai), [karinakaori/engenharia-requisitos-genai](https://github.com/karinakaori/engenharia-requisitos-genai) e [calielrfelipin/akcit-eng-requisitos](https://github.com/calielrfelipin/akcit-eng-requisitos). A estrutura final foi adaptada ao enunciado e todo o conteúdo foi analisado novamente a partir da elicitação da Eventus.

## Resultado da análise

A elicitação descreve necessidades de participantes, organizadores, equipe financeira, palestrantes e equipe de TI. A análise identificou:

- 21 requisitos funcionais, diferenciando itens confirmados, derivados e ainda sujeitos à validação;
- 12 propostas de requisitos não funcionais, pois o documento informa que esses requisitos não foram levantados;
- 12 regras de negócio, com indicação das definições ainda pendentes;
- 14 questões abertas, incluindo as nove lacunas registradas no documento original e cinco ambiguidades encontradas durante a análise.

## Estrutura do repositório

```text
.
├── README.md
├── RESPOSTA-FORUM.md
└── docs
    ├── 01-elicitacao
    │   └── documento-de-elicitacao.md
    ├── 02-analise
    │   ├── requisitos-funcionais.md
    │   ├── requisitos-nao-funcionais.md
    │   ├── regras-de-negocio.md
    │   ├── lacunas-e-ambiguidades.md
    │   └── matriz-de-rastreabilidade.md
    ├── 03-especificacao
    │   ├── historias-de-usuario.md
    │   ├── criterios-de-aceitacao.md
    │   ├── casos-de-uso.md
    │   └── prototipos-e-fluxos.md
    └── 04-genai
        ├── selecao-de-artefatos.md
        └── registro-de-uso-da-ia.md
```

## Artefatos de especificação escolhidos

- **Histórias de usuário:** representam as necessidades a partir dos diferentes perfis envolvidos e funcionam como unidades de planejamento.
- **Critérios de aceitação em Dado/Quando/Então:** tornam o comportamento verificável e evidenciam exceções relacionadas a vagas, pagamentos, cancelamentos e conflitos de horário.
- **Casos de uso seletivos:** detalham somente os fluxos de maior complexidade, evitando duplicar histórias simples.
- **Protótipos de baixa fidelidade e fluxos:** apoiam a validação antecipada da navegação e das informações de cada tela.
- **Matriz de rastreabilidade:** conecta a elicitação aos requisitos, regras, histórias, critérios e questões abertas, permitindo verificar a origem de cada item.

A análise completa da decisão está em [seleção dos artefatos](docs/04-genai/selecao-de-artefatos.md).

## Por que esses artefatos são adequados

O projeto envolve vários perfis, regras condicionais e pontos ainda sem definição. As histórias mantêm o foco no valor para cada usuário; os critérios de aceitação tornam as condições objetivas; os casos de uso preservam a sequência dos fluxos complexos; os protótipos facilitam a validação com os stakeholders; e a matriz evita que sugestões plausíveis sejam confundidas com requisitos efetivamente solicitados.

## Ferramenta de GenAI utilizada

Foi utilizado o **ChatGPT, da OpenAI**, como apoio nas seguintes atividades:

1. extração e classificação das informações da elicitação;
2. identificação de lacunas, ambiguidades e tensões entre declarações;
3. sugestão e avaliação de artefatos de especificação;
4. elaboração de versões iniciais dos artefatos escolhidos;
5. revisão cruzada de identificadores, origem e coerência.

O processo detalhado está no [registro de uso da IA](docs/04-genai/registro-de-uso-da-ia.md).

## Sugestões aproveitadas

- separar requisitos funcionais, requisitos não funcionais, regras e questões abertas;
- identificar as fontes da elicitação com códigos rastreáveis;
- usar histórias de usuário com critérios em Dado/Quando/Então;
- produzir casos de uso somente para fluxos complexos;
- manter uma matriz de rastreabilidade;
- registrar os requisitos não funcionais como propostas a validar.

## Sugestões modificadas

- Casos de uso para todo o backlog foram reduzidos a três fluxos críticos.
- Métricas não funcionais sugeridas pela IA foram mantidas como propostas, e não como acordos com stakeholders.
- Soluções para lista de espera, reembolso, reserva de vaga, certificado, notificações e conflitos de horário foram convertidas em questões abertas.
- A priorização MoSCoW foi registrada como preliminar, pois não houve uma sessão de priorização com os stakeholders.

## Sugestões descartadas

Foram descartadas funcionalidades sem origem na elicitação, como login social, check-in por QR Code, notificações obrigatórias por WhatsApp, recomendação de eventos e relatórios analíticos avançados. Também foram recusados, nesta etapa, protótipos de alta fidelidade, modelo físico de dados e decisões de arquitetura, por serem prematuros diante das questões abertas.

## Limite da especificação

Os marcadores utilizados nos documentos são:

- **Confirmado:** sustentado diretamente pela elicitação;
- **Derivado:** necessário para viabilizar ou preservar uma necessidade confirmada, com justificativa explícita;
- **A validar:** proposta ou definição que depende de resposta dos stakeholders.

A IA não resolveu nenhuma questão de negócio. Seu papel foi ampliar a cobertura da análise e tornar visível o que ainda precisa ser decidido.

## Postagem do fórum

O texto final, já com o link deste repositório, está em [RESPOSTA-FORUM.md](RESPOSTA-FORUM.md).
