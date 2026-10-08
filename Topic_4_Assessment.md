# TOPIC 4 — ASSESSMENT
Business Consultation Prompting & Analytical
Reasoning Frameworks
Comprehensive Implementation Guide, Technical Exercises & Assessment Criteria

## 1. Assessment Overview
This assessment evaluates your ability to set up a Virtual Consulting Workspace using ChatGPT, apply
advanced analytical reasoning frameworks (CoT, ToT, Self-Consistency, and APEX), execute structured
business consultation prompts on a real B2B case study, compile outputs into a structured Markdown
portfolio, and deliver all project files via a public GitHub repository with a Loom video walkthrough. The
assessment is based on the provided Requirement Document and Implementation Plan.
## 2. Assessment Objective
Demonstrate your ability to complete a full advanced prompt engineering workflow simulating a business
consulting engagement. The solution should include:
- Setting up a Virtual Consulting Workspace in ChatGPT using the Apex Retail Group B2B case study.
- Applying Chain of Thought (CoT) prompting to perform SWOT analysis and root-cause diagnosis of
business bottlenecks.
- Using Tree of Thoughts (ToT) prompting to generate and evaluate 3 competitive strategic solution
branches.
- Building a mathematically sound Weighted Decision Matrix comparing all three branches using
weighted criteria scoring.
- Generating a phased 12-month implementation roadmap and a risk mitigation registry using Planning
Prompting.
- Compiling all prompt templates, business analysis, decision matrix, and roadmap into structured
Markdown files.
- Recording a Loom video walkthrough demonstrating your prompt methodology and live ToT
evaluation execution.
- Publishing all deliverables to a public GitHub repository named prompt-engineering-consultant.
## 3. Prerequisites
- Review the Requirement Document before starting the project.
- Review the Implementation Plan for the step-by-step setup and configuration flow.
- Have access to a web browser and a stable internet connection.
- Have a free OpenAI account to access ChatGPT.
- Have completed Lesson 1, Lesson 2, and Lesson 3 of the Prompt Engineering course.

- Have a free GitHub account ready to create a public repository.
- Have a free Loom account (or any screen recorder) ready to record your video walkthrough.
- Prepare a local folder on your computer named prompt-engineering-consultant to organize your
deliverables.
## 4. Assessment Tasks & Answers
### Exercise 1 — Set Up the Virtual Consulting Workspace & Case Study
Task: Initialize your consulting environment in ChatGPT by setting up the Apex Retail Group B2B client
dossier as your working context. Familiarize yourself with the key client metrics that will drive all
subsequent prompts.
Answer --- Setup Steps:
- Open your browser and navigate to https://chatgpt.com/ and log in to your account.
- Click the New Chat button to open a clean thread free of prior context.
- Open a local text editor and create your draft workspace by copying and pasting the following B2B
retail client matrix:
=== CLIENT DOSSIER: APEX RETAIL GROUP ===
- Background: Apex operates 45 brick-and-mortar apparel stores.
- Financials: Annual revenue is $12M, but margins have declined by 15% due to inventory
carry costs.
- Foot Traffic: Decreased by 25% year-over-year.
- E-commerce: Active online store, but cart abandonment is at 82% and conversion rate is low
(1.2%).
- Operational Bottlenecks: Over-stocked warehouses, slow shipping speeds (5-7 days), manual
inventory tracking.
=========================================
- Review and familiarize yourself with all client metrics as they will be referenced in every subsequent
prompt stage.
- Confirm the workspace is ready before proceeding to the diagnostic prompting stage.
### Exercise 2 — Run the 'Assess' & 'Pinpoint' Stages (CoT Diagnosis)
Task: Apply Chain of Thought (CoT) and Persona prompting to analyze the Apex Retail Group's current
state, perform a SWOT analysis, identify the single most critical root-cause bottleneck, and generate a gap
analysis comparing their current state with an optimized state (REQ-001).
Answer --- Setup Steps:
- In your text editor, draft the APEX Diagnostic Prompt:
Act as a Senior Management Consultant. We need to perform the ASSESS and PINPOINT
stages for our B2B retail client, Apex Retail Group.
[CLIENT METRICS]:
- 45 physical stores.
- Annual revenue: $12M. Margins down 15% due to inventory carry costs.

