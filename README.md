 Nestopia Financial Simulator

A lightweight, interactive browser-based tool designed to simulate Nestopia’s 60-month financial model with editable assumptions and live outputs. Built by Kris Ericsson (Founder), Atlas (AI Co-Pilot), and Gemini (Financial Integrity Engine).

🚀 Project Summary

This simulator allows investors and internal stakeholders to explore Nestopia’s financials across key metrics:
	•	Monthly user growth
	•	Revenue (4 streams)
	•	Operating costs (17 line items)
	•	EBITDA (monthly)
	•	Live month-by-month analysis via dropdown

All values are sourced directly from the validated FS model, ensuring precision and clarity.

✅ Sprint Log

Sprint 1:
	•	Built foundational layout (HTML/CSS structure)
	•	Introduced month selection logic and static output box

Sprint 2:
	•	Constructed salary engine with NI and pension logic
	•	Enabled EBITDA calculation based on dynamic roles

Sprint 3:
	•	Added backend engine for operating costs (17 lines)
	•	Wired output logic to pull from all cost categories

Sprint 4:
	•	Hardwired user growth, revenue, and cost arrays based on validated FS model
	•	Added all 60 months of simulator logic

Sprint 5:
	•	Gemini joined as integrity layer to validate FS data
	•	Final dataset confirmed from Excel sheets
	•	Full integration of users, revenue, costs, and EBITDA
	•	Simulator now functioning end-to-end with correct monthly outputs

🛠 Setup Instructions

To run the simulator locally:
	1.	Clone or download the repo
	2.	Make sure the following files are in the same directory:
	•	index.html
	•	script.js
	•	data.js
	3.	Open index.html in your browser (double click or right-click > Open With > Chrome/Safari/etc.)

⚠️ If you move any files into subfolders, update the <script> path in index.html accordingly.

📁 File Structure

/Nestopia-Financial-Simulator/
├── index.html         – Main UI
├── script.js          – Rendering logic
└── data.js            – Financial dataset (users, revenue, costs, EBITDA)

👥 Contributors
	•	Kris Ericsson – Founder & Product Lead
	•	Atlas – AI Strategist & Technical Lead
	•	Gemini – Financial Validation & Model Integrity

---
