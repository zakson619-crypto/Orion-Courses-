# TOPIC 5 — ASSESSMENT
**AI-Assisted Research & Knowledge Verification**
**Architectures**
**Comprehensive Implementation Guide, Technical Exercises & Assessment Criteria**

## 1. Assessment Overview
This assessment evaluates your ability to set up a ChatGPT research workspace, apply advanced
knowledge-grounding techniques, execute a full Chain of Verification (CoVe) audit cycle, compile a
structured research report and comparison matrix, and deliver all project files via a public GitHub
repository with a Loom video walkthrough. The assessment is based on the provided Requirement
Document and Implementation Plan.

## 2. Assessment Objective
Demonstrate your ability to complete a full AI-assisted research workflow using advanced prompt
engineering techniques that follow course best practices. The solution should include:
- Using Generated Knowledge Prompting to compile verified background facts about three container
orchestration technologies before drafting any report.
- Applying the ERA (Expectation, Role, Action) framework to structure a detailed technical comparison
prompt in ChatGPT.
- Executing the full 4-step Chain of Verification (CoVe) cycle — drafting, formulating verification
questions, independently answering them, and applying corrections.
- Running an Assumption Audit Prompt to identify 3 hidden latent biases in the finalized comparison
report.
- Compiling a Comparison Matrix (Markdown table) and a 150-word Executive Summary.
- Recording a Loom video walkthrough of minimum 3 minutes demonstrating the live CoVe process.
- Publishing all deliverables to a structured public GitHub repository.

## 3. Prerequisites
- Review the Requirement Document before starting the project.
- Review the Implementation Plan for the step-by-step setup and configuration flow.
- Have completed Lessons 1 through 4 of the Prompt Engineering Hands-On Course.
- Have access to a web browser and a stable internet connection.
- Have a free OpenAI account to access ChatGPT.
- Have a free GitHub account ready to create a public repository named prompt-engineering-
researcher.
- Have a free Loom account (or any screen recorder) ready to record your video walkthrough.
- Prepare a local folder on your computer named prompt-engineering-researcher to organize your
deliverables.

## 4. Assessment Tasks & Answers

### Exercise 1 — Set Up the Research Workspace and Generate Background Knowledge
Task: Open a fresh ChatGPT session, identify the three container orchestration technologies to be studied,
and execute the Generated Knowledge Prompt to compile a verified background fact sheet before drafting
any report.
Answer — Setup Steps:
- Open your browser and navigate to https://chatgpt.com/ and log in to your account.
- Click the New Chat button to clear any prior conversation context and start a clean research session.
- Confirm the three technologies that will be compared throughout this project: Kubernetes (K8s),
Docker Swarm, and AWS Fargate (Serverless Containers).
- In your text editor, draft the Generated Knowledge Prompt as follows:
Generate a factual summary detailing the core architecture, scalability limits,
setup complexity, and cost structures of the following three technologies:
Kubernetes, Docker Swarm, and AWS Fargate. Focus on raw specifications, documentation
facts, and industry statistics. Do not write a comparison or recommendations yet.
Keep your focus on compiling background knowledge.
- Paste the prompt into ChatGPT and run it.
- Review the output to verify key factual points — such as Kubernetes node limits, Docker Swarm's
built-in status, and AWS Fargate's pay-as-you-go pricing — are present and accurate.
- Save this compilation locally as your background fact sheet. This fulfills REQ-001 (Knowledge
Grounding).

### Exercise 2 — Draft the Baseline Research Report Using the ERA Framework
Task: Use the ERA (Expectation, Role, Action) framework to write and execute a structured research
prompt in ChatGPT that produces an initial, unverified comparison report based on the fact sheet
generated in Exercise 1.
Answer — Setup Steps:
- In your text editor, draft the ERA Research Prompt using the three ERA parameters as follows:
[EXPECTATION]: I expect a detailed comparison report comparing Kubernetes, Docker
Swarm, and AWS Fargate. Structure the response with H2 headers for: Introduction,
Tech Overviews, Detailed Comparison, and Final Verdict. Do not write summary tables yet.
[ROLE]: Act as a Lead Systems Architect.
[ACTION]: Write the comparison report based on the following background facts:
=== BACKGROUND FACTS ===
[Insert the fact sheet generated in Exercise 1]
- Run the prompt in ChatGPT.
- Copy the full output text and save it in a local scratch file labeled baseline_draft.txt. This baseline draft
will be used as the input for the CoVe audit cycle in the next exercise. This fulfills REQ-002 (ERA
Prompting).

