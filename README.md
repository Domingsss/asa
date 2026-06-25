#Caderno Temático: Python para Análise de Dados
Um repositório de aprendizagem ativa com curadoria de fontes, engenharia de prompts e miniguia de estudos.

PythonPandasNumPyLicenseDIO

Projeto prático desenvolvido para o Desafio de Projeto da Digital Innovation One (DIO), no qual a Inteligência Artificial é utilizada como ferramenta de aprendizagem ativa, aliada a pensamento crítico, curadoria de fontes e organização do conhecimento.

#Sumário
Contexto e Objetivos
Curadoria de Fontes
Mapa Mental do Tema
Engenharia de Prompts e "Cicatrizes"
Miniguia de Estudo (Entrega Final)
Referências
Como Usar Este Repositório
1. Contexto e Objetivos
1.1 Tema escolhido
O presente Caderno Temático tem como foco a aprendizagem de Python para Análise de Dados, com ênfase nas bibliotecas fundamentais do ecossistema PyData: NumPy e Pandas, além de uma introdução à visualização de dados com Matplotlib e Seaborn. A escolha do tema justifica-se pela centralidade da linguagem Python no mercado de trabalho contemporâneo de Ciência de Dados, sendo requisito mínimo para atuação em posições júnior de análise de dados, business intelligence e engenharia de dados. Adicionalmente, o tema oferece um percurso de aprendizagem progressivo e bem documentado, adequado a estudantes iniciantes que precisam construir fundamentos sólidos antes de avançar para tópicos mais avançados como machine learning e estatística aplicada.

#1.2 Justificativa
Python mantém-se como a linguagem mais utilizada por profissionais de dados no Brasil, com adoção superior a 80% entre os praticantes da área, conforme levantamentos setoriais disponíveis em fontes abertas. Para um estudante iniciante, dominar os fundamentos de manipulação tabular de dados (Pandas) e computação numérica vetorial (NumPy) constitui pré-requisito inegociável para qualquer avanço posterior em temas como aprendizado de máquina, estatística aplicada, visualização avançada ou engenharia analítica. Ignorar essa base costuma resultar em frustração posterior, quando o estudante se depara com APIs mais complexas sem compreender os objetos subjacentes.

A presente iniciativa adota a aprendizagem ativa como paradigma metodológico, em detrimento do consumo passivo de conteúdos. Em vez de apenas assistir a videoaulas ou ler tutoriais, o estudante formula perguntas estratégicas, testa variações de prompts em IA generativa, valida respostas contra fontes primárias e registra o raciocínio envolvido em cada iteração. Esse fluxo aproxima-se das boas práticas de curadoria de conhecimento valorizadas pelo mercado de tecnologia, particularmente em funções que exigem combinação de pensamento crítico, domínio técnico e capacidade de documentação.

#1.3 Objetivos
Objetivo geral

Desenvolver compreensão sólida e aplicável dos fundamentos de Python para análise de dados, com foco em Pandas e NumPy, por meio de aprendizagem ativa mediada por IA generativa (Google NotebookLM).

Objetivos específicos

Identificar e selecionar fontes abertas e confiáveis sobre Python para dados, organizando-as no NotebookLM como base de conhecimento citável;
Formular perguntas estratégicas e variações de prompts para extrair respostas de qualidade da IA, documentando o processo iterativo e as dificuldades encontradas;
Produzir um miniguia de estudos consolidado, contendo resumos estruturados, glossário temático e conjunto de prompts reutilizáveis para revisões futuras;
Construir um repositório público no GitHub que demonstre maturidade técnica, organização do conhecimento e capacidade de documentação profissional.
2. Curadoria de Fontes
2.1 Critérios de seleção
Foram adotados os seguintes critérios para a seleção das fontes carregadas no NotebookLM, com o objetivo de garantir qualidade acadêmica e utilidade prática:

Disponibilidade aberta: material gratuito e acessível sem barreira financeira, respeitando o princípio da democratização do conhecimento;
Autoria reconhecida: preferência por documentação oficial ou obras de referência assinadas por especialistas da comunidade PyData;
Atualidade: conteúdo compatível com versões recentes das bibliotecas (NumPy ≥ 1.24, Pandas ≥ 2.0), evitando APIs depreciadas;
Idioma acessível: material em português ou inglês técnico de leitura intermediária;
Profundidade adequada ao nível iniciante: equilíbrio entre fundamentos teóricos e exemplos práticos executáveis.
2.2 Fontes selecionadas
As cinco fontes a seguir foram carregadas no NotebookLM para servir de base de conhecimento citável pela IA durante as interações:

#	Título	Autor / Mantenedor	Tipo	Link
1	Python Data Science Handbook	Jake VanderPlas	Livro aberto (HTML)	https://jakevdp.github.io/PythonDataScienceHandbook/
2	Python for Data Analysis, 3ª ed.	Wes McKinney	Livro aberto (HTML)	https://wesmckinney.com/book/
3	Documentação Oficial do Pandas	PyData Community	Documentação	https://pandas.pydata.org/docs/
4	Documentação Oficial do NumPy	NumPy Community	Documentação	https://numpy.org/doc/stable/
5	The Turing Way: Guide to Reproducible Data Science	The Alan Turing Institute	Comunidade/livro colaborativo	https://the-turing-way.netlify.app/welcome
2.3 Síntese das fontes
Fontes 1 e 2: obras de referência assinadas por autores centrais do ecossistema (VanderPlas e McKinney, criador do Pandas). Funcionam como bússola conceitual e fonte primária de boas práticas, sendo particularmente úteis quando a IA precisa citar uma autoridade reconhecida.
Fontes 3 e 4: documentação oficial, utilizadas como referência canônica para checagem de API, assinaturas de funções e comportamentos de versões específicas.
Fonte 5: guia colaborativo britânico sobre reprodutibilidade em ciência de dados, agregando perspectiva metodológica que vai além do código e aborda questões éticas, organizacionais e de colaboração.
A combinação dessas cinco fontes oferece à IA uma base de conhecimento suficientemente ampla para responder a perguntas conceituais, práticas e metodológicas, ao mesmo tempo em que permite citação rastreável, reduzindo o risco de alucinação.

3. Mapa Mental do Tema
A estrutura visual a seguir representa a organização conceitual do caderno. O diagrama foi elaborado em sintaxe Mermaid, renderizado automaticamente pelo GitHub, e permite uma visão panorâmica dos tópicos cobertos pelo estudo.

mindmap  root((Python para Dados))    Fundamentos da Linguagem      Tipos nativos      Estruturas de dados      Comprehensions      Funções e módulos    NumPy      ndarray      Indexação e slicing      Operações vetoriais      Broadcasting    Pandas      Series      DataFrame      Indexação (.loc / .iloc)      Limpeza de dados      Agrupamento (groupby)      EDA    Visualização      Matplotlib      Seaborn      Tipos de gráfico    Reprodutibilidade      Ambientes virtuais      Notebooks      Versionamento
O mapa mental serve como índice navegável do conteúdo: cada ramo corresponde a uma seção do miniguia apresentado adiante. Recomenda-se ao leitor retornar a este diagrama sempre que precisar situar um tópico específico dentro do conjunto maior do conhecimento coberto.

4. Engenharia de Prompts e "Cicatrizes"
4.1 Metodologia
A seção a seguir documenta três prompts estratégicos elaborados durante o estudo, com o objetivo de extrair da IA respostas úteis, precisas e citáveis. Para cada prompt, registra-se: (1) a versão inicial formulada; (2) as variações testadas e o porquê de cada ajuste; (3) a resposta obtida, resumida; (4) as referências apontadas pela IA ou validadas manualmente; (5) as dificuldades encontradas ("cicatrizes") durante a iteração; (6) a versão final otimizada do prompt.

Essa documentação reflete o raciocínio envolvido na interação com IA generativa, atividade valorizada pelo mercado de tecnologia. O registro explícito das iterações e dos erros permite que outros estudantes replicem o processo, aprendam com as dificuldades já mapeadas e evitem os mesmos tropeços.

4.2 Prompt 1 — Conceitos fundamentais
Versão inicial
"Explique o que é um DataFrame no Pandas."