- Foot traffic down 25%.
- E-commerce conversion rate: 1.2%. Cart abandonment: 82%.
- Bottlenecks: Over-stocked warehouses, 5-7 days shipping, manual inventory tracking.
Let's think step-by-step to diagnose the situation:
1. Conduct a SWOT analysis based on the metrics.
2. Pinpoint the single most critical root-cause bottleneck. Explain your logic.
3. Generate a gap analysis comparing their current state with an optimized state.
- Paste the prompt into ChatGPT and run it.
- Review the output. Verify that the model highlights how inventory carry costs and manual tracking
are draining margins. Copy the diagnostics output to your local scratch file.
### Exercise 3 — Run the 'Evaluate' Stage (Tree of Thoughts)
Task: Use Tree of Thoughts (ToT) prompting to generate and evaluate three distinct competitive
strategic solution branches for Apex Retail Group, scoring each out of 10 and selecting the best candidate
(REQ-002).
Answer --- Setup Steps:
- Draft the ToT Evaluation Prompt:
We need to evaluate strategic solutions for Apex Retail Group. Generate three distinct
solution branches:
- Branch A: E-Commerce & Logistics Overhaul (Optimize online checkout, integrate
automated inventory, and switch to 3PL shipping).
- Branch B: Retail Footprint Downsizing (Close the 15 lowest-performing stores,
consolidate inventory, and reinvest capital).
- Branch C: Hybrid B2B Licensing (Franchise physical stores, license the brand, and
pivot corporate focus to online wholesale).
Evaluate each branch in parallel. For each option, analyze:
1. Estimated Impact on Margins (High/Med/Low).
2. Capital Expenditure (CapEx) required (High/Med/Low).
3. Execution Risk.
Let's think step-by-step. Score each branch out of 10 and select the best candidate.
- Run the prompt in ChatGPT. Copy the output candidate paths to your local scratch file.
- Self-Consistency Check: Open a new ChatGPT thread, paste the same prompt, and verify if it selects
the same winning branch (usually Branch A or a combination of A & B).
### Exercise 4 — Build the Weighted Decision Matrix
Task: Create a mathematically sound weighted decision matrix in Markdown format comparing all three
strategic branches using criteria with weights that sum to 100% (REQ-003, TR-002).
Answer --- Setup Steps:
- Draft the Decision Matrix Prompt:
Act as an Analyst. Create a markdown table comparing Branch A, Branch B, and Branch C.

Use these criteria and weights (weights must sum to 100%):
- ROI (30% weight)
- Low Execution Risk (20% weight)
- Implementation Speed (20% weight)
- Resource Alignment (30% weight)
For each option, assign a score from 1 (poor) to 10 (excellent) for each criterion,
calculate the weighted score, and sum them to find the winner.
Format:
| Solution | Criterion | Weight | Score (1-10) | Weighted Score |
- Verify the calculations manually: Weighted Score = Raw Score × Weight (e.g. if ROI is scored 9, the
weighted score is 9 × 0.30 = 2.70).
- Ensure the column weights sum to exactly 100% (or 1.0) as required by US-003.
- Copy the Markdown table to your decision_matrix.md draft file.
### Exercise 5 — Run the 'Execute' Stage (Roadmapping & Risks)
Task: Generate a phased 12-month implementation roadmap and a risk mitigation registry for Branch A
(E-Commerce & Logistics Overhaul) using Planning Prompting (REQ-004, TR-003).
Answer --- Setup Steps:
- Draft the Roadmap Planning Prompt:
We have selected Branch A (E-Commerce & Logistics Overhaul) as the winner. Act as a
Project Manager.
First, outline the three distinct implementation phases over a 12-month timeline. Pause
and write only the phase names and durations.
Once I say "Execute", write the detailed milestones, activities, and RACI assignments
for each phase.
- Send the prompt. Once ChatGPT outputs the phase outline, type Execute.
- Draft the Risk Log Prompt:
For the selected overhaul strategy, identify 3 critical implementation risks.
Format your response as a markdown table with columns:
- Risk Event
- Probability (Low/Med/High)
- Impact (Low/Med/High)
- Mitigation Strategy
- Copy the generated roadmap and risk log outputs to your implementation_roadmap.md draft file.
## 5. Practical Assessment Checklist
Status Requirement / Task Description

[ ] Virtual Consulting Workspace Initialized with Apex

Retail Group Client Dossier

[ ] APEX Diagnostic Prompt Executed with CoT (SWOT +

Root-Cause + Gap Analysis)

[ ] Output Verified: Inventory Carry Costs and Manual

Tracking Identified as Key Bottlenecks

[ ] ToT Evaluation Prompt Executed Generating 3 Strategic

Branches

[ ] Each Branch Scored Out of 10 and Winning Branch

Selected

[ ] Self-Consistency Check Performed in a New ChatGPT

Thread

[ ] Weighted Decision Matrix Created with Criteria

Weights Summing to 100%

[ ] Matrix Formula Verified: Weighted Score = Raw Score ×

Criteria Weight

[ ] 12-Month Implementation Roadmap Generated Using

Planning Prompting

[ ] Risk Log Generated with Risk Event, Probability,

Impact, and Mitigation Columns

[ ] business_analysis_report.md Created with SWOT,
Diagnostics, and Final Recommendation
[ ] prompt_collection.md Created with All Parameter-

Driven Prompt Templates

[ ] decision_matrix.md Created with Scored Markdown

Table

[ ] implementation_roadmap.md Created with 12-Month

Phases and Risk Logs

[ ] Loom Video Recorded (3 to 4 Minutes) Following the

Structured Agenda

[ ] Loom Video Sharing Set to "Anyone with the Link Can

View"

[ ] README.md Created with Project Title, Name,

Objectives, and Loom URL

[ ] Local Folder prompt-engineering-consultant Created

with All Required Files

[ ] GitHub Repository Initialized and All Files Pushed
[ ] GitHub Repository Confirmed as Public
[ ] End-to-End Review of All Deliverables Completed

