# Engenharia de Prompts e Cicatrizes do Projeto

## 1. Objetivo

O objetivo desta documentação é registrar como os prompts foram utilizados e refinados durante a construção do miniguia de RCM.

O processo não foi linear. As primeiras respostas serviram como ponto de partida, mas foram revisadas conforme surgiram dúvidas relacionadas à rastreabilidade das informações, terminologia e aplicação dos conceitos ao estudo de caso.

---

# 2. Primeiro ciclo — exploração do tema

O primeiro objetivo foi utilizar o NotebookLM para compreender os fundamentos da Manutenção Centrada em Confiabilidade a partir das fontes selecionadas.

### Exemplo de prompt

> Com base exclusivamente nas fontes disponíveis, explique o conceito de Manutenção Centrada em Confiabilidade (RCM), seus principais objetivos e como a metodologia pode ser utilizada para definir estratégias de manutenção.

### Objetivo

Construir uma visão geral do tema antes de partir para o estudo de caso.

---

# 3. Segundo ciclo — estruturação da metodologia

Depois da compreensão inicial, o foco passou para a estrutura lógica utilizada pelo RCM.

### Prompt

> Com base nas fontes disponíveis, apresente uma sequência estruturada para realizar uma análise de RCM. Explique cada etapa e indique quais fontes sustentam cada conceito apresentado.

### Aprendizado

Foi possível perceber que diferentes fontes apresentam estruturas semelhantes, mas não necessariamente utilizam exatamente a mesma quantidade de etapas ou perguntas.

Isso levou à necessidade de evitar uma falsa equivalência entre diferentes formulações da metodologia.

---

# 4. Terceiro ciclo — aplicação ao exaustor

Após compreender a metodologia, o conceito foi aplicado a um equipamento didático.

### Prompt

> Aplique a lógica de RCM a um exaustor industrial. Considere o contexto operacional, suas funções, padrões de desempenho, falhas funcionais, modos de falha, causas, efeitos, consequências e possíveis estratégias de manutenção.

### Objetivo

Transformar conceitos abstratos em uma aplicação prática.

---

# 5. Quarto ciclo — controle dos exemplos hipotéticos

Durante a elaboração do estudo de caso, foram utilizados valores numéricos para caracterizar o exaustor.

O problema identificado foi que um leitor poderia interpretar esses valores como dados retirados das referências.

### Refinamento

> Identifique quais valores e informações apresentados na análise do exaustor são encontrados diretamente nas fontes e quais foram criados apenas como hipóteses didáticas. Não apresente valores hipotéticos como recomendações técnicas.

### Resultado

Os valores utilizados no estudo de caso passaram a ser explicitamente identificados como **hipotéticos**.

---

# 6. Quinto ciclo — revisão das recomendações de manutenção

Um dos pontos que exigiu maior cuidado foi a definição de periodicidade para monitoramento.

Uma recomendação genérica de monitoramento mensal poderia ser interpretada como uma regra técnica.

### Prompt de revisão

> Revise as recomendações de monitoramento apresentadas. Verifique se existe suporte nas fontes para os intervalos sugeridos. Caso não exista, não estabeleça uma frequência fixa e explique quais fatores deveriam ser considerados para definir o intervalo.

### Resultado

O miniguia deixou de apresentar uma frequência universal para análise de vibração.

A periodicidade passou a ser tratada como uma decisão dependente do contexto, criticidade, histórico, comportamento do equipamento e qualidade dos dados.

---

# 7. Sexto ciclo — modo de falha x causa

Outro ponto identificado durante a revisão foi a necessidade de separar adequadamente os conceitos de:

* modo de falha;
* causa;
* efeito;
* consequência.

### Prompt

> Revise a análise de falhas e identifique possíveis confusões entre modo de falha e causa. Para cada exemplo, apresente separadamente o modo de falha, sua causa, o efeito observado e a consequência para a operação.

### Resultado

A estrutura da análise passou a seguir:

**Falha funcional → Modo de falha → Causa → Efeito → Consequência**

Essa alteração tornou a análise mais consistente com a lógica de RCM.

---

# 8. Sétimo ciclo — auditoria das respostas

Na etapa final, foi utilizado um prompt de auditoria.

### Prompt

> Faça uma auditoria técnica da resposta anterior utilizando as fontes disponíveis. Para cada afirmação técnica relevante, indique a fonte que a sustenta. Identifique também afirmações que sejam exemplos hipotéticos, interpretações ou aplicações didáticas e que não estejam diretamente presentes nas fontes.

### Objetivo

Reduzir o risco de transformar uma inferência da IA em uma informação aparentemente documentada.

---

# 9. Principais "cicatrizes"

## Cicatriz 1 — Não assumir que uma resposta plausível está necessariamente documentada

Uma resposta pode ser tecnicamente coerente e ainda assim não estar explicitamente sustentada pelas fontes selecionadas.

**Correção:** exigir rastreabilidade.

---

## Cicatriz 2 — Não transformar exemplos em recomendações

Valores criados para facilitar a compreensão do estudo de caso não devem ser interpretados como parâmetros universais.

**Correção:** identificar explicitamente os valores hipotéticos.

---

## Cicatriz 3 — Não generalizar intervalos de manutenção

A periodicidade de monitoramento depende do equipamento e do contexto.

**Correção:** evitar recomendações fixas quando as fontes não fornecem suporte para elas.

---

## Cicatriz 4 — Diferenciar conceitos próximos

Termos como modo de falha, causa, efeito e consequência podem ser confundidos.

**Correção:** estabelecer uma estrutura lógica explícita para a análise.

---

## Cicatriz 5 — Considerar diferenças entre fontes

As fontes utilizadas não apresentam necessariamente a metodologia com a mesma estrutura ou terminologia.

**Correção:** apresentar cada formulação dentro do contexto da fonte correspondente, sem forçar equivalência.

---

# 10. Resultado do processo

O processo de refinamento resultou em um conteúdo final estruturado em torno da seguinte lógica:

**Contexto operacional**

↓

**Função**

↓

**Padrão de desempenho**

↓

**Falha funcional**

↓

**Modo de falha**

↓

**Causa**

↓

**Efeito**

↓

**Consequência**

↓

**Estratégia de manutenção**

Essa sequência passou a ser a estrutura central do miniguia.
