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
✅ Sprint 3 – Complete: Cost Section & EBITDA

Sprint Goals:
	•	Add clean cost section below revenue
	•	Introduce placeholder logic for operating costs
	•	Ensure EBITDA line updates based on salaries and total cost assumptions
	•	Update output layout to clearly separate Revenue and Costs

What Was Done:
	•	Created architecture for the cost section using clean, stackable HTML blocks
	•	Added total salaries logic, including Employer NI and Pension
	•	Built early logic for total operating costs using placeholder values
	•	Introduced visual EBITDA output beneath all costs
	•	Cleaned up output layout for clarity between Revenue and Cost sections

Pending/Deferred:
	•	Monthly cost breakdowns per category (from FS model)
	•	Dynamic user and revenue source activation logic
	•	Dropdown toggles for category-level cost visibility (planned for Sprint 4)

Date Completed: Saturday, 7 June 2025
Owner: Kris Ericsson
Status: ✅ Complete
Next Sprint: Sprint 4 – Operating Cost Breakdown & Revenue Channel Activation

## ✅ Sprint 4 – Data Extraction + Validation  
**Status:** Complete  
**Date:** 7 June 2025  
**Lead:** Atlas (with Gemini escalation)

### Objectives:
- Extract and validate all user, revenue, and cost data from the master FS spreadsheet  
- Manually input 17 cost lines and 60-month arrays where necessary  
- Resolve parsing and NaN errors that blocked simulator output

### Outcomes:
- Full dataset (`users[]`, `totalRevenue[]`, `totalOperatingCosts[]`, `ebitda[]`) confirmed line-by-line  
- Final dataset structured in clean JSON format for injection into the simulator  
- Gemini onboarded to support code stability, error-handling, and file debugging  
---

## ✅ Sprint 5 – Financial Engine Implementation  
**Status:** Complete  
**Date:** 7 June 2025  
**Lead:** Gemini (execution), Atlas (oversight)

### Objectives:
- Rebuild the simulator’s financial engine using validated data  
- Ensure accurate rendering of monthly figures in dropdown and output  
- Repair UI rendering, dropdown logic, and module imports

### Outcomes:
- Simulator now dynamically renders all 60 months with correct values  
- Total Revenue, Operating Costs, and EBITDA are all live, formatted, and test-validated  
- Recovered from broken state to fully working interface via Gemini's intervention  
- All hardcoded errors, parser bugs, and UI blockers resolved  

✅ Sprint 6 – UI & Layout Upgrade
	•	Status: Completed
	•	Date: 8 June 2025
	•	Lead: Atlas (validated by Gemini)

What was built:
	•	Rebuilt the simulator interface with a clean two-column layout
	•	Styled financial output as card components with responsive design
	•	Applied Nestopia brand colors: #FA5926 (primary), #000045 (secondary)
	•	Implemented mobile responsiveness via Flexbox and media queries
	•	Added Nestopia logo (25% scale, aligned above title)
	•	Fixed encoding bugs with currency formatting
	•	Ensured all files (HTML, CSS, JS, logo) are integrated and validated
	•	Gemini validated all front-end components and JS logic

Outcome:
	•	The simulator now feels visually professional and investor-ready
	•	Clear structure prepares us for scenario toggles, growth curves, and AI chat in Sprints 7–9
