# 🏛️ Civic-AurAI

Welcome to the **Civic-AurAI** GitHub Organization! 

We are building a next-generation, high-trust civic dispatch and reporting ecosystem. By combining crowdsourced mobile video intelligence with advanced AI vision analysis and scalable databases, Civic-AurAI empowers cities and citizens to automatically detect, report, and verify civic hazards in real time.

---

## 🚀 Our Repositories

Here's an overview of the core services, apps, and pipelines that make up the Civic-AurAI ecosystem:

### 1. [CivicAurAI](https://github.com/Civic-AurAI/CivicAurAI) (Core Engine & Web Portal)
The backbone data processing pipeline and primary citizen-facing web portal.
- **Semantic Engine:** Ingests video chunks and uses Gemini Vision to detect and classify street-level hazards.
- **Spanner Database:** Utilizes Google Cloud Spanner seamlessly blending relational state tracking with complex Property Graphs to link users, reports, videos, and organizations.
- **High-Trust Portal:** A Vite/React web frontend integrated with a FastAPI backend that merges our proprietary locally-detected AI issues alongside public municipal data (e.g., SF311 API) into one unified dispatch dashboard.

### 2. [CivicAurAIRecorder](https://github.com/Civic-AurAI/CivicAurAIRecorder) (Mobile App)
The mobile frontend for civic data collection. 
- A secure, privacy-first mobile application that allows citizens to record their environment. It captures video arrays and device telemetry (GPS, heading) while stripping unnecessary metadata to protect reporter anonymity before passing data up to our extraction pipeline.

### 3. [Final_Code](https://github.com/Civic-AurAI/Final_Code)
An alternative and parallel implementation of the CivicAurAI backend pipeline and backbone.
- Built by our teammate during the core development phases, this repository contains similar architectural approaches for the AI integration, telemetry parsing, and semantic processing pipeline. It mirrors the core functionality of the standard CivicAurAI backend.

### 4. RocketRide (Fork) - *In Development*
A specialized server fork slated for our future scalable infrastructure.
- We are adapting this fork to act as a high-performance routing and orchestration layer. It will eventually house our custom processing components—such as advanced **Gemini vector embeddings** for semantic similarity search—enabling deduplication of civic issues based on visual and textual vector proximity.

---

## 🛠️ Technology Stack
- **AI / ML:** Google Gemini (Vision & Embeddings)
- **Database:** Google Cloud Spanner (Relational + Graph Database)
- **Backend:** Python, FastAPI
- **Frontend:** React, Vite, TypeScript
- **Mobile:** Flutter / Dart (Recorder App)
- **Cloud Infrastructure:** Google Cloud Storage (GCS), GCP
- **RocketRide:** Prototyping agentic ingestion pipelines

---

*(This [README.md](cci:7://file:///home/csaba/repos/AIML/CivicAurAI/CivicAurAI/README.md:0:0-0:0) is designed to be placed inside a `.github` repository to serve as the landing page for the Civic-AurAI organization!)*