Before Submission

## 6. Assessment Success Criteria
- Complete a full, functioning business consultation prompt engineering workflow from workspace
setup to GitHub delivery.
- Successfully apply CoT prompting to diagnose the Apex Retail Group case study with a SWOT analysis,
root-cause identification, and gap analysis.
- Generate exactly 3 competitive strategic branches using ToT prompting and select a winning branch
backed by a self-consistency check.
- Build a mathematically correct Weighted Decision Matrix in Markdown where all criteria weights sum
to 100% and all weighted scores are calculated using the formula: Weighted Score = Raw Score ×
Criteria Weight.
- Generate a phased 12-month implementation roadmap and a risk mitigation registry using planning
prompting.
- Compile all outputs into four correctly structured Markdown files: business_analysis_report.md,
prompt_collection.md, decision_matrix.md, and implementation_roadmap.md.
- Record a Loom video of 3 to 4 minutes demonstrating the APEX/ToT framework, prompt collection,
live ToT evaluation in ChatGPT, and the final Decision Matrix review.
- Publish a public GitHub repository named prompt-engineering-consultant containing all four
Markdown files and a README.md with the Loom video URL.
- Submit all required deliverables through the LMS with accessible public links.
## 7. Required Deliverables
Deliverable Item Requirement Status Description / Additional

Comments

Loom Video Link Mandatory 3–4 min demo covering: self-
introduction and case study

overview (0:00–0:45), prompt
collection walkthrough (0:45–2:00),
live ToT evaluation in ChatGPT
(2:00–3:15), and Decision Matrix
review (3:15–3:45)
GitHub Repository Link Mandatory Public repo named prompt-
engineering-consultant containing
business_analysis_report.md,
prompt_collection.md,
decision_matrix.md,
implementation_roadmap.md, and
README.md

Supporting Documents Optional Screenshots of ChatGPT outputs for
each APEX stage, additional prompt
iterations, self-consistency check
results, or personal notes on
strategic reasoning

## 8. Submission Guidelines
After completing the assessment, submit the following through the LMS:
- A Loom video link demonstrating: your self-introduction and outline of the Apex Retail Group case
study, your prompt_collection.md file explaining the difference between linear CoT and multi-branch
ToT prompting, a live paste-and-run of the ToT Evaluation Prompt in ChatGPT showing how the
model scores and selects the winning strategic path, and a review of the final Decision Matrix table.
- A public GitHub repository link containing all four Markdown deliverable files
(business_analysis_report.md, prompt_collection.md, decision_matrix.md,
implementation_roadmap.md) and a README.md with your name, project objectives, and Loom URL.
- In the Description field, mention any challenges faced during the weighted matrix calculation or
roadmap generation, how they were resolved (e.g. using planning prompting to avoid token
truncation), any assumptions made about strategic branch scoring, known limitations, or additional
prompt variations explored beyond the required stages.
## 9. Final Submission Checklist
- Completed all five assessment exercises
- Verified CoT diagnostic output correctly identifies inventory carry costs and manual tracking as the
root-cause bottlenecks
- Confirmed ToT prompt generates exactly 3 strategic branches with individual scores out of 10
- Confirmed self-consistency check validates the winning branch selection

- Confirmed decision_matrix.md criteria weights sum to exactly 100% and all weighted score
calculations are mathematically correct
- Confirmed implementation_roadmap.md contains the 12-month phased roadmap and the risk log
table with all four required columns
- Confirmed all four Markdown files are present and correctly structured in the GitHub repository
- Confirmed README.md includes project title, your name, objectives, and the public Loom URL
- Confirmed GitHub repository is public and all files are visible
- Uploaded and verified Loom video is publicly accessible with sharing set to "Anyone with the link can
view"
- Reviewed all deliverables before submission
Note: In the Description field, mention challenges faced during matrix calculations or roadmap
generation, how they were resolved, assumptions made, limitations encountered, and any additional
prompt strategies implemented beyond the required five stages.
## 10. Important Note
CRITICAL SUBMISSION REQUIREMENT:
Before clicking Submit in the LMS, ensure that you have provided:
1. A Loom video link (minimum 3 minutes) demonstrating your active ChatGPT workspace, self-introduction
with the Apex Retail Group case study overview, a live execution of the ToT Evaluation Prompt with the model's
scoring and branch selection visible on screen, and a review of the final Decision Matrix.
2. A public GitHub repository link showing your prompt-engineering-consultant folder containing all five
required files: business_analysis_report.md (with SWOT, diagnostics, and final recommendation),
prompt_collection.md (with all parameter-driven prompt templates), decision_matrix.md (with the scored
weighted matrix), implementation_roadmap.md (with 12-month phases, milestones, and risk logs), and
README.md (with your name, objectives, and Loom URL).
3. Additional comments in the Description field describing any challenges faced during weighted matrix
calculation or roadmap generation using planning prompting, how they were resolved, assumptions about
strategic branch scoring, known limitations, or additional prompt frameworks implemented beyond the required
APEX stages.
Submissions without the required Loom video link or a publicly accessible GitHub repository may be considered
