# InvestigatorAI

### From Signals to Evidence

InvestigatorAI is an open-source AI-powered investigation platform designed to analyze evidence, connect entities, surface risk signals, and generate structured investigation insights.

The system combines Natural Language Processing, Face Intelligence, Voice Analysis, Sanctions Screening, Financial Crime Data, and Knowledge Graph reasoning into a unified investigation workflow.

---

## Supported Evidence Inputs

✓ Face Image  
✓ Voice Clip  
✓ Name / Alias  
✓ Email Metadata  
✓ Phone Metadata  
✓ Documents & Text Evidence  

---

## Key Features

| Module | Technology | Current Status |
|----------|-------------|---------------|
| Face Intelligence | ArcFace ResNet100 | Active |
| Voice Analysis | ECAPA-TDNN | Active |
| Named Entity Recognition | DeBERTa-v3 (21+ entity types) | Active |
| Sanctions Screening | OpenSanctions + Global Lists | Active |
| Financial Intelligence | FinCEN + Panama Papers integration | Active |
| Knowledge Graph | Neo4j | Active |
| Risk Engine | Evidence-based scoring | Active |

---

## Investigation Pipeline

```text
Input Evidence
(Face | Voice | Name | Documents)

            ↓

Entity Extraction
(NER + Metadata Processing)

            ↓

Evidence Normalization

            ↓

Sanction Screening

            ↓

Relationship Extraction

            ↓

Knowledge Graph

            ↓

Risk Analysis Engine

            ↓

Structured Investigation Report
