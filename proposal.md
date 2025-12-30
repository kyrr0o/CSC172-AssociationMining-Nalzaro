# CSC172 Association Rule Mining Project Proposal
**Student:** Kaycee T. Nalzaro, 2021-1756  
**Date:** December 12, 2025

## 1. Project Title
Association Rule Mining of Urban Drainage Conditions for Clogging Detection

## 2. Problem Statement
Urban drainage systems frequently experience clogging due to waste accumulation, stagnant water, and abnormal flow behavior, 
leading to flooding, sanitation issues, and infrastructure damage. While monitoring systems such as DrainSight can detect visual 
and flow-related drainage conditions, translating these observations into clear and interpretable decision logic remains challenging. 
Without explainable rules, maintenance decisions often rely on manual inspection and subjective judgment. This project addresses this 
gap by applying Association Rule Mining to discover interpretable patterns that indicate drainage clogging conditions, supporting 
data-driven and explainable maintenance decisions.

## 3. Objectives
- Discover frequent patterns and associations among drainage conditions using Association Rule Mining
- Identify interpretable rules that indicate clean, partially clogged, and clogged drainage states
- Provide explainable decision-support logic that complements DrainSight’s detection outputs

## 4. Dataset Plan
- **Source:** Synthetic drainage dataset generated using DrainSight domain knowledge  
- **Expected Size:** 100 transactional records  
- **Item Categories / Classes:**
  - Trash conditions (e.g., heavy_trash, plastic_trash, organic_trash)
  - Flow behavior (e.g., stagnant_flow, slow_flow, backflow)
  - Visual water cues (e.g., dark_water, foam_present)
  - Drainage state labels (clean, partially_clogged, clogged)
- **Acquisition:** Programmatically generated synthetic transactions based on rule-based drainage scenarios

## 5. Technical Approach
- **Architecture Sketch:** Transactional data mining pipeline using symbolic drainage observations
- **Algorithm:** Apriori Association Rule Mining
- **Framework & Tools:** Python, pandas, mlxtend
- **Process:**
  - Transaction encoding using one-hot representation
  - Frequent itemset extraction using Apriori
  - Association rule generation and filtering based on confidence and lift
- **Hardware:** Local machine (CPU-based execution)

## 6. Expected Challenges & Mitigations
- **Challenge:** Dataset is synthetic and may not fully represent real-world drainage complexity  
  **Solution:** Use domain knowledge-based rules and clearly state limitations in analysis

- **Challenge:** Overgeneration of weak or redundant rules  
  **Solution:** Apply minimum support, confidence, and lift thresholds and retain only state-predictive rules

- **Challenge:** Limited generalization capability  
  **Solution:** Position results as explainable decision support rather than predictive modeling
