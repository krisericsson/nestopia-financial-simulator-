🗓️ June 6, 2025 – Sprint #1 – Core Simulator Engine
✅ What Was Completed
• Built initial financial simulator with user input
• Added growth rate and user count logic
• Connected four revenue channels: ID Verification, Subscriptions, Affiliates, Landlords (consolidated in totalRevenue)
• Displayed revenue and user metrics for Month 1, Month 60, and cumulative

🛠️ Technical Details
• Simulator coded in vanilla JS + HTML
• Revenue logic fully driven by user count and phased monetisation
• Handled affiliate percentage growth shift after Month 18
• Added toggle for data view (monthly/cumulative)

💭 Reasoning & Notes
• This sprint focused on validating the simulation engine against our FS Model
• Accuracy was checked against model screenshots and founder expectations
• Ensured code is clean, understandable, and ready for scaling in Sprint 2

📈 Next Steps
• Add salary cost logic and EBITDA tracking
• Enable Predicted vs Actual toggle with input override
• Begin runway, gross margin, and LTV/CAC tracking

✅ Sprint 2 – Revenue & Cost Engine
Date: June 6, 2025
Status: ✅ Completed
Lead: Kris Ericsson
Sprint Type: Functional + UI
Files Affected: script.js, index.html, style.css

🔧 What Was Built
• Salary Engine: Foundational logic added to calculate dynamic salary costs per employee across 60 months.
• NI + Pension Contributions: Employer National Insurance (15%) and Pension (3%) accurately calculated and applied.
• Founders as Initial Roles: Only Kris & Matt are included in the cost logic by default — all other roles can be added in future sprints.
• Monthly EBITDA: Now calculated live by subtracting salary + contributions from total revenue.
• Total Cost Breakdown: Backend logic in place, front-end visualisation deferred to Sprint 3.

🧪 Notes
• Actual OPEX (e.g., marketing, rent, SaaS, accounting) implemented in Sprint 3.
• Visual layout improved but styling refinements handled in Sprint 6.

✅ Sprint 3 – Cost Section & EBITDA
Date Completed: June 7, 2025
Lead: Kris Ericsson
Status: ✅ Complete
Sprint Goals:
• Add clean cost section below revenue
• Introduce logic for operating costs
• Ensure EBITDA line updates based on salaries and total cost assumptions
• Update output layout to clearly separate Revenue and Costs

What Was Done:
• Created architecture for the cost section using clean, stackable HTML blocks
• Added total salaries logic, including Employer NI and Pension
• Built logic for total operating costs using validated monthly data
• Introduced visual EBITDA output beneath all costs
• Cleaned up output layout for clarity between Revenue and Cost sections

✅ Sprint 4 – Data Extraction + Validation
Status: ✅ Complete
Date: June 7, 2025
Lead: Atlas (with Gemini escalation)
Objectives:
• Extract and validate all user, revenue, and cost data from the FS spreadsheet
• Manually input 17 cost lines and 60-month arrays where necessary
• Resolve parsing and NaN errors that blocked simulator output

Outcomes:
• Full dataset (users[], totalRevenue[], totalOperatingCosts[], ebitda[]) confirmed line-by-line
• Final dataset structured in clean JSON format for injection into the simulator
• Gemini onboarded to support code stability, error-handling, and file debugging

✅ Sprint 5 – Financial Engine Implementation
Status: ✅ Complete
Date: June 7, 2025
Lead: Gemini (execution), Atlas (oversight)
Objectives:
• Rebuild the simulator’s financial engine using validated data
• Ensure accurate rendering of monthly figures in dropdown and output
• Repair UI rendering, dropdown logic, and module imports

Outcomes:
• Simulator now dynamically renders all 60 months with correct values
• Total Revenue, Operating Costs, and EBITDA are all live, formatted, and test-validated
• Recovered from broken state to fully working interface via Gemini's intervention
• All hardcoded errors, parser bugs, and UI blockers resolved

✅ Sprint 6 – UI & Layout Upgrade
Date: June 8, 2025
Lead: Atlas (validated by Gemini)
Status: ✅ Complete

