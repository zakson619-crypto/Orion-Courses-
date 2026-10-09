# TOPIC 7 — ASSESSMENT
Capstone: AI-Powered Business Automation & Decision Systems
Comprehensive Implementation Guide, Technical Exercises &
Assessment Criteria
## 1. Assessment Overview
This assessment evaluates your ability to integrate advanced prompt engineering frameworks (CO-
STAR, Meta-Prompting, and Quantitative Graph of Thoughts) to build a virtual CRM vendor decision
agent, produce a weighted decision matrix, generate a phased implementation roadmap, compile a
business proposal and executive presentation, write a lessons learned report, and deliver all project
files via a public GitHub repository with a Loom video walkthrough. The assessment is based on the
provided Requirement Document and Implementation Plan.
## 2. Assessment Objective
Demonstrate your ability to complete a full capstone prompt engineering workflow that follows
course best practices. The solution should include:
- Establishing the Apex Cloud Services enterprise case study scenario for CRM vendor
evaluation.
- Using Meta-Prompting to generate a specialized CRM research prompt.
- Executing a CO-STAR + Q-GoT vendor evaluation comparing Salesforce, HubSpot, and Zoho
with verified TCO calculations.
- Building a Weighted Cost-Benefit Decision Matrix scored against four criteria.
- Generating a phased 6-month Gantt roadmap and a risk registry.
- Writing a B2B business proposal and a 6-slide executive presentation.
- Compiling a lessons learned post-mortem report covering LLM limitations.
- Recording a Loom video walkthrough demonstrating the live capstone system.
- Publishing all deliverables to a public GitHub repository.
## 3. Prerequisites
- Review the Requirement Document before starting the project.
- Review the Implementation Plan for the step-by-step setup and configuration flow.
- Have access to a web browser and a stable internet connection.
- Have completed Lessons 1 through 6 of the Prompt Engineering course.
- Have a free OpenAI account to access ChatGPT.
- Have a free GitHub account ready to create a public repository.
- Have a free Loom account (or any screen recorder) ready to record your video walkthrough.
- Prepare a local folder on your computer named prompt-engineering-capstone to organize your
deliverables.

## 4. Assessment Tasks & Answers
### Exercise 1 — Select the Enterprise Case Study Scenario
Task: Establish your enterprise parameters in ChatGPT by defining the Apex Cloud Services CRM
migration scenario, including user count, current state, and vendor financial metrics for Salesforce,
HubSpot, and Zoho.
Answer — Setup Steps:
- Open your browser and navigate to https://chatgpt.com/. Log in and click New Chat to clear the
conversation window.
- Define the scenario: Apex Cloud Services is migrating 150 active sales representatives, currently
tracking client data in offline spreadsheets with high data fragmentation (REQ-002).
- Record the financial metrics for each vendor: Salesforce ($150/user/mo + $25k setup), HubSpot
($90/user/mo + $10k setup), Zoho ($40/user/mo + $5k setup).
- Confirm this baseline context is established in the chat thread before running any evaluation
prompts.
### Exercise 2 — Run Meta-Prompting and the CO-STAR Q-GoT Vendor Evaluation
Task: Draft a Meta-Prompt instructing ChatGPT to generate a specialized B2B CRM research
prompt, then execute a CO-STAR-structured prompt combined with Q-GoT calculations to determine
1-year and 3-year Total Cost of Ownership (TCO) for each vendor.
Answer — Setup Steps:
- Meta-Prompt: Act as an expert Prompt Engineer. Write a system prompt turning ChatGPT into a
specialized B2B CRM Pricing and Feature Researcher, focused on comparing Salesforce
Enterprise, HubSpot Sales Hub, and Zoho CRM, enforcing verified licensing models and
structured Markdown output (REQ-003).
- Save the generated prompt block into prompt_portfolio.md.
- CO-STAR Q-GoT Prompt: Using Context (Apex Cloud Services, 150 reps, three vendor cost
structures), Objective (run a Q-GoT evaluation to calculate 1-year and 3-year TCO), System
Controls (calculate TCO = User Count × Cost/mo × Months + Setup Fee, then self-check the
arithmetic), Style (McKinsey Strategy Consultant), Tone (objective, analytical, finance-first),
Audience (CEO and Board of Directors), and Response (structured markdown analysis with a
recommendation) (REQ-001, CON-001).
- Execute the prompt and save the verified TCO output.
### Exercise 3 — Build the Weighted Decision Matrix and Phased Roadmap
Task: Generate a markdown decision matrix scoring the three vendors against weighted criteria,
then produce a 6-month Gantt roadmap and risk registry for the selected vendor.
Answer — Setup Steps:
- Create the Decision Matrix prompt using four criteria: TCO Cost Model (30%), Customization &
Scale (20%), Setup Speed (25%), and User Adoption Ease (25%), with raw scores (1–10)
multiplied by weight (TR-002).

