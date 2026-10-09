# TOPIC 6 — ASSESSMENT

AI-Driven Software Development Lifecycle (SDLC) Prompting
Comprehensive Implementation Guide, Technical Exercises &
Assessment Criteria

## 1. Assessment Overview

This assessment evaluates your ability to set up a ChatGPT-driven development workspace, apply
advanced prompting techniques (Least-to-Most decomposition, the CRISPE framework, and
reflection prompting) to build a backend REST API, generate secure code with supporting
documentation and tests, and deliver all project files via a public GitHub repository with a Loom
video walkthrough. The assessment is based on the provided Requirement Document and
Implementation Plan.

## 2. Assessment Objective

Demonstrate your ability to complete a full AI-driven SDLC workflow that follows course best
practices. The solution should include:
- Setting up a ChatGPT workspace and defining the target project — B2B "Task Tracker
REST API."
- Generating software requirements and user stories using Least-to-Most prompting.
- Designing SQL database schemas with proper keys and constraints.
- Generating route controllers using the CRISPE framework.
- Running a Secure Reflection audit to identify and refactor vulnerable code (e.g., SQL injection).
- Generating Swagger/OpenAPI documentation and unit tests.
- Compiling all deliverables into a structured Markdown-based Prompt Library and SRD.
- Recording a Loom video walkthrough demonstrating the live secure reflection code review.
- Publishing all deliverables to a public GitHub repository.

## 3. Prerequisites

- Review the Requirement Document before starting the project.
- Review the Implementation Plan for the step-by-step setup and configuration flow.
- Have access to a web browser and a stable internet connection.
- Have a free OpenAI account to access ChatGPT.
- Have a free GitHub account ready to create a public repository.
- Have a free Loom account (or any screen recorder) ready to record your video walkthrough.
- Basic coding familiarity with Python or JavaScript and SQL query structure.
- Prepare a local folder on your computer named prompt-engineering-developer to organize your
deliverables.

## 4. Assessment Tasks & Answers


### Exercise 1 — Set Up the Coding Workspace and Define the Target Project

Task: Initialize your ChatGPT development session and define the software to be built — a B2B
"Task Tracker REST API" handling Users, Tasks, and Status Management.
Answer — Setup Steps:
- Open your browser and navigate to https://chatgpt.com/, then log in to your account.
- Click New Chat to clear the conversation context window before starting.
- Confirm the scope of the project: a B2B Task Tracker REST API covering Users (Registration,
Login, Auth tokens), Tasks (CRUD operations), and Status Management (Open, In Progress,
Completed).
- Verify you are working in a clean workspace before running any prompts (REQ-001).

### Exercise 2 — Generate Requirements, Schema, and Controllers

Task: Use Least-to-Most prompting to generate software requirements and user stories, then design
SQL schemas, and finally generate route controllers using the CRISPE framework.
Answer — Setup Steps:
- Least-to-Most Requirements Prompt: "Act as a Business Analyst. We want to design a
backend REST API named 'Task Tracker API'. First, outline the system architecture scope and
write 3 core B2B user stories (for User Signup, Task Creation, and Task Updates) with
acceptance criteria. Do not write database schemas or backend code yet." Save the output to
srd_draft.txt (REQ-001).
- SQL Database Schema Prompt: Instruct ChatGPT to generate relational SQL table schemas
for users (id, name, email, password_hash, created_at) and tasks (id, user_id, title, description,
status, due_date, created_at), including NOT NULL, UNIQUE, FOREIGN KEY, and PRIMARY
KEY constraints, with raw DDL SQL output (REQ-003).
- CRISPE Coding Prompt: Following the CRISPE framework (Capacity, Recipient, Instruction,
Style, Parameters, Evaluation), instruct ChatGPT to act as a Senior Backend Software Engineer
and write route controller logic in Node.js/Express or Python/FastAPI for POST /api/v1/tasks and
GET /api/v1/tasks/:id, following DRY/SOLID principles, using raw SQL (no ORM), with inline
comments (REQ-002, REQ-004). Save the code draft in a local folder named code_repository/.