Resultado: resposta genérica, sem analogias, sem diferenciação clara em relação a uma tabela SQL ou planilha Excel. Não citou fontes.

Variações testadas
Variação A: "Explique DataFrame como se eu fosse iniciante, usando analogia do dia a dia."
Variação B: "Compare Series e DataFrame no Pandas, com exemplos práticos e cite a fonte."
Variação C (final): "Explique a diferença entre Series e DataFrame no Pandas como se eu fosse iniciante. Use uma analogia concreta do cotidiano, forneça um exemplo curto de código e indique a página ou seção do Python for Data Analysis (Wes McKinney) onde o tema é tratado."
Resposta obtida (resumida)
A IA explicou que uma Series é uma estrutura unidimensional, comparável a uma coluna de planilha, enquanto um DataFrame é uma estrutura bidimensional, semelhante a uma planilha inteira com várias colunas indexadas. A analogia utilizada foi a de um cardápio de restaurante: cada item (prato) com seu preço forma uma Series; o cardápio completo, com colunas adicionais como descrição e ingredientes, forma um DataFrame. Forneceu o seguinte exemplo de código:
-------------------------------
import pandas as pd

precos = pd.Series([25.0, 18.5, 32.0], index=["Lasanha", "Risoto", "Salmão"])
cardapio = pd.DataFrame({
    "preco": precos,
    "serve": [2, 1, 1],
})
--------------------------------
A IA citou o capítulo 5 do livro de McKinney (seção "Introduction to Pandas Data Structures").

Referências
McKinney, W. Python for Data Analysis, 3. ed., cap. 5;
Documentação oficial do Pandas, seção "Intro to Data Structures".
Dificuldades encontradas ("cicatrizes")
A primeira versão do prompt produziu resposta que poderia ser encontrada em qualquer blog, sem profundidade analítica;
A exigência de citação forçou a IA a buscar nas fontes carregadas no NotebookLM, evitando alucinação bibliográfica;
Em uma das variações, a IA citou "capítulo 4" incorretamente; foi necessário validar manualmente na fonte primária e reformular o pedido para especificar "seção" em vez de "capítulo", reduzindo ambiguidade;
A IA inicialmente não mencionou que o índice de uma Series e de um DataFrame pode ser de qualquer tipo hashable, não apenas inteiro; esse detalhe só apareceu após pergunta específica.
Versão final otimizada
------------------------------
Explique a diferença entre Series e DataFrame no Pandas como se eu fosse
iniciante. Use uma analogia concreta do cotidiano, forneça um exemplo
curto de código (3-5 linhas) e indique a seção da documentação oficial
ou do livro de Wes McKinney onde o tema é tratado. Inclua uma nota sobre
o tipo do índice.
------------------------------
4.3 Prompt 2 — Aplicação prática (Análise Exploratória de Dados)
Versão inicial
"Faça uma EDA com Pandas."

Resultado: resposta confusa, listou funções soltas (head, describe, info) sem contextualizar fluxo nem objetivo analítico.

Variações testadas
Variação A: "Mostre um fluxo completo de EDA com Pandas para um iniciante."
Variação B: "Liste as 10 funções de Pandas mais usadas em EDA."
Variação C (final): "Apresente um fluxo de trabalho passo a passo de Análise Exploratória de Dados (EDA) usando Pandas, com 6 etapas numeradas. Para cada etapa, forneça: (i) objetivo, (ii) snippet de código comentado e (iii) o que observar no resultado. Considere um dataset tabular genérico carregado de um arquivo CSV e a versão 2.x do Pandas."
Resposta obtida (resumida)
A IA estruturou a resposta nas seis etapas a seguir:

Carregamento e inspeção inicial — pd.read_csv, df.head(), df.shape;
Diagnóstico de tipos e nulos — df.info(), df.isnull().sum();
Estatística descritiva — df.describe(), com atenção a outliers;
Distribuição de variáveis categóricas — df["col"].value_counts();
Correlação entre variáveis numéricas — df.corr(numeric_only=True);
Identificação de outliers e visualização — histograma e boxplot com Matplotlib/Seaborn.
Cada etapa incluiu snippet comentado e indicação do que observar (e.g., "valores nulos acima de 30% sugerem necessidade de imputação ou exclusão de coluna").

