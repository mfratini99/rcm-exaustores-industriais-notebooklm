# Miniguia Prático de RCM Aplicado à Manutenção de Exaustores Industriais

## 📌 Sobre o projeto

Este projeto foi desenvolvido como parte do desafio da DIO sobre **aprendizagem ativa com Inteligência Artificial e NotebookLM**.

O tema escolhido foi **Manutenção Centrada em Confiabilidade (RCM — Reliability-Centered Maintenance)**, com aplicação didática em um **exaustor industrial**.

A proposta foi utilizar a Inteligência Artificial não apenas para gerar conteúdo, mas como uma ferramenta de apoio ao estudo, realizando **curadoria de fontes, elaboração e refinamento de prompts, análise crítica das respostas e organização do conhecimento**.

O resultado desse processo é um miniguia técnico que apresenta os principais conceitos de RCM e demonstra sua aplicação em um equipamento industrial rotativo.

---

## 🎯 Objetivos

Os principais objetivos do projeto foram:

* compreender os fundamentos da Manutenção Centrada em Confiabilidade;
* entender como o contexto operacional influencia a estratégia de manutenção;
* diferenciar função, falha funcional, modo de falha, causa, efeito e consequência;
* compreender como o RCM auxilia na seleção das estratégias de manutenção;
* relacionar conceitos de RCM com técnicas de monitoramento de equipamentos rotativos;
* aplicar a metodologia a um exemplo didático de exaustor industrial;
* utilizar o NotebookLM como ferramenta de pesquisa e organização do conhecimento;
* desenvolver uma metodologia de validação das respostas produzidas pela IA;
* registrar os problemas encontrados durante o processo e as melhorias realizadas nos prompts.

---

## 🏭 Tema escolhido

### Manutenção Centrada em Confiabilidade aplicada a exaustores industriais

O RCM foi escolhido por sua relação direta com temas de **confiabilidade, manutenção, análise de falhas, disponibilidade e gestão de ativos industriais**.

O exaustor industrial foi utilizado como equipamento didático por ser um sistema rotativo que permite relacionar diferentes conceitos de manutenção, como:

* rolamentos;
* correias;
* eixo;
* rotor;
* pás;
* vibração;
* temperatura;
* desgaste;
* desalinhamento;
* desbalanceamento;
* manutenção baseada em condição.

O objetivo não foi desenvolver um plano de manutenção específico para uma instalação real, mas demonstrar como a lógica do RCM pode ser aplicada de maneira estruturada.

---

# 📚 Curadoria de fontes

Foram selecionadas cinco fontes para formar a base de conhecimento utilizada no NotebookLM.

### [1] U.S. Department of Energy / FEMP

**Operations & Maintenance Best Practices: A Guide to Achieving Operational Efficiency. Release 3.0.**

Fonte utilizada principalmente para fundamentos de manutenção e técnicas de monitoramento aplicáveis a equipamentos industriais.

---

### [2] U.S. Department of Energy / FEMP

**Operations & Maintenance Best Practices: A Guide to Achieving Operational Efficiency — Chapter 5: Types of Maintenance Programs. Release 3.0.**

Utilizada para complementar o estudo das diferentes estratégias e tipos de manutenção.

---

### [3] NASA

**Reliability-Centered Maintenance Guide for Facilities and Collateral Equipment. Final. September 2008.**

Foi uma das principais referências para compreender a estrutura do RCM, incluindo contexto operacional, funções, falhas funcionais, modos de falha, consequências e seleção de tarefas de manutenção.

---

### [4] NASA

**NPR 8831.2F — Facilities Maintenance and Operations Management, Chapter 7: Reliability Centered Maintenance.**

Utilizada para complementar a compreensão do processo formal de RCM e sua aplicação à manutenção de instalações e equipamentos.

---

### [5] PICANÇO, Ailson Renan Santos

**Uma abordagem híbrida entre a manutenção produtiva total e a manutenção centrada em confiabilidade para ambientes industriais.**

