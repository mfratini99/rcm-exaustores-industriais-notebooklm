# Glossário de RCM e Prompts Reutilizáveis

# 1. Glossário

### RCM — Reliability-Centered Maintenance

Metodologia estruturada utilizada para determinar requisitos de manutenção a partir das funções que um ativo deve desempenhar, das formas pelas quais essas funções podem falhar e das consequências dessas falhas.

### Contexto operacional

Conjunto de condições nas quais o ativo desempenha suas funções, incluindo regime de operação, carga, ambiente, desempenho requerido, importância do equipamento e consequências associadas às falhas.

### Função

Aquilo que o ativo deve realizar dentro de determinado contexto operacional.

### Padrão de desempenho

Nível de desempenho que deve ser mantido para que a função seja considerada cumprida.

### Falha funcional

Incapacidade do ativo de cumprir uma função dentro do padrão de desempenho requerido.

### Modo de falha

Forma específica pela qual uma falha funcional ocorre.

### Causa da falha

Condição, evento ou mecanismo que contribui para a ocorrência de um determinado modo de falha.

### Efeito da falha

Aquilo que pode ser observado ou ocorre quando o modo de falha acontece.

### Consequência da falha

Impacto provocado pela falha sobre a operação, segurança, meio ambiente, produção ou outros aspectos relevantes.

### Manutenção baseada em condição

Estratégia de manutenção na qual decisões são tomadas a partir da condição observada do equipamento e de indicadores de degradação.

### Manutenção preventiva

Manutenção realizada antes da falha, normalmente associada a uma estratégia baseada em tempo, utilização ou ciclos, quando tecnicamente justificável.

### Run-to-failure

Estratégia na qual o equipamento permanece em operação até a ocorrência da falha, quando as consequências da falha e as condições operacionais tornam essa decisão aceitável.

### Confiabilidade

Capacidade de um ativo desempenhar uma função requerida sob determinadas condições durante um período definido.

### Disponibilidade

Capacidade de um ativo estar em condição de executar sua função quando necessário.

### Criticidade

Avaliação da importância de um ativo ou função considerando as consequências associadas à sua perda.

### Manutenção proativa

Ações destinadas a eliminar ou reduzir causas de falhas e melhorar o desempenho ou a confiabilidade do ativo.

---

# 2. Prompts reutilizáveis

Os prompts abaixo podem ser utilizados para analisar outros equipamentos industriais.

---

## Prompt 1 — Contexto operacional

> Analise o seguinte equipamento: [EQUIPAMENTO].
>
> Considerando as fontes disponíveis, descreva quais informações precisam ser conhecidas sobre o contexto operacional antes de iniciar uma análise de RCM.
>
> Não invente informações ausentes. Separe claramente dados fornecidos, informações necessárias e hipóteses.

---

## Prompt 2 — Identificação das funções

> Para o equipamento [EQUIPAMENTO], identifique suas funções principais considerando o contexto operacional informado.
>
> Para cada função, indique:
>
> 1. função;
> 2. padrão de desempenho necessário;
> 3. informação utilizada como base.
>
> Não confunda função com o componente físico responsável por executá-la.

---

## Prompt 3 — Falhas funcionais

> Para cada função identificada no equipamento [EQUIPAMENTO], determine as possíveis falhas funcionais.
>
> Diferencie claramente:
>
> * perda total da função;
> * perda parcial da função.
>
> Não crie valores de desempenho sem identificar que são hipóteses.

---

## Prompt 4 — Modos e causas de falha

> Para cada falha funcional identificada, determine os possíveis modos de falha e suas causas.
>
> Mantenha separados:
>
> * falha funcional;
> * modo de falha;
> * causa;
> * efeito;
> * consequência.
>
> Utilize exclusivamente as fontes disponíveis e identifique quando uma aplicação for uma interpretação para o equipamento analisado.

---

## Prompt 5 — Efeitos e consequências

> Para cada modo de falha, descreva:
>
> 1. efeito local no equipamento;
> 2. efeito sobre o desempenho;
> 3. consequência operacional;
> 4. possível impacto sobre segurança, meio ambiente, produção ou custo, quando aplicável.
>
> Não presuma que toda falha possui a mesma consequência. Considere o contexto operacional.

---

## Prompt 6 — Estratégia de manutenção

> Para cada modo de falha identificado, avalie quais estratégias de manutenção podem ser consideradas:
>
> * manutenção baseada em condição;
> * manutenção preventiva baseada em tempo ou ciclo;
> * run-to-failure;
> * ação proativa ou melhoria.
>
> Explique o raciocínio utilizado.
>
> Não estabeleça intervalos, limites ou valores numéricos sem suporte nas fontes.

---

## Prompt 7 — Auditoria técnica

> Audite a análise anterior utilizando exclusivamente as fontes disponíveis.
>
> Classifique cada afirmação relevante como:
>
> **A — diretamente sustentada pela fonte**
>
> **B — aplicação dos conceitos da fonte ao equipamento analisado**
>
> **C — hipótese ou exemplo didático**
>
> **D — afirmação sem suporte suficiente**
>
> Para os itens classificados como D, proponha uma reformulação ou indique que a informação deve ser removida.

---

## Prompt 8 — Revisão contra alucinações

> Revise o conteúdo procurando:
>
> * números inventados;
> * recomendações não sustentadas;
> * intervalos de manutenção apresentados como universais;
> * afirmações que parecem vir das fontes mas são inferências;
> * conceitos técnicos utilizados de maneira incorreta;
> * confusão entre modo de falha e causa;
> * confusão entre efeito e consequência.
>
> Apresente os problemas encontrados e a correção recomendada.

---

## Prompt 9 — Aplicação a outro equipamento

> Utilize a mesma lógica de RCM aplicada anteriormente, mas substitua o equipamento por [EQUIPAMENTO].
>
> Preserve a estrutura:
>
> Contexto operacional → Função → Padrão de desempenho → Falha funcional → Modo de falha → Causa → Efeito → Consequência → Estratégia.
>
> Não transfira automaticamente valores ou recomendações do equipamento anterior.

---

## Prompt 10 — Resumo para revisão

> Resuma o conteúdo estudado sobre RCM em uma estrutura de revisão rápida.
>
> Apresente:
>
> * conceitos fundamentais;
> * sequência da análise;
> * principais diferenças entre os conceitos;
> * erros comuns;
> * exemplos de aplicação;
> * perguntas para testar minha compreensão.
>
> Baseie a resposta nas fontes disponíveis e identifique qualquer exemplo criado especificamente para fins didáticos.