Referências
VanderPlas, J. Python Data Science Handbook, cap. 3 (Pandas);
Documentação oficial do Pandas, seção "Cookbook".
Dificuldades encontradas ("cicatrizes")
A primeira versão foi excessivamente aberta, gerando resposta dispersa e sem utilidade prática;
A exigência de "objetivo + código + observação" por etapa reduziu drasticamente a superficialidade;
A IA sugeriu df.corr() sem advertir sobre o parâmetro numeric_only, introduzido no Pandas 2.0; foi necessário perguntar para que mencionasse a quebra de compatibilidade e a recomendação atual;
Em uma das variações, a IA recomendou df.append(), método removido no Pandas 2.0; foi necessário restringir explicitamente a versão da biblioteca no prompt.
Versão final otimizada
text

Apresente um fluxo de trabalho passo a passo de Análise Exploratória
de Dados (EDA) usando Pandas, com 6 etapas numeradas. Para cada etapa,
forneça: (i) objetivo, (ii) snippet de código comentado e (iii) o que
observar no resultado. Considere Pandas 2.x e um dataset tabular
genérico carregado de um CSV. Ao final, cite a seção da documentação
oficial onde cada função é detalhada e alerte sobre APIs depreciadas.
4.4 Prompt 3 — Troubleshooting (debug de erro)
Versão inicial
"Estou recebendo KeyError no Pandas. Como resolver?"

Resultado: resposta genérica sugerindo "verifique se a coluna existe", sem enumerar causas raiz nem estratégias de diagnóstico.

Variações testadas
Variação A: "Liste as 5 causas mais comuns de KeyError no Pandas."
Variação B: "Meu código dá KeyError em df['coluna']. Quais diagnósticos devo fazer?"
Variação C (final): "Estou recebendo o erro KeyError: 'nome_coluna' no Pandas. Liste as 5 causas mais comuns, incluindo casos não óbvios como MultiIndex. Para cada uma, apresente: (i) sintoma típico, (ii) comando de diagnóstico e (iii) correção. Ao final, sugira um checklist de debug em 3 passos."
Resposta obtida (resumida)
A IA listou as cinco causas a seguir:

Nome da coluna com espaços ou maiúsculas — diagnosticar com df.columns.tolist(); correção com df.rename(columns=...);
Index vs. coluna — diagnosticar com df.index, df.reset_index();
Coluna removida em etapa anterior — diagnosticar revisando o pipeline com df.columns após cada transformação;
Acesso por posição em vez de rótulo — usar df.iloc[:, i] quando o índice for numérico;
MultiIndex não tratado — diagnosticar com df.index.nlevels, acessar com df.loc[("a", "b"), :].
Checklist sugerido em 3 passos: (1) imprimir df.columns literalmente, (2) checar type(df) e df.shape, (3) isolar a linha problemática em uma célula separada.

Referências
Documentação oficial do Pandas, seção "Indexing and Selecting Data";
Stack Overflow tags pandas + keyerror.
Dificuldades encontradas ("cicatrizes")
A primeira versão do prompt produziu resposta descartável, que não agregava valor sobre o que o estudante já saberia por intuição;
A exigência de "sintoma + diagnóstico + correção" por causa elevou a utilidade da resposta para nível de referência rápida;
A IA inicialmente não mencionou o caso de MultiIndex, que é comum mas raramente coberto em tutoriais iniciantes; foi necessário perguntar especificamente sobre "casos menos óbvios";
A IA sugeriu como correção o uso de df.xs() para MultiIndex sem explicar a diferença entre xs e loc com tupla, gerando confusão adicional; foi necessário pedir explicitamente a comparação entre as duas abordagens.
Versão final otimizada
---------------------------------------
Estou recebendo o erro `KeyError: 'nome_coluna'` no Pandas. Liste as
5 causas mais comuns, incluindo casos não óbvios como MultiIndex. Para
cada causa, apresente: (i) sintoma típico, (ii) comando de diagnóstico
e (iii) correção. Ao final, sugira um checklist de debug em 3 passos
e compare brevemente as abordagens `loc`, `iloc` e `xs` para MultiIndex.
---------------------------------------
4.5 Lições aprendidas (síntese das "cicatrizes")
Da iteração com os três prompts, extraíram-se as seguintes lições, úteis como heurísticas gerais de engenharia de prompts para qualquer tema técnico:

