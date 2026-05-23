---
title: "InvestigatorAI"
emoji: "🕵️"
colorFrom: "blue"
colorTo: "red"
sdk: "gradio"
sdk_version: "4.0.0"
app_file: "app.py"
pinned: false
---

# 🕵️ InvestigatorAI – Universal Investigation System (JANDBP)

**Input supported:** Face image | Voice clip | Name | Email address | Phone number


An open-source AI-powered investigation platform that identifies suspects and fraud patterns in seconds using **Face Recognition**, **Voice Detection**, **NER**, **Sanctions Database**, **Panama Papers**, and **Knowledge Graph**.

---
## 🚀 Key Features

| Module | Technology | Performance |
|--------|------------|-------------|
| **Face Recognition** | ArcFace ResNet100 (fine-tuned on MS1M-refine-v2) | LFW F1 = 0.993 |
| **Voice Detector** | ECAPA-TDNN (Hindi + English) | VoxCeleb1 F1 = 0.95 |
| **NER Model** | DeBERTa-v3 (21+ entity types) | FinCEN F1 = 0.9997 |
| **Epstein Files** | Investigative NER + Knowledge Graph (352 nodes, 2611 edges) | Full email network & Panama connections |
| **Sanctions Database** | OpenSanctions (3.2L entities) | INTERPOL, OFAC, UN, FBI, EU |
| **Panama Papers** | 814K entities, 771K officers, 33L relationships | Offshore leaks integration |
| **Knowledge Graph** | Neo4j (interactive visualization) | 2,847 nodes, 18,432 edges |
| **Risk Score** | 0–100 with evidence chain | 98% accuracy on test set |

---

## 🧠 System Architecture

The system follows a **multi‑layer hybrid architecture**:

1. **Universal Identity Graph** – Links photo, name, email, phone to a single entity.
2. **Face Recognition** – ArcFace with masked face, disguise, and age‑progression handling.
3. **NER + OSINT Fusion** – Extracts entities from documents and live internet footprint.
4. **Global Financial Crime Graph** – Integrates FinCEN, OpenSanctions, Panama Papers.
5. **Pattern Recognition & Anomaly Detection** – Shell companies, money laundering, identity fraud.
6. **Central Knowledge Graph** – Neo4j with interactive graph visualization.
7. **Investigation Dashboard** – Gradio/FastAPI frontend with PDF report generation.

```bash
# Clone the repository
git clone https://github.com/surendragrover/InvestigatorAI.git
cd InvestigatorAI

# Create virtual environment (optional)
python -m venv venv
source venv/bin/activate  # Linux/Mac
# or .\venv\Scripts\activate (Windows)

# Install dependencies
pip install -r requirements.txt
