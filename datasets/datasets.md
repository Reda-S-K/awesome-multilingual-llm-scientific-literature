# Datasets

This section lists datasets and research corpora that are useful for evaluating multilingual reliability, scientific information retrieval, scientific claim verification, and language-model performance on research-oriented text.

The selected resources complement the repository's focus on multilingual evaluation and scientific literature analysis. They can be used for retrieval, claim verification, translation evaluation, biomedical question answering, and large-scale scientific-text processing.

---

## 1. S2ORC — Semantic Scholar Open Research Corpus

**Source:** Allen Institute for AI / Semantic Scholar
**Type:** Scientific literature corpus
**Primary Use:** Scientific NLP, information retrieval, citation analysis, document mining

S2ORC is a large-scale corpus designed for natural language processing and text-mining research over scientific papers. It provides structured bibliographic metadata, abstracts, full-text information for eligible papers, and citation relationships. The resource is particularly useful for experiments involving scientific-document retrieval, evidence extraction, and citation-aware literature analysis.

**Why it is relevant:**
A multilingual scientific-literature system needs access to a large research corpus for retrieval and evidence analysis. S2ORC provides an important infrastructure for studying scientific documents and citation networks.

**Official Repository:**
[S2ORC on GitHub](https://github.com/allenai/s2orc)

**Semantic Scholar:**
[Semantic Scholar](https://www.semanticscholar.org/)

**Paper:**
Lo, K., Wang, L. L., Neumann, M., Kinney, R., & Weld, D. S. (2020). *S2ORC: The Semantic Scholar Open Research Corpus*. Proceedings of ACL 2020.

[ACL Anthology](https://aclanthology.org/2020.acl-main.447/)
[DOI](https://doi.org/10.18653/v1/2020.acl-main.447)

**License / Usage:**
The original S2ORC repository specifies the **Open Data Commons Attribution License (ODC-By 1.0)**. Users should consult the current dataset terms before redistribution or large-scale reuse.

---

## 2. SciFact

**Source:** Allen Institute for AI
**Type:** Scientific claim-verification dataset
**Primary Use:** Scientific fact checking, evidence retrieval, claim verification

SciFact is a dataset for verifying scientific claims using evidence retrieved from scientific abstracts. Claims are associated with evidence documents and labels indicating whether the evidence supports or contradicts the claim.

**Why it is relevant:**
Scientific LLM reliability depends on whether generated claims can be supported by research evidence. SciFact directly represents this problem and is therefore highly relevant for evaluating factuality and evidence grounding.

**Official Repository:**
[SciFact on GitHub](https://github.com/allenai/scifact)

**Dataset Documentation:**
[SciFact Data Documentation](https://github.com/allenai/scifact/blob/master/doc/data.md)

**Paper:**
Wadden, D., Lin, S., Lo, K., Wang, L. L., van Zuylen, M., Cohan, A., & Hajishirzi, H. (2020). *Fact or Fiction: Verifying Scientific Claims*. Proceedings of EMNLP 2020.

[ACL Anthology](https://aclanthology.org/2020.emnlp-main.609/)
[DOI](https://doi.org/10.18653/v1/2020.emnlp-main.609)

**License / Usage:**
Consult the official repository and dataset documentation for the current terms governing use and redistribution.

---

## 3. FLORES-200

**Source:** Meta AI / Facebook Research
**Type:** Multilingual machine-translation evaluation dataset
**Primary Use:** Multilingual translation evaluation, low-resource language evaluation

FLORES-200 is a multilingual evaluation benchmark containing professionally translated and aligned text for a large number of languages. It was designed to improve evaluation of multilingual and low-resource machine translation systems.

**Why it is relevant:**
Language switching and translation are important components of multilingual scientific analysis. FLORES-200 can be used to study whether a model preserves meaning and performs consistently across different languages.

**Official Repository:**
[FLORES on GitHub](https://github.com/facebookresearch/flores)

**FLORES-200 Documentation:**
[FLORES-200 README](https://github.com/facebookresearch/flores/blob/main/flores200/README.md)

**Dataset on Hugging Face:**
[FLORES on Hugging Face](https://huggingface.co/datasets/facebook/flores)

**Paper:**
Goyal, N., Gao, C., Chaudhary, V., Chen, P.-J., Wenzek, G., Ju, D., Krishnan, S., Ranzato, M.-A., Guzmán, F., & Fan, A. (2022). *The FLORES-101 Evaluation Benchmark for Low-Resource and Multilingual Machine Translation*. **Transactions of the Association for Computational Linguistics, 10**, 522–538.

[ACL Anthology](https://aclanthology.org/2022.tacl-1.30/)
[DOI](https://doi.org/10.1162/tacl_a_00474)

**License:**
The official FLORES repository identifies FLORES-200 as **CC-BY-SA 4.0**.

**Important Note:**
The original Facebook Research FLORES repository is archived. The repository itself points users toward newer FLORES resources maintained by the Open Language Data Initiative.

---

## Dataset Selection Rationale

These datasets were selected because they represent different components of the research problem:

| Dataset    | Main Research Dimension                               |
| ---------- | ----------------------------------------------------- |
| S2ORC      | Scientific literature retrieval and document analysis |
| SciFact    | Scientific claim verification and evidence grounding  |
| FLORES-200 | Multilingual and low-resource language evaluation     |

Together, they support a research pipeline involving:

**multilingual input → retrieval → scientific evidence extraction → claim verification → cross-lingual reliability evaluation**

---

## Responsible Use

Dataset users should review the official documentation and licensing conditions before downloading, modifying, redistributing, or publishing derived datasets.

This repository links to the official dataset sources rather than redistributing the datasets themselves.