Exija citação de fonte sempre que possível — isso reduz drasticamente alucinações e força a IA a ancorar a resposta nas fontes carregadas no NotebookLM, em vez de recorrer a conhecimento genérico de pré-treino;
Especifique a estrutura da resposta — pedir "objetivo + código + observação" por item gera respostas muito mais estruturadas do que perguntas abertas;
Restrinja a versão da tecnologia — mencionar "Pandas 2.x" evita que a IA sugira APIs depreciadas, como df.append() ou df.corr() sem numeric_only;
Peça casos não óbvios explicitamente — a IA tende a listar apenas os casos mais comuns; é necessário perguntar para obter edge cases como MultiIndex;
Valide manualmente referências bibliográficas — IAs podem citar capítulos ou páginas inexistentes; sempre conferir na fonte primária antes de incorporar a referência a um material definitivo;
Registre o processo iterativo — o valor pedagógico está nas iterações e nos erros, não apenas no prompt final; documentar essas variações é o que diferencia um caderno "Nota 10" de um repositório superficial.
5. Miniguia de Estudo (Entrega Final)
Esta seção consolida o resultado final do aprendizado, integrando os conhecimentos extraídos das fontes curadas e das interações com a IA. Está dividida em três partes: resumos estruturados do assunto, glossário dos principais conceitos e conjunto de prompts reutilizáveis para revisões futuras.

5.1 Resumos estruturados do assunto
5.1.1 Fundamentos do Python para Dados
Python é uma linguagem multiparadigma de tipagem dinâmica cuja popularidade em ciência de dados deve-se à sintaxe expressiva, ao vasto ecossistema de bibliotecas científicas e à integração nativa com ferramentas de análise. Para fins de análise de dados, são considerados pré-requisitos: domínio dos tipos nativos (int, float, str, bool, None), estruturas de dados (list, tuple, dict, set), compreensões de lista e dicionário, funções de primeira classe, manipulação de arquivos e o uso de ambientes virtuais (venv ou conda) para isolamento de dependências. A ausência de qualquer um desses fundamentos tende a manifestar-se como dificuldade recorrente no uso produtivo das bibliotecas científicas.

A organização idiomática do código Python é orientada pela PEP 8, que define convenções de nomes (snake_case para funções e variáveis, PascalCase para classes, UPPER_CASE para constantes), indentação (4 espaços), comprimento de linha (79 caracteres) e importações (uma por linha, no topo do arquivo). Em projetos de dados, recomenda-se ainda separar o código de análise (em scripts ou notebooks) do código de apoio (módulos reutilizáveis), adotando uma estrutura de diretórios como src/, data/, notebooks/ e tests/. Essa separação facilita a reprodutibilidade e a manutenção do código ao longo do tempo.

5.1.2 NumPy: arrays e computação vetorial
NumPy é a biblioteca fundamental da pilha PyData, fornecendo o objeto ndarray — uma estrutura homogênea e multidimensional que permite operações vetoriais com desempenho muito superior ao das listas nativas do Python. O ganho de desempenho decorre da implementação em C e da contiguidade de memória dos arrays, evitando o overhead de interpretação e boxing de tipos presente nas listas. Para datasets de médio e grande porte, a diferença entre operar com listas Python e com arrays NumPy pode chegar a duas ordens de magnitude.

Conceitos essenciais a serem dominados:

