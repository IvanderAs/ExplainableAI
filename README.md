Robustness and Reliability of Interpretable Machine Learning for Anti-Money Laundering (AML) Systems
A dual-perspective Explainable Artificial Intelligence (XAI) framework designed for financial technology and banking security. This repository implements an end-to-end pipeline that combines synthetic data balancing with global and local interpretability models to resolve the black-box transparency crisis in automated Anti-Money Laundering (AML) and fraud detection systems[cite: 2].

Overview
Automated fraud detection systems often utilize complex machine learning models that excel at predictive accuracy but lack transparency[cite: 2]. In modern financial compliance, a high true-positive rate is insufficient if security analysts and auditors cannot audit why a specific transaction was flagged[cite: 2].

This project provides:
Class Imbalance Handling: Utilizes SMOTE (Synthetic Minority Over-sampling Technique) to synthesize minority fraud cases, ensuring robust training against heavily skewed financial datasets[cite: 2].
Local Diagnostics: Employs LIME (Local Interpretable Model-agnostic Explanations) for real-time, transaction-level feature attribution, giving analysts instant visibility into high-risk indicators[cite: 2].
Global Validation: Integrates SHAP (SHapley Additive exPlanations) to validate overall model behavior across the dataset, ensuring alignment with regulatory compliance and policy standards[cite: 2].

[ Financial Data ]
          │
          ▼
   [ Preprocessing ]  ──► (SMOTE Imbalance Correction)
          │
          ▼
   [ ML Fraud Model ]
          │
   ┌──────┴──────────────────────────┐
   │                                 │
   ▼                                 ▼
[ LIME Explainer ]           [ SHAP Explainer ]
 (Transaction Level)           (Global Policy)
   │                                 │
   ▼                                 ▼
 Real-time Analyst Alerts     Regulatory Audit Trail

Key Features
Dual-Perspective Interpretability:

Local (LIME): Instant explanation vectors for single-transaction audits[cite: 2].

Global (SHAP): Game-theoretic feature contribution analysis across all data samples[cite: 2].

Imbalance Mitigation: Integrated SMOTE pipeline to prevent model bias towards non-fraudulent instances[cite: 2].

Regulatory-Ready: Designed to support auditability requirements under modern fintech governance frameworks[cite: 2].

