# Seleção dos Artefatos de Especificação

## Contexto da decisão

A IA foi consultada para sugerir artefatos adequados a um sistema de eventos com quatro perfis operacionais, regras condicionais de vaga e pagamento e nove pontos explicitamente não definidos. A recomendação inicial foi avaliada antes da produção dos documentos.

## Critérios de escolha

Um artefato foi mantido quando atendia a pelo menos dois critérios:

1. responde a uma pergunta que os demais artefatos não respondem;
2. possui um leitor ou uma decisão claramente beneficiada;
3. pode ser atualizado sem transformar cada resposta dos stakeholders em retrabalho extenso;
4. é compatível com o nível atual de conhecimento, que ainda possui 14 questões abertas.

## Avaliação das sugestões

| Artefato sugerido | Decisão | Prioridade | Justificativa |
|---|:---:|:---:|---|
| Histórias de usuário | Aceito | Alta | As necessidades foram fornecidas por perfis distintos e se traduzem naturalmente em ator, objetivo e benefício. |
| Critérios de aceitação | Aceito | Alta | Tornam histórias verificáveis e expõem exceções de capacidade, pagamento, cancelamento e conflito. |
| Casos de uso detalhados | Aceito parcialmente | Média | Agregam valor nos fluxos com várias decisões; produzir um para cada história duplicaria informação. |
| Protótipos de baixa fidelidade | Aceito | Média | Permitem validar conteúdo, ações e navegação sem antecipar identidade visual. |
| Matriz de rastreabilidade | Aceito | Alta | Responde quem solicitou cada requisito e revela itens sem origem ou necessidades sem cobertura. |
| Backlog e plano de sprints | Não selecionado | Baixa | A atividade não fornece capacidade da equipe nem prioridade validada. MoSCoW foi mantido apenas como proposta nas histórias. |
| Diagrama geral de casos de uso UML | Não selecionado | Baixa | A matriz e os casos textuais comunicam atores, escopo e exceções com mais precisão neste estágio. |
| BPMN | Não selecionado | Baixa | Não existe descrição suficiente dos processos internos e integrações para justificar uma modelagem formal. |
| Protótipo de alta fidelidade | Não selecionado | Baixa | Seria retrabalho antes de resolver políticas de inscrição, lista de espera e cancelamento. |
| Modelo de domínio e diagrama de classes | Adiado | Baixa | Entidades e estados ainda mudam conforme Q-03, Q-06, Q-10 e Q-12. Pertencem à etapa de projeto após validação. |
| Modelo físico de dados | Não selecionado | Baixa | É decisão de projeto, não artefato necessário para responder o exercício de requisitos. |
| Documento monolítico de especificação | Não selecionado | Baixa | Arquivos modulares facilitam revisão, rastreabilidade e atualização das questões abertas. |

## Conjunto final

### Histórias de usuário

Leitores principais: stakeholders, Product Owner e equipe de desenvolvimento.  
Pergunta respondida: **quem precisa de qual capacidade e para obter qual valor?**

### Critérios de aceitação

Leitores principais: stakeholders, desenvolvimento e testes.  
Pergunta respondida: **como verificar objetivamente que a necessidade foi atendida?**

### Casos de uso seletivos

Leitores principais: análise, desenvolvimento e testes.  
Pergunta respondida: **qual é a sequência dos fluxos com múltiplas decisões e exceções?**

Foram escolhidos:

1. solicitar inscrição;
2. cancelar inscrição e tratar efeitos;
3. oferecer vaga à lista de espera.

### Protótipos de baixa fidelidade e fluxos

Leitores principais: participantes, organizadores, financeiro e palestrantes.  
Pergunta respondida: **quais informações e ações cada perfil precisa visualizar?**

### Matriz de rastreabilidade

Leitores principais: análise, produto, testes e auditoria da atividade.  
Pergunta respondida: **onde cada necessidade foi tratada e qual é a origem de cada requisito?**

## Conclusão

O conjunto escolhido cobre valor, comportamento verificável, sequência, interface e procedência sem exigir decisões técnicas prematuras. A seleção foi intencionalmente menor que a recomendação inicial da IA, pois a qualidade da especificação depende mais de coerência e validação do que da quantidade de documentos.