Criação de arrays: np.array([1, 2, 3]), np.zeros((2, 3)), np.arange(0, 10, 2), np.linspace(0, 1, 50), np.random.randn(100);
Atributos: shape, dtype, ndim, size, nbytes;
Indexação e slicing: sintaxe arr[start:stop:step]; indexação fancy com listas (arr[[0, 2, 4]]) e máscaras booleanas (arr[arr > 5]);
Operações vetoriais (universal functions): aritmética elemento a elemento, funções universais como np.sqrt, np.exp, np.log, e reduções como sum, mean, std, max, argmax;
Broadcasting: mecanismo que permite operar arrays de formas compatíveis sem replicação explícita de dados, essencial para escrever código conciso e eficiente. As regras de broadcasting podem ser contraintuitivas no início, mas são determinísticas e vale a pena dominá-las.
5.1.3 Pandas: Series, DataFrames e EDA
Pandas, construído sobre NumPy, é a biblioteca padrão para manipulação de dados tabulares em Python. Os dois objetos centrais são a Series, array unidimensional rotulado com índice explícito, e o DataFrame, estrutura bidimensional com índice de linha e rótulos de coluna, semelhante a uma planilha ou tabela SQL em memória. A separação entre índice e colunas é uma das características que distingue o Pandas de outras bibliotecas como R data.frame ou data.table, e compreender essa distinção é fundamental para uso produtivo da biblioteca.

Operações essenciais a dominar:

Carregamento: pd.read_csv(), pd.read_excel(), pd.read_json(), pd.read_sql();
Inspeção: df.head(), df.tail(), df.info(), df.describe(), df.shape;
Seleção: df["coluna"], df[["a", "b"]], df.loc[rotulo], df.iloc[posicao];
Filtragem: df[df["idade"] > 18], df.query("idade > 18");
Limpeza: df.dropna(), df.fillna(), df.drop_duplicates(), df.astype();
Transformação: df.assign(), df.apply(), df.map(), df.replace();
Agrupamento: df.groupby("col")["outra"].agg(["mean", "count"]);
Junção: pd.merge(), df.join(), pd.concat().
A análise exploratória de dados (EDA) em Pandas segue tipicamente o fluxo: carregar → inspecionar → tratar nulos → descrever estatisticamente → analisar distribuições → investigar correlações → identificar outliers → comunicar achados. Cada etapa consome uma fração não negligenciável do tempo total de análise, e a qualidade do resultado final depende fortemente do cuidado dedicado às etapas iniciais de inspeção e limpeza.

5.1.4 Visualização de dados
A visualização é etapa indispensável da EDA, pois permite identificar padrões visuais que estatísticas descritivas não capturam, como multimodalidade, caudas pesadas, clusters e relações não lineares entre variáveis. As bibliotecas mais utilizadas no ecossistema Python são:

Matplotlib: biblioteca base, flexível porém verbosa; toda visualização mais sofisticada eventualmente recorre a ela;
Seaborn: construída sobre Matplotlib, oferece API de mais alto nível e estética mais agradável, com funções como sns.histplot, sns.boxplot, sns.scatterplot, sns.heatmap e sns.pairplot;
Pandas plotting: interface direta via df.plot(), útil para visualizações rápidas durante a EDA.
Boas práticas: sempre rotular eixos e incluir título descritivo; evitar gráficos de pizza para mais de cinco categorias, pois a percepção humana de ângulos é limitada; preferir boxplots para distribuições com outliers; usar paletas de cores acessíveis (e.g., viridis, cividis), que funcionam para daltônicos e em impressão preto e branco; e dimensionar adequadamente a figura com figsize para evitar compressão visual.

5.2 Glossário
Termo
Definição
Anaconda	Distribuição de Python voltada para ciência de dados, com gerenciador de pacotes conda.
Array	Estrutura de dados multidimensional e homogênea do NumPy (ndarray).
Broadcasting	Mecanismo do NumPy que permite operar arrays de formas diferentes sem cópia explícita.
CSV	Comma-Separated Values; formato de arquivo texto padrão de facto para dados tabulares.
DataFrame	Estrutura bidimensional rotulada do Pandas, análoga a uma planilha.
EDA	Exploratory Data Analysis; análise exploratória de dados.
Indexação booleana	Seleção de elementos de um array com base em uma máscara de True/False.
Jupyter Notebook	Ambiente interativo que combina código, saída e markdown, padrão em análise de dados.
loc / iloc	Acessores do Pandas: loc seleciona por rótulo, iloc seleciona por posição inteira.
NaN	Not a Number; valor sentinela para dado ausente em arrays numéricos (IEEE 754).
NumPy	Biblioteca fundamental para computação numérica vetorial em Python.
Pandas	Biblioteca para manipulação de dados tabulares em Python, construída sobre NumPy.
PEP 8	Python Enhancement Proposal 8; guia de estilo oficial do Python.
Reprodutibilidade	Princípio de que um experimento analítico deve poder ser reexecutado por terceiros com o mesmo resultado.
Series	Estrutura unidimensional rotulada do Pandas.
Shape	Tupla que descreve as dimensões de um array ou DataFrame.
Vectorization	Processo de aplicar operações a arrays inteiros em vez de elementos individuais, aproveitando implementação em C.
venv	Módulo da biblioteca padrão para criação de ambientes virtuais isolados.

