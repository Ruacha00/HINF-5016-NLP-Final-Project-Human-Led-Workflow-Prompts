# HINF-5016 NLP Final Project — Human-Led Workflow Prompts

This repository contains structured prompt templates for writing a course literature review on:

**“Early ICU Mortality Prediction Using Time-Series Data: Multi-Window Modeling and Cross-Dataset Generalization Evaluation.”**

The prompts are designed for a **human-led workflow**: the user supplies evidence from reviewed papers, and the model helps transform that evidence into publishable section drafts without fabricating claims.

## Purpose

This repository supports a staged academic writing process for AMIA-style literature reviews by providing:

- section-specific writing prompts,
- synthesis-note generation prompts,
- strict constraints to reduce hallucination,
- ordered workflow guidance from Methods through Abstract.

## Repository Contents

- `section_writing_prompts.md`  
  End-to-end prompt set for drafting each section of the paper in recommended order:
  1. Methods  
  2. Related Work / Results  
  3. Discussion  
  4. Introduction  
  5. Conclusion  
  6. Abstract

- `synthesis_notes_prompts.md`  
  Prompt template for generating cross-paper synthesis notes (themes, trends, tensions, gaps, future directions) from completed paper evaluation sheets.

## Core Workflow

1. Complete your per-paper evaluation template (for all included studies).
2. Use `synthesis_notes_prompts.md` to generate structured synthesis notes.
3. Use `section_writing_prompts.md` section-by-section in order.
4. Review each generated section manually before moving to the next.
5. Finalize Abstract last, using finalized section openings.

## Prompting Principles Enforced in This Repo

- Use only user-provided evidence.
- Do not invent citations, metrics, or claims.
- Omit or hedge weakly supported points (e.g., mark uncertainty where needed).
- Prefer cross-paper synthesis over paper-by-paper summaries.
- Keep output aligned to AMIA-style length and tone constraints.

## Recommended Use

These prompts are intended for:

- graduate health informatics coursework,
- literature review drafting with LLM assistance,
- transparent human-in-the-loop writing workflows.

They can be adapted to adjacent clinical NLP/ML review topics by replacing the source notes and paper evidence while preserving the workflow structure.

## Notes

- This repository currently emphasizes **prompt assets**, not code.
- Add your finalized manuscript, references, and evaluation tables separately if you want the repo to serve as a full reproducible writing package.

## Maintainer

- GitHub: [@Ruacha00](https://github.com/Ruacha00)
