# 📊 Expense-Tracker Dashboard — Mini PRD

| **Meta**             | |
|----------------------|--------------------------------------|
| **Owner**            | Anushka Mishra |
| **Doc version**      | v1.0 — 12 May 2025 |
| **Status**           | Draft — feedback welcome |
| **Target MVP date**  | 31 May 2025 |

---

## 1 · Problem / Opportunity
Gen-Z users juggle 7–10 subscriptions plus UPI/card spends. They **cannot answer “Where did my ₹ go?”** without pivot tables or paid apps.

## 2 · Goal
Ship a lightweight **web dashboard** that ingests bank CSVs & UPI SMS, auto-categorises spends, and surfaces:

* Top 5 categories (pie)  
* Subscription renewals next 7 days (alert bar)  
* 30-day cash-flow trend (line)

### Success KPIs

| KPI                           | Target |
|-------------------------------|--------|
| Weekly Active Users           | 500    |
| CSV → Dashboard completion    | 70 %   |
| Subscription renewals caught  | 200    |

## 3 · Personas
* **Ria (24)** — PM intern tracking salary vs. lifestyle spends  
* **Karan (30)** — Freelancer needing GST filter & export

## 4 · User Stories (MoSCoW)

| Priority | Story                                       |
|----------|---------------------------------------------|
| **Must** | Upload bank CSV → see instant charts        |
| **Must** | View upcoming subscription bills            |
| **Should**| Tag a spend as “tax-deductible”            |
| **Could**| Toggle dark mode                            |
| **Won’t**| Export monthly PDF (v2)                     |

## 5 · MVP Scope
* Local SQLite `warehouse.db`  
* CSV ingest only (no live bank auth)  
* React + Chart.js front-end, FastAPI back-end  

## 6 · Risks & Mitigations

| Risk                   | Mitigation                           |
|------------------------|--------------------------------------|
| Bad CSV headers        | Provide sample + header-map UI       |
| Ambiguous categories   | Manual re-tag; ML in v2              |
| Privacy concerns       | All processing local; no cloud upload|

## 7 · Timeline / Next Steps
1. ✅ Scaffold repo — 12 May  
2. 🏗️ Build CSV ingest — 18 May  
3. 🎨 Ship dashboards — 26 May  
4. 📢 Post demo on LinkedIn — 31 May  

> _“Track your money like a PM tracks KPIs.”_
