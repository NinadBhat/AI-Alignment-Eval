# Responsible Quote Alignment Eval


This project evaluates the alignment of language models (LLMs) by testing how they handle quotes, particularly in ideologically sensitive contexts. Final reports are available in the `final_report.md` file.

**Team:** Aletheia

**Members (listed alphabetically):** Kabir, Ninad, Shantanu, Soumyadeep, Vanessa

---

## Motivation

Quotes are a powerful rhetorical tool. When misused, especially in political or historical contexts, they can lend false credibility to misleading narratives. A well-aligned model should:

- Distinguish between real and fabricated quotes
- Avoid confidently presenting false or unverifiable statements
- Encourage users to verify when appropriate
- Resist pressure to invent supporting "evidence" for ideological positions

---

## Evaluations

### Study A: Role-Based Sycophancy

Tests if a model favors the user's point of view depending on social roles (e.g., *me* vs *my professor*).

- Generates quotes for opposing ideologies
- Swaps roles to test for consistency
- Classifies which ideology the quote supports
- Computes a sycophancy score

### Study B: Confirmation Bias (Vanessa’s Benchmark)

Evaluates whether a model is biased toward classifying quotes as "real" if they align with themes associated with the quoted figure.

- Uses real and fake quotes, both neutral and ideologically loaded
- Initial benchmark uses Stalin and communism
- Outputs confusion matrices
- Observes vibe-based vs factual classification

---

## How to Use

- Run `study_a_sycophancy_quotes.ipynb` to execute Study A.
- Run `study_b_confirmation_bias.ipynb` for Study B.
- Requires access to Gemini API and optional dataset inputs.
- Final reports can be found in the `final_report.md` file.

---

## Goals

- Measure ideological alignment and hallucination tendencies
- Compare model responses across social framing
- Identify sycophancy and confirmation bias patterns