5.3 Conjunto de prompts reutilizáveis
Os prompts a seguir foram refinados a partir da seção 4 e podem ser reutilizados em revisões futuras sobre o tema. Estão escritos como templates, com placeholders entre colchetes que devem ser substituídos pelo contexto específico.

Prompt A — Explicação de conceito
Explique o conceito de [CONCEITO] em [BIBLIOTECA] como se eu fosse
iniciante. Use uma analogia concreta do cotidiano, forneça um exemplo
curto de código (3-5 linhas) e indique a seção da documentação oficial
ou livro de referência onde o tema é tratado. Inclua uma nota sobre
armadilhas comuns.

Explique o conceito de [CONCEITO] em [BIBLIOTECA] como se eu fosse
iniciante. Use uma analogia concreta do cotidiano, forneça um exemplo
curto de código (3-5 linhas) e indique a seção da documentação oficial
ou livro de referência onde o tema é tratado. Inclua uma nota sobre
armadilhas comuns.

Prompt B — Fluxo prático

Apresente um fluxo de trabalho passo a passo de [TAREFA] usando
[BIBLIOTECA], com 6 etapas numeradas. Para cada etapa, forneça:
(i) objetivo, (ii) snippet de código comentado e (iii) o que observar
no resultado. Considere a versão [VERSÃO] da biblioteca. Ao final,
cite a seção da documentação oficial onde cada função é detalhada e
alerte sobre APIs depreciadas.

Prompt C — Debug de erro

Estou recebendo o erro `[MENSAGEM DE ERRO]` em [BIBLIOTECA]. Liste
as 5 causas mais comuns, incluindo casos não óbvios. Para cada causa,
apresente: (i) sintoma típico, (ii) comando de diagnóstico e
(iii) correção. Ao final, sugira um checklist de debug em 3 passos.

Prompt D — Comparação de abordagens

Compare [ABORDAGEM A] e [ABORDAGEM B] em [BIBLIOTECA] quanto a:
(i) legibilidade, (ii) desempenho, (iii) idiomatismos da comunidade.
Apresente um exemplo equivalente em cada abordagem e indique quando
preferir uma sobre a outra.

Prompt E — Síntese para revisão

Com base nas fontes carregadas, produza um resumo estruturado de
[TEMA] contendo: (i) definição em uma frase, (ii) três pontos
centrais, (iii) dois exemplos de código comentados, (iv) duas
armadilhas comuns a evitar. Cite as fontes utilizadas.

6. Referências
As referências a seguir seguem adaptação do padrão ABNT NBR 6023:2018, voltada para recursos eletrônicos. As datas de acesso devem ser atualizadas no momento da entrega final do projeto.

McKINNEY, Wes. Python for Data Analysis. 3. ed. Sebastopol: O'Reilly Media, 2022. Disponível em: https://wesmckinney.com/book/. Acesso em: 26 jun. 2026.

NUMPY. NumPy Documentation. Version 2.x. NumPy Community, 2024. Disponível em: https://numpy.org/doc/stable/. Acesso em: 26 jun. 2026.

PANDAS. Pandas Documentation. Version 2.x. PyData Community, 2024. Disponível em: https://pandas.pydata.org/docs/. Acesso em: 26 jun. 2026.

THE ALAN TURING INSTITUTE. The Turing Way: A Handbook for Reproducible, Ethical and Collaborative Research. Londres: The Alan Turing Institute, 2024. Disponível em: https://the-turing-way.netlify.app/welcome. Acesso em: 26 jun. 2026.