What Was Built:
• Rebuilt the simulator interface with a clean two-column layout
• Styled financial output as card components with responsive design
• Applied Nestopia brand colors: #FA5926 (primary), #000045 (secondary)
• Implemented mobile responsiveness via Flexbox and media queries
• Added Nestopia logo (25% scale, aligned above title)
• Fixed encoding bugs with currency formatting
• Ensured all files (HTML, CSS, JS, logo) are integrated and validated

Outcome:
• The simulator now feels visually professional and investor-ready
• Clear structure prepares us for scenario toggles, growth curves, and AI chat in future sprints

✅ Sprint 7 – Growth Scenario Toggle
Date: June 8, 2025
Lead: Atlas (validated by Gemini)
Status: ✅ Complete

What Was Built:
• Added scenario dropdown: Baseline, Conservative, Aggressive, Custom Input
• Created growthProfiles.js with 60-month data arrays
• Connected growth toggle to users[] dynamically
• Ensured revenue/EBITDA output updates with each toggle
• Added display explainer beneath scenario selector
• Preserved selected month during scenario switching

Outcome:
• Investors can now toggle different growth strategies and instantly see the impact
• Prepared structure for future GPT chat interface and scenario insights

✅ Final Sprint 8 Closure Summary – Revenue Breakdown View

🗓️ Date: June 8, 2025
Status: ✅ Completed
Lead: Atlas (code) + Gemini (validation)

⸻

🎯 Sprint Objectives
	•	Show diversification of revenue streams
	•	Display monthly + cumulative values
	•	Provide clarity on how each revenue source activates
	•	Improve investor understanding of financial drivers

⸻

🚀 What We Built
	•	Clean two-column layout for revenue data
	•	Monthly breakdown: ID Verification, Subscription, Affiliate, Landlord
	•	Cumulative totals auto-calculate once for maximum performance
	•	Descriptive notes using <small> tags for clarity
	•	Responsive and readable design validated for investors

⸻

🧠 Why It Matters

This sprint closes the loop on the financial engine.
For the first time, investors can see how revenue is earned and scales across all sources, not just lumped together. This brings clarity, confidence, and data transparency.

🧠 Sprint 9 – GPT-Integrated FS Chat Assistant
Mission: Let investors "talk" to the model using natural language prompts
Capabilities:
• Query summary: “Summarise Month 24”
• Explain logic: “How is EBITDA calculated?”
• Impact analysis: “What happens if growth slows to 5% MoM?”
• Compare: “How does Conservative differ from Aggressive?”
• Export answers as PDF
• Optional voice prompt UI

🌀 Sprint 10 – Timeline Scroll + Month Deltas
Mission: Improve UX for time period navigation and add comparison insights
Deliverables:
• Replace month dropdown with horizontal scrollable timeline (Month 1–60)
• Highlight selected month
• Display comparison to previous month (delta values)
• Optional: chart view of key metrics over time

🟢 Sprint 11 – Investor-Ready UX Polish

Status: Pending
Lead: Atlas (execution) + Kris (creative direction)
Timing: Post-core feature completion (after Sprint 10)

⸻

🎯 Objective

Make the simulator feel like a seamless extension of the Nestopia brand. This sprint transforms it from functional prototype to high-conviction investor tool — clean, credible, and product-ready.

⸻

🧱 What We’ll Build
	•	✅ Apply Nestopia fonts, spacing, and layout rules to match main product and site
	•	✅ Use real UI components from Figma (where available)
	•	✅ Adjust color contrasts, padding, and button states for polish
	•	✅ Add subtle animations or hover effects for modern touch
	•	✅ Consider mobile/tablet view refinements
	•	✅ Fix all alignment, overflow, and spacing quirks
	•	✅ Clean up or hide dev/debug toggles unless needed

⸻

💡 Optional Additions
	•	Mini tutorial overlay for first-time users
	•	Tooltip icons with “what does this mean?” next to financial terms
	•	Export or screenshot button
	•	Light/dark mode toggle (stretch goal)

⸻

🧠 Why This Matters

Investors judge not just the data, but the presentation. This final layer builds trust, reinforces brand, and positions Nestopia as serious and capable.
