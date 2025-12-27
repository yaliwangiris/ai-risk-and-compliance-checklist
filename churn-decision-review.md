# AI-Assisted Churn Prediction — Business Decision Review

This example illustrates how the **AI Risk & Decision Review framework** is applied in a realistic business scenario.

The focus is not on model accuracy, but on **decision design, risk awareness, and governance**.

---

## Business Context

A subscription-based digital service is experiencing increased customer churn among mid-tier users.

The business team proposes using an AI model to **identify high-risk customers** and prioritize retention offers.

---

## Decision Definition

**Business decision:**  
Whether to offer a retention incentive to a customer.

**Decision owner:**  
Growth / Retention Manager.

**AI role:**  
Provide a **risk score** to help prioritize customers for review.

**Key design choice:**  
The AI system is **advisory**, not autonomous.  
Final decisions remain with the business team.

---

## Non-AI Baseline

Before AI deployment, the company relied on:
- Rule-based targeting (e.g., inactivity thresholds)
- Broad discount campaigns
- Limited personalization and high cost

This baseline is used as a comparison point for evaluating AI value.

---

## Risk Review (Business Perspective)

### Financial Risk
- False positives may lead to unnecessary discounts
- False negatives may result in lost customers
- Conservative thresholds are used initially

### Customer Risk
- Customers are not informed of individual risk scores
- No automated denial of service or access
- Human review remains available for edge cases

---

## Model Use and Limits

It is explicitly documented that:
- The model predicts **likelihood**, not intent
- Predictions do not explain *why* churn occurs
- Outputs degrade as customer behavior changes

The model is used for **ranking**, not for deterministic decisions.

---

## Go / No-Go Decision

**Outcome:**  
Go with constraints.

**Constraints include:**
- Human approval required for all campaign rules
- No fully automated customer-level actions
- Mandatory post-launch review after 30 days

---

## Post-Deployment Review Plan

The business team commits to reviewing:
- Churn rate changes
- Retention campaign ROI
- Evidence of over-reliance on AI outputs

If benefits are unclear or risks increase, AI usage will be paused or revised.

---

## Why This Example Matters

This case demonstrates:
- Decision-first AI deployment
- Explicit risk acknowledgment
- Human accountability by design
- Practical use of AI without over-automation

