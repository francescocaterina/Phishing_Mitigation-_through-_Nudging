# 🛡️ SecureMail: Phishing Mitigation Through Nudging

## 📌 Project Overview
This repository contains the evaluation and analysis of **SecureMail**, a simulated email environment designed to test the effectiveness of **nudging and visual friction** in preventing phishing attacks.

Modern cybersecurity directives (such as NIS2) require strict policies, but human limitations — like cognitive fatigue, biases, and habits — often render them ineffective. This project explores a paradigm shift: modifying the choice architecture of an interface to intuitively guide users toward safer decisions without restricting their options.

## 🔬 Study Design and Methodology
We conducted a rigorous **A/B test with a within-subjects design** on a sample of 12 non-expert participants. To prevent learning bias (order effect), we applied a strict counterbalancing protocol with sealed envelopes.

The study evaluated user behavior during a critical task (identifying a phishing email, Task 3) under two different conditions:
*   **Condition A (Original):** A standard gray warning banner, easily ignorable.
*   **Condition B (Mitigated):** A red security banner, highly salient and with high visual friction, featuring critical warning text and no quick close button.

### Collected Metrics
*   Task Failure Rate (Phishing susceptibility)
*   Task Completion Time (TCT)
*   Observation of Impulsiveness and Frustration
*   **NASA-TLX** (Cognitive Workload)
*   **SUS** (System Usability Scale)

## 📊 Key Findings: The Security-Usability Trade-off
The implementation of visual friction (Condition B) proved highly effective for security, but introduced a significant usability trade-off:

| Metric | Cond. A (Gray Banner) | Cond. B (Red Banner) | Impact |
| :--- | :--- | :--- | :--- |
| **Failure Rate** | 83.3% | **16.7%** | ✅ Massive security improvement |
| **Impulsiveness** | 50.0% | 33.3% | ✅ Better decision processing |
| **Avg. Time (TCT)** | 43.58 s | 67.83 s | ⚠️ Increased execution time |
| **Frustration Rate** | 8.3% | 58.3% | ❌ Higher user stress |
| **SUS Score** | 84.79 (Excellent) | 63.12 (Insufficient) | ❌ Usability drop |
