## 🗓️ June 6, 2025 – Sprint #1 – Core Simulator Engine

### ✅ What Was Completed
- Built initial financial simulator with user input
- Added growth rate and user count logic
- Connected four revenue channels: ID Verification, Subscriptions, Affiliates, Landlords
- Displayed revenue and user metrics for Month 1, Month 60, and cumulative

### 🛠️ Technical Details
- Simulator coded in vanilla JS + HTML
- Revenue logic fully driven by user count and phased monetisation
- Handled affiliate percentage growth shift after Month 18
- Added toggle for data view (monthly/cumulative)

### 💭 Reasoning & Notes
- This sprint focused on validating the simulation engine against our FS Model
- Accuracy was checked against model screenshots and founder expectations
- Ensured code is clean, understandable, and ready for scaling in Sprint 2

### 📈 Next Steps
- Add salary cost logic and EBITDA tracking
- Enable Predicted vs Actual toggle with input override
- Begin runway, gross margin, and LTV/CAC tracking



---

### ✅ Sprint 2 – Revenue & Cost Engine

**Date:** June 6, 2025  
**Status:** ✅ Completed  
**Lead:** Kris Ericsson  
**Sprint Type:** Functional + UI  
**Files Affected:** `script.js`, `index.html`, `style.css`

---

#### 🔧 What We Built

- 🧠 **Salary Engine**: Foundational logic added to calculate dynamic salary costs per employee across 60 months.
- 💸 **NI + Pension Contributions**: Employer National Insurance (15%) and Pension (3%) accurately calculated and applied.
- 💾 **Founders as Initial Roles**: Only Kris & Matt are included in the cost logic by default — all other roles can be added in future sprints.
- 🧾 **Monthly EBITDA**: Now calculated live by subtracting salary + contributions from total revenue.
- 🧮 **Total Cost Breakdown** (backend logic in place, front-end visualisation deferred to Sprint 3).

---

#### 🧪 Notes

- Actual OPEX (e.g., marketing, rent, SaaS, accounting) will be implemented in **Sprint 3**.
- Visual layout improved but styling refinements (alignment, spacing) will be handled separately.

---
