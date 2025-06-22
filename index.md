---
layout: default
title: Overview
permalink: /
---

# Transaction Monitoring Portfolio

Welcome to the **Transaction Monitoring Portfolio**—a showcase of how we detect, analyze and visualize suspicious transaction patterns using rule-based “indicators.”

## 1. Background & Business Case  
- **Problem:** Bank X must comply with AML/CTF regulations. We’ve implemented multiple detection rules, each producing an “Indicator” file (e.g. unusual foreign transfers, off-hour payments).  
- **Value:** For large institutions producing dozens of alert categories—each generating hundreds of thousands of transactions—manual review quickly becomes infeasible. This approach automatically consolidates and deduplicates these massive alert streams into a concise, high-quality set of signals, enabling analysts to focus on true positives, dramatically reducing false alarms, and ensuring robust regulatory compliance.

## 2. Insights & Impact  
- **Key Discoveries:**  
  - Which rules overlap most (high duplication rate)?  
  - How many alerts are merely repeats of the same transaction?  
  - Which rules generate the highest share of unique alerts?  
- **Potential Impact:**  
  - Deduplication ROI: up to **30% less manual review**, faster identification of true positives.

## 3. Data & Visuals to Tell the Story  
- **Dashboard Overview:**  
  - Bar chart: alerts per rule vs. % duplicated  
  - Heatmap: pairwise duplication correlation  
- **Time Series:** alert volume over time to spot anomalies  
- **Sankey / Network Graph:** flow of unique→duplicate alerts across rules  
- **Interactivity:** built with Plotly Dash (or Power BI) to filter by rule, time window, transaction type  

## 4. Technical Details

For deeper dives into the implementation, see:

- [Architecture & Code]({{ site.baseurl }}/architecture/)  
- [Scalability & Performance]({{ site.baseurl }}/scalability/)  
- [Automation & CI/CD]({{ site.baseurl }}/automation/)  
- [Testing]({{ site.baseurl }}/testing/)  

---
