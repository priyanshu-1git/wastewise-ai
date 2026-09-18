# ♻️ WasteWise AI

### AI-Powered Perishable Inventory Waste Prevention System

> A prototype decision-support system that combines **AI demand forecasting**, **shelf-life analysis**, and **inventory risk reasoning** to identify potential perishable inventory surplus before expiry.

[![Python](https://img.shields.io/badge/Python-3.x-blue)](https://www.python.org/)
[![Streamlit](https://img.shields.io/badge/Streamlit-App-red)](https://streamlit.io/)
[![Machine Learning](https://img.shields.io/badge/ML-Random%20Forest-green)](https://scikit-learn.org/)
[![SDG 12](https://img.shields.io/badge/SDG-12%20Responsible%20Consumption-orange)](https://sdgs.un.org/goals/goal12)

---

## 🚀 Live Prototype

**WasteWise AI is designed as an interactive Streamlit prototype.**

🔗 **Live Demo:**  
[Open WasteWise AI](https://wastewise-ai-app.streamlit.app/)

> ✅ The prototype is deployed on Streamlit Community Cloud and is available for interactive demonstration.

---

## 📌 Table of Contents

- [Problem](#-problem)
- [Solution](#-solution)
- [How It Works](#-how-it-works)
- [AI Component](#-ai-component)
- [Decision Logic](#-decision-logic)
- [Prototype Dashboard](#-prototype-dashboard)
- [Example](#-example)
- [Technology Stack](#-technology-stack)
- [Dataset](#-dataset)
- [Responsible AI](#-responsible-ai)
- [Project Scope](#-project-scope)
- [Repository Structure](#-repository-structure)
- [Future Improvements](#-future-improvements)
- [SDG Alignment](#-sdg-alignment)

---

## 🌍 Problem

Perishable products such as milk, yogurt, ready meals and other food products have a limited shelf life.

When inventory exceeds the quantity likely to be sold before expiry, products can become potential waste.

Traditional inventory monitoring may show:

- Current stock
- Historical sales
- Reorder levels

But it may not clearly answer:

> **"How much of this inventory is likely to remain unsold before expiry?"**

WasteWise AI addresses this decision-support problem by combining demand forecasting with remaining shelf-life information.

---

## 💡 Solution

WasteWise AI follows a simple decision pipeline:

```mermaid
flowchart LR

A[Historical Sales] --> B[AI Demand Forecast]

B --> C[Expected Sales During Remaining Shelf Life]

D[Inventory] --> E[Potential Surplus]
F[Remaining Shelf Life] --> C

C --> E

E --> G[Waste Risk Assessment]

G --> H[Recommended Intervention]

H --> I[Human Inventory Manager]