VANDERPLAS, Jake. Python Data Science Handbook. 2. ed. Sebastopol: O'Reilly Media, 2023. Disponível em: https://jakevdp.github.io/PythonDataScienceHandbook/. Acesso em: 26 jun. 2026.

7. Como Usar Este Repositório
7.1 Estrutura de arquivos
   miniguia-estudos-notebooklm/
├── README.md              # Documento principal (este arquivo)
├── LICENSE                # Licença MIT
├── sources/               # Cópias locais das fontes carregadas no NotebookLM
│   ├── vanderplas_handbook.pdf
│   ├── mckinney_pda.pdf
│   └── ...
├── prompts/               # Prompts reutilizáveis em formato .txt
│   ├── prompt_A_conceito.txt
│   ├── prompt_B_fluxo.txt
│   ├── prompt_C_debug.txt
│   ├── prompt_D_comparacao.txt
│   └── prompt_E_sintese.txt
└── notebook/              # Anotações e exercícios práticos
    └── eda_exemplo.ipynb
   
7.2 Passo a passo para reproduzir o estudo
Clone este repositório: git clone https://github.com/[SEU_USUARIO]/miniguia-estudos-notebooklm.git;
Crie um ambiente virtual: python -m venv .venv && source .venv/bin/activate (no Windows, use .venv\Scripts\activate);
Instale as dependências: pip install pandas numpy matplotlib seaborn jupyter;
Carregue as fontes da pasta sources/ no Google NotebookLM;
Reproduza os prompts da seção 5.3 e valide as respostas contra as fontes primárias;
Registre suas próprias iterações em notebook/, incluindo dificuldades e aprendizados.
7.3 Sugestões de personalização
Substitua [SEU_USUARIO] no link de clone pelo seu usuário real do GitHub;
Atualize a data de acesso nas referências bibliográficas para a data real da entrega;
Caso tenha escolhido fontes adicionais próprias, adicione-as à tabela da seção 2.2 e à lista de referências;
Considere adicionar uma pasta data/ com datasets de exemplo utilizados nos testes de prompt;
Para maior credibilidade, inclua capturas de tela das respostas obtidas no NotebookLM em uma pasta images/.
7.4 Entrega na plataforma DIO
Após finalizar a documentação:

Faça git add . && git commit -m "Entrega final do caderno temático" e git push para o GitHub;
Copie a URL principal do repositório (formato: https://github.com/[SEU_USUARIO]/miniguia-estudos-notebooklm);
Na página do Desafio de Projeto na DIO, clique em Entregar Projeto;
Cole o link do repositório, adicione uma descrição breve do tema estudado (2-3 linhas) e confirme a entrega.
Licença
Distribuído sob licença MIT. Consulte o arquivo LICENSE para mais detalhes. Você é livre para reutilizar, adaptar e distribuir este material, desde que mantenha a atribuição de autoria.

Este caderno temático foi elaborado como entrega do Desafio de Projeto da DIO, utilizando IA generativa (Google NotebookLM) como ferramenta de aprendizagem ativa, em conjunto com curadoria de fontes abertas e documentação pública do raciocínio iterativo.


---

## ✅ Pronto! Conteúdo completo em uma única mensagem

**Como usar:**

1. **Selecione todo o conteúdo** dentro do bloco de código acima (começa com `# Caderno Temático: Python para Análise de Dados` e termina com `... raciocínio iterativo._`)
2. **Copie** (Ctrl+C / Cmd+C)
3. Vá no GitHub: **https://github.com/new**
4. Crie o repositório com nome `miniguia-estudos-notebooklm`, marque **"Add a README file"** e clique em **Create repository**
5. Clique no `README.md` → ícone de lápis ✏️ (Edit this file)
6. **Apague todo o conteúdo padrão** e **cole** o texto copiado
7. Substitua `[SEU_USUARIO]` pelo seu usuário do GitHub (2 ocorrências) e a data `26 jun. 2026` pela data de hoje (5 ocorrências)
8. Clique em **Commit changes...** → **Commit changes**
9. Copie a URL do repositório e cole na página de entrega da DIO

Boa sorte na entrega! 🚀 Se precisar de mais alguma coisa, é só falar.