- Verify the weights sum to exactly 1.0 (100%) and confirm the math steps shown (e.g., Weighted
Score = Raw Score × Weight). Save the matrix to decision_matrix.md.
- Generate the Roadmap & Gantt prompt for the selected vendor (HubSpot), covering: Phase 1 –
Planning & Data Cleanup (Month 1), Phase 2 – System Configuration & Pilot (Months 2–3),
Phase 3 – Full Migration & Staff Training (Months 4–5), and Phase 4 – Post-Launch Optimization
(Month 6), formatted as a markdown text Gantt chart (REQ-004).
- Generate the Risk Registry prompt identifying 3 implementation risks in a table with Risk Event,
Probability, Impact, and Mitigation columns. Save both to implementation_plan.md.
### Exercise 4 — Write the Business Proposal, Executive Presentation, and Lessons Learned
Report
Task: Compile a B2B business proposal and a 6-slide executive presentation using markdown slide
dividers, then write a lessons learned report reflecting on LLM capabilities and limitations.
Answer — Setup Steps:
- Generate the Executive Presentation prompt producing 6 slides (Title & Overview, Client
Problem & Metrics, Vendor Candidates, Cost-Benefit Analysis & TCO, Decision Matrix &
Recommendation, Phased Roadmap & Next Steps), separated by exactly three dashes (---)
(REQ-005, TR-003).
- Save the slide deck to executive_presentation.md and the full proposal text to
business_proposal.md.
- Create lessons_learned_report.md covering: Hallucination Prevention (how step-by-step math
audits prevented calculation errors), Context Window Wind-down (how model performance
degrades over long threads and how to manage it), and Framework Alignment (when to use
RGCCO, CARE, ERA, or CO-STAR) (REQ-006, CON-002).
### Exercise 5 — Record Loom, Organize, and Push Deliverables to GitHub
Task: Record a 4-to-6-minute Loom video demonstrating the capstone system, then organize all
files into a local project folder and push them to a public GitHub repository.
Answer — Setup Steps:
- Log in to Loom, set up screen and webcam bubble, and record a paced 4–6 minute walkthrough:
- 0:00–1:00: Introduce yourself and summarize the B2B CRM migration case study.
- 1:00–2:00: Walk through your prompt_portfolio.md library and explain CO-STAR and Q-GoT
techniques.
- 2:00–4:00: Paste the CO-STAR Q-GoT vendor evaluation prompt live in ChatGPT and show
the 1-year and 3-year TCO calculated step-by-step.
- 4:00–5:30: Show executive_presentation.md slide formatting and explain the
lessons_learned_report.md insights.
- Copy the public Loom share URL, ensuring sharing is set to "Anyone with the link can view."
- Create a local folder named prompt-engineering-capstone and move in: prompt_portfolio.md,
decision_matrix.md, business_proposal.md, implementation_plan.md,
executive_presentation.md, lessons_learned_report.md, and README.md (with title, objectives,
your name, and the Loom URL) (REQ-007, TR-001).

- Run git init, git add ., git commit -m "Initialize Prompt Engineering Capstone project", git branch -
M main, git remote add origin https://github.com/YOUR_USERNAME/prompt-engineering-
capstone.git, and git push -u origin main.
git init
git add .
git commit -m "Initialize Prompt Engineering Capstone project"
git branch -M main
git remote add origin https://github.com/YOUR_USERNAME/prompt-engineering-capstone.git
git push -u origin main
- Confirm the repository is public and viewable from an incognito browser tab.
## 5. Practical Assessment Checklist

Status Requirement / Task Description
[ ] Enterprise Case Study (Apex Cloud Services)
Defined with User Count and Financial Metrics
[ ] Meta-Prompt Executed to Generate
Specialized Research Prompt

[ ] CO-STAR Q-GoT Vendor Evaluation Executed
with 1-Year and 3-Year TCO Calculated
[ ] Self-Check Math Verification Printed for TCO

Calculations