Ponta Grossa, PR: Atena, 2023.

A obra foi utilizada como referência complementar para conceitos de manutenção centrada em confiabilidade e sua relação com o ambiente industrial.

DOI: 10.22533/at.ed.388232807

---

# 🤖 Uso do NotebookLM

As cinco fontes foram inseridas no NotebookLM para criar um ambiente de estudo baseado em um conjunto controlado de referências.

A utilização da ferramenta ocorreu em etapas:

1. levantamento dos conceitos fundamentais;
2. solicitação de uma estrutura inicial para o estudo;
3. aplicação dos conceitos ao caso de um exaustor industrial;
4. análise das respostas obtidas;
5. identificação de afirmações que precisavam de maior rastreabilidade;
6. refinamento dos prompts;
7. verificação das fontes utilizadas;
8. separação entre informações presentes nas fontes e exemplos hipotéticos;
9. consolidação do conteúdo final.

Dessa forma, o NotebookLM foi utilizado como **ferramenta de apoio ao raciocínio e à organização do conhecimento**, e não como substituto da análise crítica.

---

# 🧠 Engenharia de Prompts

Durante o desenvolvimento foram realizados diferentes ciclos de perguntas e refinamentos.

O processo começou com perguntas mais amplas sobre RCM e evoluiu para prompts com restrições específicas de:

* rastreabilidade;
* utilização das fontes selecionadas;
* separação entre conceitos e exemplos;
* diferenciação entre modo de falha e causa;
* identificação de efeitos e consequências;
* análise das estratégias de manutenção;
* revisão crítica das respostas.

Um dos principais aprendizados foi perceber que uma resposta tecnicamente plausível não necessariamente significa que determinada afirmação esteja diretamente sustentada pelas fontes selecionadas.

Por isso, os prompts foram progressivamente modificados para exigir maior rastreabilidade.

Os prompts e as principais etapas desse processo estão documentados em:

**`prompts/prompts-e-cicatrizes.md`**

---

# 🔎 Cicatrizes e Troubleshooting

Durante o desenvolvimento foram identificados alguns problemas importantes.

### 1. Diferenças na estrutura do RCM

A formulação clássica do RCM apresenta sete perguntas fundamentais, enquanto os documentos da NASA utilizados no projeto apresentam uma estrutura mais sintetizada.

Foi necessário evitar apresentar essas estruturas como se fossem idênticas.

### 2. Valores numéricos apresentados como exemplo

Durante a construção do estudo de caso foram utilizados valores hipotéticos para caracterizar o exaustor.

Foi necessário deixar explícito que esses valores são **didáticos** e não representam recomendações extraídas das fontes.

### 3. Frequência de monitoramento de vibração

Uma frequência fixa de monitoramento poderia parecer uma recomendação técnica universal.

A revisão das fontes mostrou que a periodicidade deve considerar fatores como criticidade, histórico do equipamento, comportamento da degradação e qualidade dos dados disponíveis.

Por isso, uma periodicidade mensal não foi incorporada como regra ao miniguia.

### 4. Confusão entre modo de falha e causa

Uma primeira abordagem poderia tratar, por exemplo, "falta de lubrificação" e "falha do rolamento" como elementos equivalentes.

O conteúdo foi reorganizado para separar:

**modo de falha → causa → efeito → consequência.**

### 5. Necessidade de rastreabilidade

As respostas foram revisadas para diferenciar:

* informação diretamente apoiada pelas fontes;
* aplicação dos conceitos ao exemplo;
* valores hipotéticos;
* interpretações didáticas.

Esse processo foi importante para evitar que exemplos criados durante o estudo fossem apresentados como dados encontrados na literatura.

---

# 📖 Miniguia de Estudo

O conteúdo consolidado foi organizado no documento:

**`miniguia/miniguia-rcm-exaustores.pdf`**

O miniguia aborda:

1. Conceito de RCM;
2. contexto operacional;
3. funções e padrões de desempenho;
4. falhas funcionais;
5. modos de falha e causas;
6. efeitos e consequências;
7. seleção da estratégia de manutenção;
8. manutenção baseada em condição;
9. manutenção preventiva;
10. run-to-failure;
11. técnicas de monitoramento;
12. estudo de caso de um exaustor industrial;
13. análise de rolamentos;
14. análise de correias;
15. análise de rotor e pás;
16. matriz simplificada de RCM;
17. aplicação da lógica em um equipamento real.

---

# 📖 Glossário

O projeto também contém um glossário com os principais conceitos estudados.

O material está disponível em:

**`prompts/glossario-e-prompts-reutilizaveis.md`**

Entre os conceitos estão:

* RCM;
* função;
* padrão de desempenho;
* falha funcional;
* modo de falha;
* causa;
* efeito;
* consequência;
* manutenção baseada em condição;
* manutenção preventiva;
* run-to-failure;
* criticidade;
* confiabilidade.

---

# 🔄 Prompts reutilizáveis

Além dos prompts utilizados durante o desenvolvimento, foram criados prompts que podem ser reutilizados para estudar outros equipamentos e sistemas.

Eles permitem estruturar uma análise seguindo a lógica:

**Contexto → Função → Padrão de desempenho → Falha funcional → Modo de falha → Causa → Efeito → Consequência → Estratégia de manutenção**

Os prompts estão disponíveis em:

**`prompts/glossario-e-prompts-reutilizaveis.md`**

---

# 💡 Principais aprendizados

O principal aprendizado do projeto foi que utilizar Inteligência Artificial para estudar um tema técnico não significa apenas fazer perguntas e aceitar as respostas.

Foi necessário:

* selecionar fontes confiáveis;
* formular perguntas adequadas;
* comparar respostas;
* verificar a origem das informações;
* identificar extrapolações;
* corrigir ambiguidades;
* distinguir exemplos de informações documentadas;
* reformular prompts;
* consolidar o conhecimento obtido.

O processo mostrou que a qualidade do resultado depende tanto da ferramenta utilizada quanto da capacidade de **questionar, validar e contextualizar as informações produzidas**.

---

# 🛠️ Ferramentas utilizadas

* **NotebookLM** — organização das fontes, pesquisa e análise do conteúdo;
* **GitHub** — documentação e versionamento do projeto;
* **Markdown** — estruturação da documentação;
* **PDF** — apresentação do miniguia final.

---

# 📁 Estrutura do repositório

```text
miniguia-rcm-notebooklm/
│
├── README.md
│
├── fontes/
│   └── referencias.md
│
├── prompts/
│   ├── prompts-e-cicatrizes.md
│   └── glossario-e-prompts-reutilizaveis.md
│
├── miniguia/
│   └── miniguia-rcm-exaustores.pdf
│
└── imagens/
```

---

# 📚 Referências

1. U.S. Department of Energy (DOE); Federal Energy Management Program (FEMP). *Operations & Maintenance Best Practices: A Guide to Achieving Operational Efficiency*. Release 3.0. August 2010.

2. U.S. Department of Energy (DOE); Federal Energy Management Program (FEMP). *Operations & Maintenance Best Practices: A Guide to Achieving Operational Efficiency — Chapter 5: Types of Maintenance Programs*. Release 3.0. August 2010.

3. National Aeronautics and Space Administration (NASA). *Reliability-Centered Maintenance Guide for Facilities and Collateral Equipment*. Final. September 2008.

4. NASA. *NPR 8831.2F — Facilities Maintenance and Operations Management, Chapter 7: Reliability Centered Maintenance*.

5. PICANÇO, Ailson Renan Santos. *Uma abordagem híbrida entre a manutenção produtiva total e a manutenção centrada em confiabilidade para ambientes industriais*. Ponta Grossa, PR: Atena, 2023. ISBN 978-65-258-1638-8. DOI: 10.22533/at.ed.388232807.