### Exercise 3 — Run Secure Code Reflection and Debugging

Task: Audit your generated controllers for security exploits (such as SQL injection) using a reflection
prompt, and verify the refactored output uses parameterized queries.
Answer — Setup Steps:
- Copy a mock vulnerable endpoint (e.g., a /api/v1/login route built with string-concatenated SQL)
into ChatGPT as the code to audit.
- Secure Reflection Prompt: "Act as a Security Auditor. Scan the code block below for security
vulnerabilities (e.g., SQL Injection, unhandled crashes). Identify the issue, explain the risk, and
write a refactored, secure version of this endpoint using parameterized SQL queries and
try/catch blocks" (REQ-005, TR-003).
- Run the prompt in ChatGPT and verify the output replaces the vulnerable query with a
parameterized query, e.g., db.query("SELECT * FROM users WHERE email = ? ...", [email,
password]).

### Exercise 4 — Generate Documentation, Tests, and Compile Deliverables

Task: Generate Swagger/OpenAPI documentation and unit tests for your endpoints, then compile all
outputs into structured Markdown deliverable files.
Answer — Setup Steps:
- API Documentation Prompt: Generate Swagger/OpenAPI YAML documentation for POST
/api/v1/tasks and GET /api/v1/tasks/:id, including request schema, 200 success response, and
400 error response blocks (REQ-006).
- Unit Test Prompt: Act as a QA Automation Engineer and write 2 unit tests in Jest/Supertest (or
Python PyTest) validating successful task creation (asserts status 201) and getting a task with
an invalid ID (asserts status 404) (REQ-006).
- Create the following four files (TR-001):
- api_documentation.md — containing your Swagger YAML block.
- test_cases.md — containing your unit tests and a QA test matrix table.
- prompt_library.md — containing your exact CRISPE, Least-to-Most, and Reflection prompt
templates with parameter variables.
- software_requirement_document.md — containing the user stories, SQL scripts, and final
code controllers.

### Exercise 5 — Record Loom Video and Push Deliverables to GitHub

Task: Record a 3-to-4-minute Loom video demonstrating your workspace and a live secure
reflection code review, then organize and push all deliverables to a public GitHub repository.
Answer — Setup Steps:
- Log in to Loom at https://www.loom.com/ and configure screen and webcam recording (REQ-
008).
- Follow this structured recording timeline:
- 0:00 – 0:45: State the project name (AI Software Development Assistant) and explain the
Least-to-Most prompting pipeline.
- 0:45 – 2:00: Show your local folder files (code_repository/ and markdown files) and explain
the CRISPE variables.
- 2:00 – 3:15: Open ChatGPT and paste your Secure Reflection Prompt live with the
vulnerable login route; show ChatGPT refactoring the code to block SQL injection.
- 3:15 – 3:45: Show the unit tests and conclude the video.
- Ensure the Loom video sharing settings are set to "Anyone with the link can view."
- Create a local directory named prompt-engineering-developer and move in:
software_requirement_document.md, api_documentation.md, test_cases.md, prompt_library.md,
code_repository/, and README.md (title, objectives, your name, and the Loom video URL)
(REQ-007, TR-001).
- Open a terminal inside the folder and run:
git init
git add .
git commit -m "Initialize Prompt Engineering Developer project"
git branch -M main
git remote add origin https://github.com/YOUR_USERNAME/prompt-engineering-
developer.git
git push -u origin main
- Confirm your repository is set to public and viewable from an incognito browser tab.

## 5. Practical Assessment Checklist

