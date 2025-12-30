# CSC172 Association Rule Mining Project Progress Report
**Student:** Kaycee T. Nalzaro, 2021-1756  
**Date:** December 16, 2025
**Repository:** [https://github.com/kyrr0o/CSC172-AssociationMining-Nalzaro.git](https://github.com/kyrr0o/CSC172-AssociationMining-Nalzaro.git)  

## Current Status

| Milestone | Status | Notes |
|-----------|--------|-------|
| Problem Definition | Completed | Drainage clogging modeled as symbolic condition patterns |
| Synthetic Dataset Design | Completed | Rule-based drainage scenarios defined |
| Synthetic Data Generation | In Progress | Partial dataset generated, rules being refined |
| Transaction Encoding | In Progress | Item vocabulary finalized, encoding ongoing |
| Association Rule Mining | Pending | Will start after dataset finalization |
| Rule Evaluation & Analysis | Not Started | Planned after ARM execution |

## 1. Dataset Progress
- **Dataset type:** Synthetic transactional dataset
- **Target size:** 100 drainage observations
- **Current size:** ~50 generated transactions
- **Item categories implemented:**
  - Trash conditions (e.g., heavy_trash, plastic_trash, organic_trash)
  - Flow behavior (e.g., slow_flow, stagnant_flow, backflow)
  - Visual water cues (e.g., dark_water, foam_present)
  - Drainage states (clean, partially_clogged, clogged)
- **Generation approach:** Rule-based synthetic generation using DrainSight domain knowledge
- **Encoding status:** Transaction list format prepared; one-hot encoding in progress

## 2. Association Rule Mining Progress

**Current Stage:**
- Apriori parameters identified (minimum support and confidence)
- Transaction encoding pipeline partially implemented
- Rule filtering logic (drainage state as consequent) designed but not yet executed

**Planned Metrics:**
- Support
- Confidence
- Lift

**Status:**  
Association rule mining will be executed once the full synthetic dataset is completed and validated.

## 3. Challenges Encountered & Solutions

| Issue | Status | Resolution |
|------|--------|------------|
| Designing realistic drainage scenarios | Ongoing | Refining rule-based generation using domain assumptions |
| Limited realism of synthetic data | Acknowledged | Clearly documented as a limitation |
| Overlapping condition rules | In Progress | Manual validation of generated transactions |
| Rule explosion risk | Planned | Apply strict support, confidence, and lift thresholds |

## 4. Next Steps (Before Final Submission)
- [ ] Complete synthetic dataset generation (remaining transactions)
- [ ] Finalize transaction encoding and validation
- [ ] Run Apriori algorithm for frequent itemset mining
- [ ] Generate and filter association rules
- [ ] Analyze rule quality using support, confidence, and lift
- [ ] Update README.md with final results and rule interpretations