[ ] Weighted Decision Matrix Built with Weights

Summing to 100%

[ ] Phased 6-Month Gantt Roadmap Generated
[ ] Risk Registry Table Generated with 3 Identified

Risks

[ ] Business Proposal Drafted and Saved to

business_proposal.md

[ ] Executive Presentation (6 Slides) Created with

--- Dividers

[ ] Lessons Learned Report Completed

(Hallucination, Context Wind-down, Framework
Alignment)

[ ] Loom Video Recorded (4–6 Minutes)
[ ] Loom Video Sharing Set to "Anyone with the

Link Can View"

[ ] README.md Created with Project Title, Name,

and Loom URL

[ ] Local Folder prompt-engineering-capstone

Created with All Files

[ ] GitHub Repository Initialized and Files Pushed
[ ] GitHub Repository Confirmed as Public
[ ] End-to-End Review of All Deliverables
Completed Before Submission

## 6. Assessment Success Criteria
- Complete a full, functioning AI-powered decision automation workflow from case study setup to
GitHub delivery.
- Successfully execute Meta-Prompting, CO-STAR, and Q-GoT techniques in ChatGPT with
mathematically verified TCO outputs.
- Build a decision matrix with weights summing to exactly 1.0 and correctly calculated weighted
scores.
- Produce a markdown-compatible Gantt roadmap, risk registry, business proposal, and 6-slide
executive presentation.
- Compile a lessons learned report addressing hallucination prevention, context window
degradation, and framework alignment.
- Record a Loom video of 4–6 minutes showing a live CO-STAR Q-GoT prompt execution with
visible TCO calculations.
- Publish a public GitHub repository containing all seven required files plus README.md with the
Loom video URL embedded.
## 7. Required Deliverables
Deliverable Item Requirement Status Description / Additional

Comments

Loom Video Link Mandatory 4–6 min demo showing case
study intro, prompt portfolio
walkthrough, and live CO-
STAR Q-GoT execution with
TCO math

GitHub Repository Link Mandatory Public repo named prompt-
engineering-capstone
containing all 6 markdown
deliverables and README.md
Supporting Documents Optional Screenshots of ChatGPT
outputs, additional prompt
iterations, or personal notes

## 8. Submission Guidelines
After completing the assessment, submit the following through the LMS:
- A Loom video link demonstrating: your self-introduction and case study summary, a
walkthrough of your prompt portfolio, and a live paste-and-run of the CO-STAR Q-GoT vendor
evaluation prompt showing TCO calculations on screen.
- A public GitHub repository link containing all capstone deliverables (prompt_portfolio.md,
decision_matrix.md, business_proposal.md, implementation_plan.md,
executive_presentation.md, lessons_learned_report.md) and your README.md with your name
and Loom URL.
- In the Description field, mention any challenges faced during Q-GoT calculations or GitHub
push, how they were resolved, any assumptions made about vendor pricing, known limitations,
or additional analysis explored beyond the required scope.
## 9. Final Submission Checklist
- Completed all five assessment exercises
- Verified the CO-STAR Q-GoT prompt executes correctly with accurate, self-checked TCO math
- Confirmed decision_matrix.md contains weighted scores summing correctly to 100%
- Confirmed executive_presentation.md uses proper --- slide dividers
- Confirmed README.md includes project title, your name, and the public Loom URL
- Confirmed GitHub repository is public and all files are visible
- Uploaded and verified Loom video is publicly accessible with sharing set to "Anyone with the link
can view"
- Reviewed all deliverables before submission
Note: In the Description field, mentioned challenges faced, resolutions, assumptions, limitations, and
any extra analysis implemented.

## 10. Important Note
CRITICAL SUBMISSION REQUIREMENT:
Before clicking Submit in the LMS, ensure that you have provided:
- A Loom video link demonstrating your case study introduction, prompt portfolio walkthrough,
and a live execution of the CO-STAR Q-GoT vendor evaluation prompt with TCO calculations
visible on screen.
- A public GitHub repository link showing your prompt-engineering-capstone folder
containing all six required markdown deliverables and README.md (with your name and
Loom URL).
- Additional comments in the Description field describing any challenges faced during Q-
GoT math verification or GitHub push, how they were resolved, assumptions about vendor
pricing or scoring, known limitations, or additional features implemented beyond the base
requirements.
Submissions without the required Loom video link or a publicly accessible GitHub
repository may be considered incomplete and may not be evaluated.
