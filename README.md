# 🧠 Miniguia de Estudos: IA Generativa e Engenharia de Prompts

> Projeto desenvolvido para o Desafio de Projeto da [DIO](https://www.dio.me/) — "Construindo um Caderno Temático com NotebookLM e IA como ferramenta de aprendizagem ativa".

---

## 1. Contexto e Objetivos

### Por que esse tema?
Escolhi **IA Generativa e Engenharia de Prompts** porque é um assunto que atravessa praticamente todas as áreas de tecnologia hoje — de desenvolvimento de software a produtividade pessoal — e ainda assim é cheio de termos soltos, dicas fragmentadas e pouca organização conceitual na maioria dos conteúdos que encontramos por aí. Queria sair do "vídeo do YouTube de 10 minutos" e construir uma base de estudo mais sólida, com fontes primárias.

### Objetivos de estudo
Com este caderno temático, busquei responder a quatro perguntas centrais:

1. **O que é, de fato, prompt engineering** — e por que pequenas mudanças de texto geram respostas tão diferentes de um LLM?
2. **Quais são as técnicas fundamentais** (zero-shot, few-shot, chain-of-thought, ReAct etc.) e quando usar cada uma?
3. **Como aplicar boas práticas de prompting no dia a dia** (estudo, trabalho, projetos de programação)?
4. **Quais erros recorrentes ("cicatrizes") aparecem quando se tenta extrair respostas precisas de uma IA**, e como evitá-los?

A ideia não foi só "ler sobre o assunto", mas **usar o próprio NotebookLM como parceiro de estudo ativo**: carregando fontes confiáveis, perguntando, testando variações de prompt e documentando o raciocínio — não só o resultado.

---

## 2. Curadoria de Fontes

Selecionei fontes abertas, gratuitas e de origem reconhecida (big techs, comunidades acadêmicas e de pesquisa), cobrindo desde a base teórica até aplicações práticas. Todas foram carregadas como fonte no NotebookLM.

| # | Fonte | Tipo | Link | Por que escolhi |
|---|-------|------|------|------------------|
| 1 | **Prompt Engineering** (whitepaper oficial do Google, por Lee Boonstra) | PDF (~69 págs.) | https://www.kaggle.com/whitepaper-prompt-engineering | Referência mais completa e estruturada que encontrei: cobre zero-shot, few-shot, system prompting, CoT, ReAct, Self-Consistency, Tree-of-Thought e configuração de parâmetros (temperature, top-k/top-p) |
| 2 | **Prompt Engineering Guide** (DAIR.AI) | Site / texto | https://www.promptingguide.ai/ | Guia colaborativo open-source mantido pela comunidade de pesquisa em NLP, com técnicas avançadas e exemplos práticos atualizados |
| 3 | **Prompt Engineering Overview** (Documentação oficial da Anthropic) | Texto/Docs | https://docs.claude.com/en/docs/build-with-claude/prompt-engineering/overview | Visão de quem constrói os modelos: boas práticas específicas para extrair respostas precisas e estruturadas |
| 4 | **Guia de Engenharia de Prompts** (Documentação oficial da OpenAI) | Texto/Docs | https://platform.openai.com/docs/guides/prompt-engineering | Permite comparar a abordagem de outro grande fornecedor de LLM, mostrando o que é universal e o que é específico de cada modelo |
| 5 | **A Prompt Pattern Catalog to Enhance Prompt Engineering with ChatGPT** (White et al., arXiv) | Artigo acadêmico (PDF) | https://arxiv.org/abs/2302.11382 | Visão acadêmica formal, trazendo uma "catalogação" de padrões de prompt reutilizáveis, o que ajudou a validar o miniguia final |

> 💡 Dica de quem está reproduzindo este projeto: no NotebookLM, vá em **"Adicionar fonte" → "Link da Web"** para Kaggle/promptingguide/docs, e **"PDF"** para o artigo do arXiv (baixe o PDF antes de subir).

---

## 3. Engenharia de Prompts e "Cicatrizes" (Troubleshooting)

Aqui documento o processo real de tentativa e erro ao interrogar o NotebookLM sobre as fontes acima. A ideia é mostrar o raciocínio, não só o resultado final.

### 🔹 Prompt 1 — Pergunta ampla demais (e por que falhou)
**Prompt testado:**
> "Me explica engenharia de prompts."

**Resultado:** resposta genérica, misturando conceitos de fontes diferentes sem hierarquia clara, com citações soltas. Útil como "primeiro contato", mas inútil para estudo aprofundado.

**Cicatriz identificada:** perguntas abertas demais fazem o NotebookLM resumir tudo no nível mais superficial, perdendo a riqueza específica de cada fonte.

**Ajuste aplicado:** quebrar em perguntas menores e direcionadas a uma fonte por vez.

---

### 🔹 Prompt 2 — Comparação direcionada (funcionou bem)
**Prompt testado:**
> "Compare como o whitepaper do Google e a documentação da Anthropic definem 'system prompting'. Aponte semelhanças e diferenças de abordagem."

**Resultado:** resposta estruturada em tópicos, com citações de ambas as fontes, destacando que o Google trata como configuração de contexto global e a Anthropic enfatiza o papel/persona do assistente.

**Por que funcionou:** pedir uma **comparação explícita entre fontes nomeadas** força o modelo a cruzar referências em vez de generalizar.

---

### 🔹 Prompt 3 — Pedido de exemplos práticos (precisou de 2 tentativas)
**Tentativa 1:**
> "Me dá exemplos de chain-of-thought prompting."

Resultado: exemplos genéricos, sem ligação clara com nenhuma fonte específica (pareciam "inventados" a partir de conhecimento geral, não das fontes carregadas).

**Cicatriz identificada:** sem pedir explicitamente "com base nas fontes", o modelo às vezes mistura conhecimento próprio com o conteúdo carregado — o que é arriscado para fins de estudo (pode introduzir imprecisão).

**Tentativa 2 (ajustada):**
> "Com base apenas nas fontes carregadas, extraia 2 exemplos de chain-of-thought prompting citados no whitepaper do Google, indicando a página/seção de origem."

Resultado: resposta mais confiável, com citação direta da seção do PDF.

**Lição:** sempre que a precisão importa, **explicitar "com base nas fontes carregadas"** evita alucinação e mistura de conhecimento externo.

---

### 🔹 Prompt 4 — Pergunta de aplicação prática
**Prompt testado:**
> "Quais boas práticas de prompting (segundo as fontes) eu deveria aplicar ao pedir a uma IA para revisar código?"

**Resultado:** boa síntese cruzando recomendações da OpenAI e da Anthropic — especificidade do pedido, fornecer contexto/exemplos (few-shot), e separar instrução de dados de entrada.

**Aprendizado:** perguntas com **caso de uso concreto** (não "o que é X", mas "como aplico X em Y situação") geram respostas com utilidade prática imediata, ótimas para o miniguia final.

---

### 🔹 Resumo das dificuldades encontradas
- Perguntas muito amplas → respostas rasas e sem citação de fonte.
- Falta de pedir "com base nas fontes" → risco de mistura com conhecimento geral do modelo.
- Pedir comparações entre fontes nomeadas → melhora muito a qualidade e a "transparência" da resposta.
- Pedir aplicação prática (caso de uso) gera conteúdo mais reutilizável do que pedir definição pura.

---

## 4. Miniguia de Estudo (Entrega Final)

### 📌 4.1 Resumos Estruturados

**O que é Prompt Engineering?**
É o processo iterativo de projetar e refinar as instruções (prompts) dadas a um modelo de linguagem para obter respostas mais precisas, relevantes e úteis. Não é "magia de palavras-chave": envolve entender como o modelo interpreta contexto, exemplos e estrutura do texto de entrada.

**Principais técnicas:**

- **Zero-shot prompting:** pedir uma tarefa sem fornecer exemplos. Rápido, mas menos preciso para tarefas complexas ou com formato específico.
- **One-shot / Few-shot prompting:** fornecer 1 ou mais exemplos do padrão esperado de entrada/saída antes da tarefa real. Melhora consistência de formato e estilo.
- **System prompting:** definir um contexto/papel global antes da conversa (ex.: "Você é um revisor técnico de código Python"). Ajuda a manter coerência ao longo da interação.
- **Chain-of-Thought (CoT):** instruir o modelo a "pensar passo a passo" antes de dar a resposta final. Melhora desempenho em tarefas de raciocínio lógico e matemático.
- **ReAct (Reason + Act):** combina raciocínio intermediário com ações (como chamadas de ferramentas) — usado em agentes que precisam buscar informação externa antes de responder.
- **Self-Consistency:** gerar múltiplas cadeias de raciocínio para a mesma pergunta e escolher a resposta mais consistente entre elas.
- **Tree-of-Thought:** explora múltiplos caminhos de raciocínio em paralelo, como uma árvore de decisão, útil para problemas com várias soluções possíveis.

**Parâmetros que afetam o resultado (além do texto do prompt):**
- *Temperature:* controla aleatoriedade — valores baixos geram respostas mais previsíveis, valores altos geram mais criatividade/variação.
- *Top-k / Top-p:* controlam o conjunto de palavras candidatas consideradas a cada passo de geração, afetando diversidade da resposta.

**Boas práticas transversais (Google, OpenAI e Anthropic convergem nesses pontos):**
1. Seja específico sobre o formato de saída desejado.
2. Separe claramente instrução, contexto e dados de entrada.
3. Use exemplos (few-shot) quando o formato importa.
4. Para tarefas de raciocínio, peça explicitamente para "pensar passo a passo".
5. Itere: trate o primeiro prompt como rascunho, não como versão final.

---

### 📌 4.2 Glossário

| Termo | Definição |
|---|---|
| **Prompt** | Texto (ou outra modalidade) de entrada usado para instruir um modelo de linguagem sobre a tarefa desejada |
| **Prompt Engineering** | Prática iterativa de criar e refinar prompts para melhorar a qualidade das respostas de um LLM |
| **Zero-shot prompting** | Pedir uma tarefa ao modelo sem fornecer exemplos prévios |
| **Few-shot prompting** | Fornecer um ou mais exemplos do padrão esperado antes de pedir a tarefa real |
| **System prompt** | Instrução de contexto global que define papel, tom ou regras gerais para toda a conversa |
| **Chain-of-Thought (CoT)** | Técnica que induz o modelo a expor o raciocínio passo a passo antes da resposta final |
| **ReAct** | Padrão que combina raciocínio textual com ações (ex.: chamadas a ferramentas/APIs) de forma intercalada |
| **Self-Consistency** | Geração de múltiplas respostas/raciocínios para a mesma pergunta, escolhendo a mais consistente entre elas |
| **Tree-of-Thought** | Exploração de múltiplos caminhos de raciocínio em estrutura de árvore, avaliando ramos antes de concluir |
| **Temperature** | Parâmetro que controla o grau de aleatoriedade/criatividade nas respostas geradas |
| **Top-k / Top-p** | Parâmetros que limitam o conjunto de palavras candidatas consideradas em cada etapa da geração de texto |
| **Alucinação** | Quando o modelo gera informação incorreta ou inventada, não baseada nas fontes fornecidas |
| **NotebookLM** | Ferramenta do Google que permite carregar fontes próprias e fazer perguntas com respostas ancoradas (citadas) nesses documentos |

---

### 📌 4.3 Prompts Reutilizáveis (para futuras revisões)

Use estes prompts como ponto de partida sempre que quiser revisar o tema no NotebookLM (ou em qualquer chat de IA com fontes carregadas):

```
1. "Com base apenas nas fontes carregadas, resuma em até 5 bullets o conceito de [TÉCNICA], citando a fonte de origem."

2. "Compare como [FONTE A] e [FONTE B] tratam [CONCEITO]. Liste semelhanças e diferenças em uma tabela."

3. "Crie 3 exemplos práticos de [TÉCNICA] aplicados a [CONTEXTO/TAREFA ESPECÍFICA], baseando-se nas fontes carregadas."

4. "Monte um quiz de 5 perguntas de múltipla escolha sobre [TEMA], usando apenas informações presentes nas fontes."

5. "Quais boas práticas de prompting, segundo as fontes, eu deveria aplicar ao [CASO DE USO REAL]? Liste em ordem de prioridade."

6. "Identifique possíveis 'pegadinhas' ou erros comuns sobre [CONCEITO] que as fontes alertam, e explique como evitá-los."
```

> 🎯 Dica: sempre que a precisão for crítica, inclua a frase **"com base apenas nas fontes carregadas"** — isso reduz drasticamente o risco de respostas misturadas com conhecimento genérico do modelo (ver seção de troubleshooting acima).

---

## 5. Ferramentas e Metodologia

- **Ferramenta principal:** [NotebookLM](https://notebooklm.google.com/)
- **Processo:** upload das 5 fontes → formulação de perguntas exploratórias → refinamento iterativo de prompts → consolidação dos achados neste README
- **Projeto desenvolvido para:** Desafio de Projeto — Caderno Temático com IA, [Digital Innovation One (DIO)](https://www.dio.me/)

---

## 📬 Autor

Projeto construído como parte do desafio prático da DIO sobre uso de IA como ferramenta de aprendizagem ativa.
