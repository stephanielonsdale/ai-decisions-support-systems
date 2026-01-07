# AI Decision Support Systems  
### Applied Machine Learning & Generative AI for High-Stakes Decision Making

This repository contains applied AI systems designed to **support human decision-making in complex, high-stakes domains**.  
Rather than replacing human judgment, these systems provide **structured analysis, evidence retrieval, and interpretable insights** to inform better decisions under uncertainty.

The projects in this repository focus on:
- Human-in-the-loop AI
- Grounded, explainable outputs
- Real-world constraints and risk awareness
- Responsible use of machine learning and generative AI

---

## Projects Overview

### 1. Research Proposal NOFO Assistant (RAG-Based Decision Support)

**Notebook:** `researchproposalaiassistant.ipynb`

This project implements a **Retrieval-Augmented Generation (RAG)** system to support the development of **federally compliant healthcare research proposals**, grounded in official policy documents and prior research evidence.

#### Problem
Writing competitive grant proposals requires:
- Interpreting dense NOFO and application guidance
- Ensuring strict policy compliance
- Grounding claims in prior research
- Avoiding unsupported or hallucinated content
- Iteratively refining technical approaches

Traditional LLMs alone are insufficient due to hallucination risk and lack of policy grounding.

#### Solution
This system provides **AI-assisted decision support** by:
- Ingesting NOFOs, application guides, and research papers
- Chunking and embedding documents into vector stores
- Retrieving relevant policy and evidence context
- Applying query expansion and reranking for relevance
- Generating proposal components constrained to retrieved sources
- Supporting iterative refinement and evaluation

#### Key Capabilities
- Policy-aware semantic retrieval
- Evidence-grounded LLM generation
- Query expansion for ambiguous user inputs
- Reranking to prioritize the most relevant context
- Transparent, inspectable retrieval results
- Designed explicitly for **human review and oversight**

#### Technologies
- Python
- LangChain
- OpenAI / LLM APIs
- FAISS / vector stores
- Sentence Transformers
- PDF ingestion and text chunking

#### Decision Support Focus
This system supports **research, compliance, and funding strategy decisions** where incorrect or hallucinated outputs carry real consequences.

---

### 2. NFL Player Sentiment & Performance Analysis

**Notebook:** `NFL_Sentiment_Player_Performance.ipynb`

This project applies machine learning and natural language processing to analyze the relationship between **public sentiment** and **player performance** in professional sports.

#### Problem
Decision-makers in sports analytics, media, and management must interpret large volumes of subjective sentiment data (e.g., commentary, public discourse) alongside objective performance metrics.

Manual analysis is inconsistent and difficult to scale.

#### Solution
This system provides decision support by:
- Performing sentiment analysis on text data related to NFL players
- Aggregating sentiment scores across time and players
- Linking sentiment trends to performance indicators
- Supporting exploratory analysis and pattern discovery

#### Key Capabilities
- Text preprocessing and sentiment scoring
- Feature engineering for temporal and player-level analysis
- Visualization of sentiment vs. performance trends
- Interpretable outputs suitable for human decision-making

#### Technologies
- Python
- pandas, NumPy
- NLP sentiment analysis tools
- Data visualization (matplotlib / seaborn)

#### Decision Support Focus
This project demonstrates how AI can support **performance evaluation, media analysis, and strategic interpretation** rather than producing automated decisions.

---

## Design Principles Across Projects

- **Human-in-the-Loop:** AI supports, not replaces, expert judgment  
- **Transparency:** Intermediate outputs (retrievals, scores, rankings) are visible  
- **Grounded Reasoning:** Outputs are tied to evidence where required  
- **Risk Awareness:** Designed for domains where incorrect outputs matter  
- **Scalability:** Methods generalize to other decision-heavy domains  

---

## Repository Structure
ai-decision-support-systems/
│
├── researchproposalaiassistant.ipynb
├── NFL_Sentiment_Player_Performance.ipynb
├── README.md
└── requirements.txt


---

## Intended Use

These projects are intended for:
- Research and policy teams
- Data-driven decision makers
- Applied AI and ML practitioners
- Evaluating AI systems for responsible, real-world deployment

They are **not** intended to produce final decisions without human oversight.

---

## Author

**Stephanie Lonsdale**  
Applied AI Graduate Student (M.S. Artificial Intelligence)  
Johns Hopkins University  

---

## License

MIT License