### Exercise 3 — Execute the Full Chain of Verification (CoVe) Cycle
Task: Audit the baseline draft using a 4-step self-correcting verification loop — formulating verification
questions, independently answering them with verified facts, and producing a corrected final report.
Answer — Setup Steps:
- Draft the CoVe Question Formulation Prompt:
Read the baseline draft comparison below. Formulate a list of exactly four specific
verification questions that can be answered with absolute facts to audit the claims,
numbers, and limitations stated in the text (e.g. check version limits, specific
scalability numbers, or operational dependencies).
[BASELINE DRAFT]:
[Insert the text from baseline_draft.txt]
- Run the prompt. ChatGPT will output four targeted audit questions (e.g., "Does Docker Swarm require
external key-value stores?", "What is the node limit of Kubernetes?").
- Draft the CoVe Question Answering Prompt:
Answer each of the following verification questions one-by-one. Rely strictly on
verified developer documentation facts:
[Insert the four questions generated in the previous step]
- Run the prompt and capture the verified answers.
- Draft the CoVe Correction Prompt:
Review the original baseline draft. Rewrite the report incorporating the verified
corrections below. Ensure the final report is fully accurate and resolved.
[BASELINE DRAFT]: [Insert baseline_draft.txt]
[VERIFIED CORRECTIONS]: [Insert the answers from the previous step]
- Execute the prompt in ChatGPT. Copy the corrected final output. This will form the core of your
Research Report. This fulfills REQ-003 (Fact Verification / CoVe Audit Trail — TR-002).

### Exercise 4 — Run the Assumption Audit and Compile the Comparison Matrix & Executive
Summary
Task: Audit the finalized research report for hidden latent biases using the Assumption Audit Prompt,
then generate the Comparison Matrix and a 150-word Executive Summary.
Answer — Setup Steps:
- Draft the Assumption Audit Prompt:
Analyze the finalized technology comparison below. Identify and list 3 hidden
assumptions the writer makes regarding the technologies (e.g. assuming high capital
expense always correlates with higher quality, or assuming simplicity is always
better for small teams). Detail if these assumptions introduce bias.
[FINALIZED REPORT]:
[Insert the corrected report from Exercise 3]
- Execute the prompt in ChatGPT. Save the assumption list. This fulfills REQ-004 (Bias Identification).
- Draft the Comparison Matrix Prompt:
Create a markdown table comparing Kubernetes, Docker Swarm, and AWS Fargate across
these columns: Technology, Scalability (High/Med/Low), Setup Complexity
(High/Med/Low), Operational Overhead (High/Med/Low), Cost Model (e.g. Pay-per-node,
Pay-per-use, Free).
- Run the prompt and save the output as comparison_matrix.md. This fulfills REQ-005 and TR-003.
- Draft the Executive Summary Prompt:
Write a 150-word executive summary synthesizing the comparison findings. Recommend
the best technology for a fast-growing startup prioritizing speed over infrastructure
scaling.
- Run the prompt and save the output as executive_summary.md.

### Exercise 5 — Record the Loom Video and Push All Deliverables to GitHub
Task: Record a 3-to-4 minute Loom video demonstrating your research architecture and live CoVe
process, then organize and push all deliverables to a public GitHub repository.
Answer — Setup Steps:
- Sign in to Loom at https://www.loom.com/ and configure your screen-share and webcam bubble.
- Follow this structured timeline for your recording:
- 0:00 – 0:45: State the project name (AI Research & Knowledge Assistant) and explain the CoVe
methodology and why it prevents hallucinations.
- 0:45 – 2:00: Show your prompt_documentation.md file. Explain the ERA parameters and walk through
all 4 CoVe steps.
- 2:00 – 3:15: Open your browser tab with ChatGPT. Paste your CoVe Question Answering Prompt live
and run it. Show how ChatGPT checks its own draft.
- 3:15 – 3:45: Show the final Comparison Matrix table and close the video.
- Copy the public Loom share URL. This fulfills REQ-007.
- Create a local folder named prompt-engineering-researcher and move the following files into it:
- research_report.md — Contains background fact sheet, final verified text, and the 4 CoVe steps log.
- executive_summary.md — The 150-word summary.
- comparison_matrix.md — The scored Markdown table.
- prompt_documentation.md — Contains the exact ERA and CoVe prompt templates with parameters.
- README.md — Contains project title, objectives, your name, and the Loom video URL.
- Open a terminal inside the folder and run the following Git commands:
git init
git add .
git commit -m "Initialize Prompt Engineering Research Assistant project"
git branch -M main
git remote add origin https://github.com/YOUR_USERNAME/prompt-engineering-researcher.git
git push -u origin main
- Confirm your repository is set to public and is viewable from an incognito browser tab. This fulfills
REQ-006 (GitHub Submission — TR-001).

## 5. Practical Assessment Checklist
Status Requirement / Task Description
- [ ] Generated Knowledge Prompt Executed and
Background Fact Sheet Saved
- [ ] ERA Research Prompt Drafted with Correct
Expectation, Role, and Action Parameters
- [ ] Baseline Draft (baseline_draft.txt) Generated and Saved
- [ ] CoVe Step 1: Verification Question Formulation Prompt
Executed (4 Questions Generated)
- [ ] CoVe Step 2: Verification Question Answering Prompt
Executed with Verified Facts
- [ ] CoVe Step 3: CoVe Correction Prompt Executed and
Final Corrected Report Saved
- [ ] Assumption Audit Prompt Executed and 3 Latent
Assumptions Identified
- [ ] Comparison Matrix (Markdown Table) Created with All
5 Required Columns
- [ ] 150-Word Executive Summary Created
- [ ] prompt_documentation.md Compiled with All Exact
Prompt Templates
- [ ] Loom Video Recorded (3–4 Minutes) Covering All 4
Required Timeline Segments
- [ ] Loom Video Sharing Set to "Anyone with the Link Can
View"
- [ ] README.md Created with Project Title, Name, and
Loom URL
- [ ] All 5 Files Organized in prompt-engineering-researcher
Folder
- [ ] GitHub Repository Initialized, Pushed, and Confirmed
as Public

## 6. Assessment Success Criteria
- Complete a full AI-assisted research workflow from knowledge grounding through GitHub delivery.
- Successfully execute the ERA framework to produce a structured, role-assigned baseline comparison
report.
- Demonstrate a complete 4-step CoVe audit cycle with all verification questions, verified answers, and
corrections clearly documented in research_report.md.
- Identify 3 latent assumptions and biases in the finalized report using the Assumption Audit Prompt.
- Compile a correctly structured Comparison Matrix across at least 4 uniform columns (Technology,
Scalability, Setup Complexity, Cost Model) as per TR-003.
- Record a Loom video of 3 to 4 minutes that covers the CoVe methodology explanation, prompt
documentation walkthrough, a live CoVe prompt run, and the Comparison Matrix.
- Publish a public GitHub repository containing all 5 required deliverable files with clean Markdown
formatting as per TR-001 and CON-003.
- Submit all required deliverables through the LMS with accessible public links.

## 7. Required Deliverables
Deliverable Item Requirement Status Description / Additional
Comments
Loom Video Link Mandatory 3–4 min demo covering CoVe
methodology,
prompt_documentation.md
walkthrough, live CoVe Question
Answering prompt run, and final
Comparison Matrix
GitHub Repository Link Mandatory Public repo named prompt-
engineering-researcher containing
all 5 required markdown files
research_report.md Mandatory Includes background facts, verified
final report text, and full CoVe audit
trail (4 steps logged)
comparison_matrix.md Mandatory Markdown table with Technology,
Scalability, Setup Complexity,
Operational Overhead, and Cost
Model columns
executive_summary.md Mandatory 150-word synthesis recommending
the best technology for a fast-
growing startup
prompt_documentation.md Mandatory Exact ERA and CoVe prompt
templates with all parameter
variables
Supporting Documents Optional Screenshots of ChatGPT CoVe steps,
additional prompt iterations, or
personal research notes

## 8. Submission Guidelines
After completing the assessment, submit the following through the LMS:
- A Loom video link demonstrating: an explanation of the CoVe methodology, a walkthrough of your
prompt_documentation.md showing ERA parameters and all 4 CoVe prompts, and a live paste-and-
run of the CoVe Question Answering Prompt showing ChatGPT auditing its own draft in real time.
- A public GitHub repository link containing all 5 required files — research_report.md (with CoVe audit
trail), executive_summary.md, comparison_matrix.md, prompt_documentation.md, and README.md
with your name and Loom URL.
- In the Description field, mention any challenges faced during the CoVe cycle or GitHub push, how they
were resolved, any assumptions made about the technologies being compared, known limitations of
ChatGPT's knowledge on the topic, and any additional prompt techniques explored beyond the
required steps.

## 9. Final Submission Checklist
- Completed all five assessment exercises
- Verified the Generated Knowledge Prompt produces a factual background sheet referenced in the
final report
- Confirmed research_report.md contains the full CoVe audit trail — baseline draft, 4 verification
questions, verified answers, and corrected report
- Confirmed comparison_matrix.md covers all 5 columns with High/Med/Low ratings and Cost Model
entries
- Confirmed executive_summary.md is 150 words and contains a technology recommendation
- Confirmed prompt_documentation.md contains all exact ERA and CoVe prompt templates
- Confirmed GitHub repository is public and all 5 files are visible and correctly rendered in Markdown
- Uploaded and verified Loom video is publicly accessible with sharing set to "Anyone with the link can
view"
- Reviewed all deliverables before submission
Note: In the Description field, mention challenges faced during the CoVe cycle, how they were resolved,
assumptions about technology comparisons, known limitations of ChatGPT's knowledge cutoff, and any
extra prompt techniques implemented.

## 10. Important Note
CRITICAL SUBMISSION REQUIREMENT:
Before clicking Submit in the LMS, ensure that you have provided:
1. A Loom video link (3–4 minutes) demonstrating your CoVe methodology explanation,
prompt_documentation.md walkthrough covering all ERA and CoVe parameters, and a live execution of the CoVe
Question Answering Prompt with ChatGPT's output visible on screen.
2. A public GitHub repository link showing your prompt-engineering-researcher folder containing all 5 required
files: research_report.md (with full CoVe audit trail), executive_summary.md, comparison_matrix.md,
prompt_documentation.md, and README.md with your name and Loom URL.
3. Additional comments in the Description field describing any challenges faced during the CoVe cycle or GitHub
push, how they were resolved, assumptions about technology outputs, known limitations regarding ChatGPT's
knowledge cutoff (CON-001), and any additional prompt techniques implemented beyond the required steps.
Submissions without the required Loom video link or a publicly accessible GitHub repository may be considered
