# GitHub Implementations

This section contains publicly available GitHub repositories implementing methods or systems related to scientific claim verification, literature retrieval, citation-supported generation, hallucination detection, and scientific literature question answering.

Repositories were selected based on their connection to published research or recognized research projects, availability of source code, documentation, and relevance to the research topic.

---

## 1. SciFact

**Repository:** [allenai/scifact](https://github.com/allenai/scifact)

**Research Area:** Scientific claim verification

**Description:**
Official implementation and dataset repository for the SciFact scientific claim-verification task. The repository includes data, evaluation scripts, training code, pretrained models, and instructions for verifying scientific claims against evidence documents.

**Why it is relevant:**
SciFact directly addresses whether scientific claims are supported or contradicted by evidence and therefore provides a strong implementation reference for evaluating LLM factual reliability.

**Associated Paper:**
Wadden et al. (2020), *Fact or Fiction: Verifying Scientific Claims*.

---

## 2. MultiVerS

**Repository:** [dwadden/multivers](https://github.com/dwadden/multivers)

**Research Area:** Scientific claim verification

**Description:**
MultiVerS is a model and research codebase for scientific claim verification. The repository provides model checkpoints, training and inference code, and support for scientific claim-verification datasets including SciFact, CovidFact, and HealthVer.

**Why it is relevant:**
MultiVerS demonstrates how full-document context, retrieval, and scientific evidence can be integrated into a claim-verification pipeline.

**Associated Paper:**
Wadden et al. (2022), *MultiVerS: Improving Scientific Claim Verification with Weak Supervision and Full-Document Context*. Findings of NAACL 2022.

**Repository:**
[GitHub](https://github.com/dwadden/multivers)

---

## 3. LitSearch

**Repository:** [princeton-nlp/LitSearch](https://github.com/princeton-nlp/LitSearch)

**Research Area:** Scientific literature retrieval

**Description:**
Official code and data for the LitSearch benchmark. The repository contains evaluation code for scientific literature retrieval and implementations of baseline retrieval and LLM-based reranking approaches.

**Why it is relevant:**
Retrieval is a critical first stage in evidence-grounded scientific analysis. An LLM cannot reliably synthesize literature if the relevant research is not retrieved in the first place.

**Associated Paper:**
Ajith et al. (2024), *LitSearch: A Retrieval Benchmark for Scientific Literature Search*. EMNLP 2024.

**Repository:**
[GitHub](https://github.com/princeton-nlp/LitSearch)

---

## 4. ALCE

**Repository:** [princeton-nlp/ALCE](https://github.com/princeton-nlp/ALCE)

**Research Area:** Citation-supported LLM generation

**Description:**
ALCE provides code and data for evaluating language-model-generated answers with citations. The repository contains evaluation tools covering answer quality and citation quality, together with benchmark datasets and baseline implementations.

**Why it is relevant:**
The presence of a citation does not guarantee that a generated scientific claim is actually supported by that source. ALCE is therefore directly relevant to citation-grounded reliability evaluation.

**Associated Paper:**
Gao, T., Yen, H., Yu, J., & Chen, D. (2023). *Enabling Large Language Models to Generate Text with Citations*. EMNLP 2023.

**Repository:**
[GitHub](https://github.com/princeton-nlp/ALCE)

---

## 5. SelfCheckGPT

**Repository:** [potsawee/selfcheckgpt](https://github.com/potsawee/selfcheckgpt)

**Research Area:** Hallucination detection

**Description:**
Official implementation of SelfCheckGPT, which evaluates the consistency of multiple generations from a language model as a signal for detecting hallucinated information. The repository contains several SelfCheck variants, including BERTScore, QA, n-gram, and NLI-based approaches.

**Why it is relevant:**
Hallucination is one of the central reliability risks in scientific literature analysis. SelfCheckGPT provides an implementation that can be incorporated into experiments investigating unsupported or inconsistent generated claims.

**Associated Paper:**
Manakul, P., Liusie, A., & Gales, M. J. F. (2023). *SelfCheckGPT: Zero-Resource Black-Box Hallucination Detection for Generative Large Language Models*. EMNLP 2023.

**Repository:**
[GitHub](https://github.com/potsawee/selfcheckgpt)

---

## 6. PaperQA / PaperQA2

**Repository:** [Future-House/paper-qa](https://github.com/Future-House/paper-qa)

**Research Area:** Scientific retrieval-augmented generation

**Description:**
PaperQA is an open-source system focused on question answering over scientific literature. The current repository provides PaperQA2, an agentic retrieval-augmented system that can process scientific documents, retrieve evidence, and generate answers with citations.

**Why it is relevant:**
PaperQA closely resembles the type of workflow required for scientific literature analysis: document retrieval, evidence selection, synthesis, citation generation, and question answering.

**Related Research:**
Lála, J., O'Donoghue, O., Shtedritski, A., Cox, S., Rodriques, S. G., & White, A. D. (2023). *PaperQA: Retrieval-Augmented Generative Agent for Scientific Research*. arXiv:2312.07559.

**Original Paper:**
[arXiv](https://arxiv.org/abs/2312.07559)

**Current Implementation:**
[GitHub](https://github.com/Future-House/paper-qa)

---

## Implementation Selection Criteria

The repositories above were selected using the following criteria:

| Criterion                | Purpose                                                                         |
| ------------------------ | ------------------------------------------------------------------------------- |
| Research connection      | Repository is linked to a paper or established research project                 |
| Source-code availability | Implementation is publicly accessible                                           |
| Documentation            | Repository explains setup and usage                                             |
| Relevance                | Implementation addresses at least one component of the research topic           |
| Reproducibility          | Code, data, checkpoints, or evaluation procedures are provided where applicable |
| Licensing                | Repository provides identifiable licensing information                          |

---

## How These Implementations Fit Together

The repositories cover complementary parts of a reliable scientific-LLM pipeline:

**LitSearch** → retrieve relevant literature
**PaperQA** → retrieve and synthesize evidence
**SciFact / MultiVerS** → verify scientific claims
**ALCE** → evaluate citation-supported generation
**SelfCheckGPT** → detect potential hallucination or inconsistency

This makes the collection useful not only as a list of repositories, but also as a starting point for designing an end-to-end reliability evaluation pipeline.