Status Requirement / Task Description
[ ] ChatGPT Workspace Set Up and Target
Project (Task Tracker API) Defined
[ ] Least-to-Most Requirements Prompt Executed
— User Stories Generated
[ ] SQL Database Schema Prompt Executed with
Constraints
[ ] CRISPE Route Controllers Generated
(POST/GET endpoints)
[ ] Secure Reflection Prompt Executed — SQL
Injection Identified and Fixed
[ ] Swagger/OpenAPI Documentation Generated
[ ] Unit Tests Generated (Jest/Supertest or
PyTest)
[ ] software_requirement_document.md Created
[ ] api_documentation.md Created
[ ] test_cases.md Created
[ ] prompt_library.md Created
[ ] Loom Video Recorded (3–4 Minutes)
[ ] Loom Video Sharing Set to "Anyone with the
Link Can View"
[ ] README.md Created with Project Title,
Objectives, Name, and Loom URL
[ ] Local Folder prompt-engineering-developer
Created with All Files
[ ] GitHub Repository Initialized and Files Pushed
[ ] GitHub Repository Confirmed as Public
[ ] End-to-End Review of All Deliverables
Completed Before Submission

## 6. Assessment Success Criteria

- Complete a full, functioning AI-driven SDLC workflow from requirements gathering to GitHub
delivery.
- Successfully execute Least-to-Most, CRISPE, and Reflection prompts producing accurate
schemas, secure controllers, documentation, and tests.
- Compile all deliverables into correctly structured Markdown files
(software_requirement_document.md, api_documentation.md, test_cases.md,
prompt_library.md).
- Record a Loom video of 3–4 minutes that shows your workspace, folder structure, and a live
secure reflection code review.
- Publish a public GitHub repository containing all deliverables with the Loom video URL
embedded in README.md.
- Submit all required deliverables through the LMS with accessible public links.

## 7. Required Deliverables

Deliverable Item Requirement Status Description / Additional
Comments
Loom Video Link Mandatory 3–4 min demo showing project
overview, folder structure, and
live Secure Reflection Prompt
execution fixing SQL injection
GitHub Repository Link Mandatory Public repo named prompt-
engineering-developer
containing
software_requirement_docum
ent.md,
api_documentation.md,
test_cases.md,
prompt_library.md,
code_repository/, and
README.md
Supporting Documents Optional Screenshots of ChatGPT
outputs, additional prompt
iterations, or personal notes

## 8. Submission Guidelines

After completing the assessment, submit the following through the LMS:
- A Loom video link demonstrating: your project overview and Least-to-Most pipeline
explanation, your local folder/CRISPE variables walkthrough, and a live paste-and-run of the
Secure Reflection Prompt showing ChatGPT refactoring the vulnerable login route.
- A public GitHub repository link containing all four Markdown deliverables, the
code_repository/ folder, and your README.md with your name and Loom URL.
- In the Description field, mention any challenges faced during schema generation, token limits,
or GitHub push, how they were resolved, any assumptions made about the prompt outputs,
known limitations, or additional prompts explored beyond the required set.

## 9. Final Submission Checklist

- Completed all five assessment exercises
- Verified all prompts (Least-to-Most, SQL Schema, CRISPE, Secure Reflection, Documentation,
Unit Test) execute correctly in ChatGPT
- Confirmed all four Markdown deliverables are present with proper formatting
- Confirmed README.md includes project title, objectives, your name, and the public Loom URL
- Confirmed GitHub repository is public and all files/folders are visible
- Uploaded and verified Loom video is publicly accessible with sharing set to "Anyone with the link
can view"
- Reviewed all deliverables before submission
Note: In the Description field, mentioned challenges faced, resolutions, assumptions, limitations, and
any extra prompts implemented.

## 10. Important Note

CRITICAL SUBMISSION REQUIREMENT:
Before clicking Submit in the LMS, ensure that you have provided:
- A Loom video link demonstrating your project workspace, folder structure walkthrough, and
a live execution of the Secure Reflection Prompt with the refactored, secure output visible on
screen.
- A public GitHub repository link showing your prompt-engineering-developer folder
containing software_requirement_document.md, api_documentation.md, test_cases.md,
prompt_library.md, code_repository/, and README.md (with your name and Loom URL).
- Additional comments in the Description field describing any challenges faced during
setup, schema generation, or GitHub push, how they were resolved, assumptions about
prompt outputs, known limitations, or additional features implemented beyond the required
prompts.
Submissions without the required Loom video link or a publicly accessible GitHub
