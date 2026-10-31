# Cynbit AI/ML Engineer Intern Task

This repository contains an AI opportunity analysis for Cynbit Technologies and a runnable proof of concept for a Revio Review Action Desk.

## Deliverables

- [AI Opportunity Report](AI_Opportunity_Report.md): public-source company context, industry signals, opportunity shortlist, recommendation, pilot scope, and success measures.
- [Technical Approach Report](Technical_Approach_Report.md): model choices, data pipeline, prompt design, evaluation plan, delivery plan, and risks.
- [Review Copilot prototype](review_copilot.py): local review triage and response drafting, with optional OpenAI API mode.
- [Fictional sample reviews](sample_reviews.csv): demo input only.

## Run the local demo

The default mode has no external dependencies or credentials:

```bash
python review_copilot.py --sample
python review_copilot.py --input sample_reviews.csv --output triaged_reviews.csv
```

Every generated reply is a draft and requires human approval. Sensitive or low-rating reviews are flagged for escalation. The local baseline is a small, explainable heuristic and is not a trained or production-ready model.

## Scope and sources

The sample data is fictional; no Cynbit internal or customer data was available. The reports distinguish publicly visible facts from hypotheses to validate with Cynbit and its customers. Source links are included in the opportunity report and technical report.
