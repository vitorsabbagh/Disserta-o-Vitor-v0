# Comparative Analysis of Single and Multi-Agent Large Language Model Architectures for Domain-Specific Tasks in Well Construction

**Autor:** Vitor Brandão Sabbagh
**Orientador:** Prof. Geraldo Bonorino Xexéo, D.Sc.

Este repositório contém o código-fonte em LaTeX para a dissertação de mestrado intitulada "Comparative Analysis of Single and Multi-Agent Large Language Model Architectures for Domain-Specific Tasks in Well Construction".

## Resumo

Apresenta-se, nesta tese, a aplicação de grandes modelos de linguagem (LLM) no setor de petróleo e gás, especificamente em tarefas de construção e manutenção de poços. O estudo avalia o desempenho de uma arquitetura baseada em LLM de agente único e de múltiplos agentes no processamento de diferentes tarefas, oferecendo uma perspectiva comparativa sobre sua precisão e as implicações de custo de sua implementação. Os resultados indicam que sistemas multiagentes oferecem desempenho melhorado em tarefas de perguntas e respostas, com uma medida de veracidade 28\% maior do que os sistemas de agente único, mas a um custo financeiro mais alto. Especificamente, a arquitetura multiagente incorre em custos que são, em média, 3,7 vezes maiores do que os da configuração de agente único, devido ao aumento do número de tokens processados. Por outro lado, os sistemas de agente único se destacam em tarefas de texto para SQL (Linguagem de Consulta Estruturada), especialmente ao usar o Transformador Pré-Treinado Generativo 4 (GPT-4), alcançando uma pontuação 15\% maior em comparação com as configurações multiagentes, sugerindo que arquiteturas mais simples podem, às vezes, superar a complexidade. A novidade deste trabalho reside em seu exame original dos desafios específicos apresentados pelos dados complexos, técnicos e não estruturados inerentes às operações de construção de poços, contribuindo para o planejamento estratégico da adoção de aplicações de IA generativa, fornecendo uma base para otimizar soluções contra parâmetros econômicos e tecnológicos.

## Abstract

This article explores the application of large language models (LLM) in the oil and gas sector, specifically within well construction and maintenance tasks. The study evaluates the performances of a single-agent and a multi-agent LLM-based architecture in processing different tasks, offering a comparative perspective on their accuracy and the cost implications of their implementation. The results indicate that multi-agent systems offer improved performance in question and answer tasks, with a truthfulness measure 28\% higher than single-agent systems, but at a higher financial cost. Specifically, the multi-agent architecture incurs costs that are, on average, 3.7 times higher than those of the single-agent setup due to the increased number of tokens processed. Conversely, single-agent systems excel in text-to-SQL (Structured Query Language) tasks, particularly when using Generative Pre-Trained Transformer 4 (GPT-4), achieving a 15\% higher score compared to multi-agent configurations, suggesting that simpler architectures can sometimes outpace complexity. The novelty of this work lies in its original examination of the specific challenges presented by the complex, technical, unstructured data inherent in well construction operations, contributing to strategic planning for adopting generative AI applications, providing a basis for optimizing solutions against economic and technological parameters.

## Estrutura do Projeto

O projeto está organizado da seguinte forma:

- `main.tex`: O arquivo principal do LaTeX que une todas as partes do documento.
- `part*.tex`: Arquivos que contêm os capítulos individuais da dissertação (Introdução, Revisão Bibliográfica, Experimentos, Conclusão).
- `bib.bib`: O arquivo de bibliografia no formato BibTeX.
- `coppe.cls`: A classe LaTeX da COPPE/UFRJ utilizada para a formatação do documento.
- `images/`, `images_exp2/`: Diretórios que armazenam as imagens e figuras utilizadas no texto.
- `data/`: Diretório para dados utilizados nos experimentos.

## Como Compilar

Para gerar o arquivo PDF da dissertação, é necessário ter uma distribuição LaTeX instalada (como TeX Live, MiKTeX ou MacTeX).

O método recomendado para a compilação é utilizando o `latexmk`. Com o `latexmk` instalado, execute o seguinte comando na raiz do projeto:

```bash
latexmk -pdf main.tex
```

Este comando cuidará de todas as compilações necessárias (LaTeX, BibTeX, etc.) na ordem correta e gerará o arquivo `main.pdf`.

Para limpar os arquivos auxiliares gerados durante a compilação, você pode usar:

```bash
latexmk -c
```

## Dependências

- Uma distribuição LaTeX completa.
- O `latexmk` (geralmente incluído nas distribuições LaTeX modernas).
