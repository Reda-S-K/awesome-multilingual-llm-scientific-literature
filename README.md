# Awesome Multilingual LLM Scientific Analysis

A curated research repository on **evaluating the multilingual reliability of Large Language Models (LLMs) in scientific literature analysis**.

This repository brings together verified scholarly papers, scientific datasets, research tools, GitHub implementations, and learning resources relevant to multilingual LLM evaluation, scientific information retrieval, factuality, hallucination detection, evidence grounding, and citation reliability.

The goal is to provide a reusable starting point for students and researchers studying whether scientific information remains accurate, consistent, and evidence-grounded when LLMs operate across different languages.

---

## Contents

* [Overview](#overview)
* [AI-Assisted Research Paper](#ai-assisted-research-paper)
* [Citation Integrity Audit](#citation-integrity-audit)
* [Survey and Overview Papers](#survey-and-overview-papers)
* [Multilingual Large Language Models](#multilingual-large-language-models)
* [Multilingual Evaluation](#multilingual-evaluation)
* [Scientific Language Models and Literature Analysis](#scientific-language-models-and-literature-analysis)
* [Factuality, Hallucination and Citation Reliability](#factuality-hallucination-and-citation-reliability)
* [Datasets](#datasets)
* [Tools and Libraries](#tools-and-libraries)
* [GitHub Implementations](#github-implementations)
* [Tutorials and Learning Resources](#tutorials-and-learning-resources)
* [References](#references)
* [License](#license)

---

## Overview

Large Language Models are increasingly used to search, summarize, explain, compare, and synthesize scientific literature. Multilingual LLMs extend these capabilities to users who interact with AI systems in languages other than English. However, the ability to produce fluent multilingual text does not necessarily mean that a model preserves scientific reliability across languages.

Scientific literature analysis requires several properties beyond ordinary language fluency. A reliable system should preserve technical terminology, numerical information, uncertainty, causal relationships, methodological details, and the distinction between evidence and interpretation. It should also retrieve appropriate scientific sources and provide citations that genuinely support its claims.

This repository focuses on these challenges by bringing together work from multilingual natural language processing, scientific NLP, scientific question answering, information retrieval, factuality evaluation, hallucination detection, and citation-grounded generation.

A central research question is:

> **When a scientifically equivalent task is performed in different languages, does an LLM produce consistent, factually correct, and evidence-grounded results?**

The repository therefore emphasizes **cross-lingual consistency, scientific factuality, evidence grounding, citation validity, retrieval quality, and reliability evaluation**.

---

## AI-Assisted Research Paper

### Evaluating Multilingual Reliability of Large Language Models in Scientific Literature Analysis

This research paper provides the theoretical foundation for this repository. It reviews multilingual LLMs, scientific language models, multilingual benchmarks, scientific literature retrieval, factuality, hallucination, citation grounding, research challenges, and future directions.

**Paper:**
[Read the AI-Assisted Research Paper](paper/AI_Assisted_Research_Paper.pdf)

---

## Citation Integrity Audit

The research paper was developed with assistance from generative AI. Because AI-generated references may contain incorrect bibliographic details or unsupported claims, the references are independently checked before being included in the curated repository.

The citation audit records the verification of:

* Paper existence
* Title
* Authors
* Publication year
* Journal or conference
* DOI or persistent identifier
* Link correctness
* Relevance to the cited claim

**Audit:**
[View Citation Integrity Audit](citation-audit/Citation_Integrity_Audit.pdf)

---

## Survey and Overview Papers

The following works provide broad background for multilingual LLMs and scientific language models.

* **A Survey of Multilingual Large Language Models** — Qin et al. (2025)
  A broad survey of multilingual LLM architectures, training, alignment, evaluation, and research challenges.

* **A Comprehensive Survey of Scientific Large Language Models and Their Applications in Scientific Discovery** — Zhang et al. (2024)
  Surveys scientific LLMs, datasets, evaluation methods, and applications in scientific discovery.

[View all verified references](references/references.md)

---

## Multilingual Large Language Models

### BLOOM

**BigScience Workshop (2022)**
A large open-access multilingual language model developed through the BigScience collaboration.

[arXiv](https://arxiv.org/abs/2211.05100)

### Aya

**Üstün et al. (2024)**
An instruction-tuned multilingual language model covering 101 languages and evaluated across multilingual tasks.

[ACL Anthology](https://aclanthology.org/2024.acl-long.845/)
[arXiv](https://arxiv.org/abs/2402.07827)

[View the full paper collection](references/references.md)

---

## Multilingual Evaluation

### XTREME-R

A multilingual benchmark covering 50 languages and multiple natural-language-understanding tasks.

[Paper](https://aclanthology.org/2021.emnlp-main.802/)

### FLORES-101

A multilingual and low-resource machine-translation evaluation benchmark.

[Paper](https://aclanthology.org/2022.tacl-1.30/)

### MEGAVERSE

A multilingual benchmark evaluating LLMs across multiple languages, modalities, models, and tasks.

[Paper](https://aclanthology.org/2024.naacl-long.143/)

### Global MMLU

An evaluation framework examining linguistic and cultural effects in multilingual benchmark construction.

[Paper](https://aclanthology.org/2025.acl-long.919/)

### MMLU-ProX

A multilingual reasoning benchmark supporting comparisons of advanced LLM performance across languages.

[arXiv](https://arxiv.org/abs/2503.10497)

### ScholarBench

A bilingual academic benchmark covering abstraction, comprehension, and reasoning across research domains.

[Paper](https://aclanthology.org/2025.findings-emnlp.465/)

[View all verified references](references/references.md)

---

## Scientific Language Models and Literature Analysis

### SciBERT

A scientific-domain pretrained language model designed for processing scientific publications.

[Paper](https://aclanthology.org/D19-1371/)

### Galactica

A large language model trained with scientific material and designed for scientific knowledge and reasoning tasks.

[arXiv](https://arxiv.org/abs/2211.09085)

### PubMedQA

A biomedical research question-answering benchmark requiring reasoning over scientific abstracts.

[Paper](https://aclanthology.org/D19-1259/)

### SciFact

A scientific claim-verification benchmark based on evidence from scientific abstracts.

[Paper](https://aclanthology.org/2020.emnlp-main.609/)

### SciReviewGen

A dataset designed for automatic scientific literature-review generation.

[Paper](https://aclanthology.org/2023.findings-acl.418/)

### LitSearch

A benchmark for retrieving relevant scientific papers in response to realistic research questions.

[Paper](https://aclanthology.org/2024.emnlp-main.840/)

### PaperQA

A retrieval-augmented approach for answering questions using scientific papers and evidence.

[arXiv](https://arxiv.org/abs/2312.07559)

[View the full reference collection](references/references.md)

---

## Factuality, Hallucination and Citation Reliability

### FActScore

Evaluates generated long-form text by decomposing it into atomic facts and measuring factual support.

[Paper](https://aclanthology.org/2023.emnlp-main.741/)

### SelfCheckGPT

Uses consistency across multiple generations to identify potentially hallucinated information.

[Paper](https://aclanthology.org/2023.emnlp-main.557/)

### ALCE

Evaluates language-model-generated answers with citations, including citation quality and answer correctness.

[Paper](https://aclanthology.org/2023.emnlp-main.398/)

[View all verified references](references/references.md)

---

## Datasets

The repository includes datasets and corpora covering multilingual evaluation, scientific literature, and scientific claim verification.

### S2ORC

Large-scale scientific literature corpus supporting NLP, information retrieval, document mining, and citation analysis.

[Dataset Repository](https://github.com/allenai/s2orc)

### SciFact

Scientific claim-verification dataset connecting claims with supporting or contradicting evidence.

[Dataset Repository](https://github.com/allenai/scifact)

### FLORES-200

Multilingual evaluation benchmark supporting low-resource and multilingual translation research.

[Dataset Repository](https://github.com/facebookresearch/flores)

[View dataset details](datasets/datasets.md)

---

## Tools and Libraries

### Hugging Face Transformers

Library for loading, running, evaluating, and fine-tuning pretrained transformer models.

[Official Repository](https://github.com/huggingface/transformers)

### Hugging Face Datasets

Library for loading, processing, and preparing datasets for machine-learning experiments.

[Official Repository](https://github.com/huggingface/datasets)

### FAISS

Library for efficient similarity search and vector indexing.

[Official Repository](https://github.com/facebookresearch/faiss)

### Stanza

Stanford NLP library supporting processing of many human languages.

[Official Repository](https://github.com/stanfordnlp/stanza)

### SciSpaCy

Scientific and biomedical NLP pipelines built around spaCy.

[Official Repository](https://github.com/allenai/scispacy)

### Semantic Scholar API

Programmatic access to scholarly paper and author metadata.

[API Documentation](https://api.semanticscholar.org/api-docs/)

[View all tools](tools/tools.md)

---

## GitHub Implementations

### SciFact

Scientific claim-verification code and dataset.

[GitHub](https://github.com/allenai/scifact)

### MultiVerS

Research implementation for scientific claim verification using document context.

[GitHub](https://github.com/dwadden/multivers)

### LitSearch

Code and data for scientific literature retrieval evaluation.

[GitHub](https://github.com/princeton-nlp/LitSearch)

### ALCE

Implementation and evaluation resources for citation-supported LLM generation.

[GitHub](https://github.com/princeton-nlp/ALCE)

### SelfCheckGPT

Implementation of black-box hallucination detection methods.

[GitHub](https://github.com/potsawee/selfcheckgpt)

### PaperQA / PaperQA2

Scientific retrieval-augmented question-answering implementation.

[GitHub](https://github.com/Future-House/paper-qa)

[View repository details](implementations/github-repositories.md)

---

## Tutorials and Learning Resources

### 1. Hugging Face LLM Course

A practical course covering transformer models, datasets, fine-tuning, and modern LLM workflows.

[Hugging Face LLM Course](https://huggingface.co/learn/llm-course/chapter0/1)

### 2. Stanford CS224N: Natural Language Processing with Deep Learning

A university-level course covering NLP, neural networks, transformers, LLMs, retrieval-augmented generation, and evaluation.

[Stanford CS224N](https://web.stanford.edu/class/cs224n/)

### 3. Speech and Language Processing

The online third-edition draft by Daniel Jurafsky and James H. Martin provides comprehensive coverage of NLP, transformers, LLMs, information retrieval, RAG, machine translation, and related topics.

[Speech and Language Processing](https://web.stanford.edu/~jurafsky/slp3/)

### 4. Semantic Scholar Academic Graph API

Official documentation for programmatic access to paper, author, and citation metadata.

[Semantic Scholar API](https://api.semanticscholar.org/api-docs/)

### 5. Crossref REST API

Official documentation for searching and retrieving scholarly metadata, DOI records, works, journals, and related information.

[Crossref REST API](https://api.crossref.org/)

---

## References

The repository contains a separate curated collection of verified scholarly references covering:

* Multilingual LLMs
* Multilingual evaluation
* Scientific language models
* Scientific literature retrieval
* Scientific question answering
* Factuality
* Hallucination detection
* Citation-supported generation

[Open the verified research-paper collection](references/references.md)

---

## Repository Structure

```text
awesome-multilingual-llm-scientific-analysis/
│
├── README.md
│
├── paper/
│   └── AI_Assisted_Research_Paper.pdf
│
├── citation-audit/
│   └── Citation_Integrity_Audit.pdf
│
├── references/
│   └── references.md
│
├── datasets/
│   └── datasets.md
│
├── tools/
│   └── tools.md
│
├── implementations/
│   └── github-repositories.md
│
└── tutorials/
    └── learning-resources.md
```

---

## Research Scope

This repository focuses on the following interconnected research problems:

```text
Multilingual LLMs
       │
       ▼
Cross-Lingual Evaluation
       │
       ▼
Scientific Literature Retrieval
       │
       ▼
Evidence Extraction
       │
       ▼
Scientific Reasoning
       │
       ├──────────────► Factuality
       │
       ├──────────────► Hallucination Detection
       │
       └──────────────► Citation Verification
                              │
                              ▼
                    Multilingual Reliability
```

The central objective is to understand whether the reliability of scientific literature analysis changes when the language of the query, evidence, or generated answer changes.

---

## Curation Principles

The resources in this repository are selected according to the following principles:

1. **Scholarly relevance**
   Papers should have a clear relationship with multilingual NLP, scientific NLP, information retrieval, factuality, or LLM evaluation.

2. **Verification**
   Bibliographic information should be checked using authoritative scholarly sources.

3. **Research usefulness**
   Datasets, tools, and implementations should provide practical value for research or experimentation.

4. **Traceability**
   Wherever possible, resources are linked to their official publisher, repository, DOI, arXiv record, or documentation page.

5. **No unauthorized redistribution**
   Copyrighted papers are linked rather than uploaded unless redistribution is explicitly permitted.

---

## Citation and Reference Policy

Generative AI may be used to discover or organize candidate resources, but the final repository is manually curated and references are independently checked.

A resource is not considered verified simply because it was suggested by an AI system.

---

## License

This repository's original documentation and original content are released under the **MIT License**, unless otherwise stated.

Third-party papers, datasets, software, logos, and other external resources remain subject to their respective copyright and license terms.

See the repository's [`LICENSE`](LICENSE) file for details.

---

## Acknowledgement

This repository was created as part of the **AI Tools for Research** course activity on GitHub-based research curation and documentation.

The repository combines AI-assisted research with independent verification, scholarly curation, and documentation.
