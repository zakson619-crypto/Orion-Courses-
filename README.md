# Prompt Engineering Foundations & Structured Frameworks

**Topic 2 — Hands-On Assessment: Prompt Engineering Portfolio**

**Prepared by:** [Your Name]  
**Loom walkthrough:** [Add public Loom video URL]  
**GitHub repository:** [Add public GitHub repository URL]

## Project Overview

This project develops a reusable prompt library for creating marketing content with ChatGPT. It compares basic (naive) prompts against optimized prompts to demonstrate how structured prompt engineering improves relevance, tone, formatting, and length.

The portfolio covers six marketing content types and uses Zero-Shot, One-Shot, Few-Shot, Role Prompting, Style Transfer, and the **RGCCO** framework (Role, Goal, Context, Constraints, Output Format).

## Objectives

- Draft and execute six naive prompts to establish baseline outputs.
- Build six optimized, parameter-driven prompt templates using the assigned techniques.
- Generate and review marketing content with ChatGPT.
- Evaluate Before vs After outputs on four quality dimensions using a 1–5 scale.
- Document the improvements and demonstrate the workflow in a 3–4 minute video.

## Content Types and Techniques

| Content type | Assigned prompt engineering technique |
| --- | --- |
| Blog Post | RGCCO + Style Transfer |
| LinkedIn Post | Role Prompting + Zero-Shot |
| Email Campaign | One-Shot Prompting |
| Instagram Caption | Few-Shot Prompting (3 examples) |
| YouTube Video Script | Role Prompting + RGCCO |
| Product Description | Few-Shot Prompting (2 examples) |

## Repository Structure

```text
prompt-engineering-hands-on/
├── README.md
├── prompt_library.md
├── generated_content.md
└── improvement_report.md
```

**Required files**

- `README.md` — Project introduction, objectives, setup and usage instructions, and Loom link.
- `prompt_library.md` — Six optimized prompts with editable parameters and techniques identified.
- `generated_content.md` — Final ChatGPT-generated outputs for all six content types.
- `improvement_report.md` — Before vs After comparison table and qualitative improvement reports for each task.

**Optional supporting file:** `before_prompts.txt` — Original naive prompts and baseline outputs.

## Prerequisites

- Access to [ChatGPT](https://chatgpt.com/) to execute the prompts.
- A text editor supporting Markdown (such as VS Code).
- A GitHub account for publishing the portfolio.
- Loom or another screen recorder for the demonstration video.
- Sample marketing topics, product details, and reference examples.

## How to Use the Prompt Library

1. Open `prompt_library.md` and select the template for the content you want to generate.
2. Review the technique and instructions attached to that template.
3. Replace placeholders such as `[Insert Topic]`, `[Insert Product/Offer]`, `[Insert Image Description]`, and `[Insert Specs]` with your own information.
4. For Style Transfer and Few-Shot templates, provide the required reference text or examples.
5. Copy the completed prompt into a new ChatGPT conversation and run it.
6. Review the response against the stated constraints, refine the prompt if necessary, and run it again.
7. Save the accepted output in `generated_content.md`.
8. Compare the output with the corresponding naive-prompt result and record the evaluation in `improvement_report.md`.

### Example Topics Used in the Assessment

- **Blog:** Why Remote Work Boosts B2B Software Engineering Efficiency
- **LinkedIn:** Learning prompt engineering
- **Email:** Apex Hydro 1-Liter Insulated Sport Bottle
- **Instagram:** Coffee cup image concept
- **YouTube:** 3 High-Income Skills You Can Self-Learn in 2026
- **Product description:** Wireless mouse specifications

These are sample topics; replace them as appropriate for your chosen marketing use case.

## Evaluation Method

Each naive (Before) and optimized (After) output is assessed on a scale from **1 (Poor) to 5 (Excellent)** in each category:

| Criterion | What to assess | Maximum score |
| --- | --- | ---: |
| Relevance | Alignment with the topic, audience, and goal | 5 |
| Tone | Suitability and consistency of writing style | 5 |
| Formatting | Compliance with the required structure | 5 |
| Length | Compliance with word-count and length requirements | 5 |
| **Total** | | **20** |

Record actual scores for all six tasks in `improvement_report.md`. For each task, explain the objective, the weakness of the naive prompt, the optimization strategy, and the observed quality difference. Scores should reflect the generated outputs rather than assumed improvements.

## Video Demonstration

**Loom video:** [Insert public Loom video URL]

The 3–4 minute walkthrough should cover:

1. Project overview and the six content types/techniques.
2. A walkthrough of `prompt_library.md`, including one complex prompt.
3. A live ChatGPT run using an optimized prompt with filled-in variables.
4. A review of the Before vs After quality comparison and closing summary.

Ensure the video is publicly accessible to assessors.

## Publishing to GitHub

From the project directory, run:

```bash
git init
git add .
git commit -m "Initialize Prompt Engineering Hands-On project"
git branch -M main
git remote add origin https://github.com/YOUR_USERNAME/prompt-engineering-hands-on.git
git push -u origin main
```

First create a **public** GitHub repository named `prompt-engineering-hands-on`. Replace `YOUR_USERNAME` with your GitHub username. Verify that the four required Markdown files display correctly on GitHub.

## Submission Checklist

- [ ] Six naive prompts executed and baseline outputs captured.
- [ ] Six optimized prompt templates saved in `prompt_library.md`.
- [ ] Six final outputs saved in `generated_content.md`.
- [ ] Before vs After scores completed for all six tasks.
- [ ] Six qualitative analyses included in `improvement_report.md`.
- [ ] Public Loom walkthrough recorded (3–4 minutes) and linked above.
- [ ] Four required Markdown files pushed to a public GitHub repository.
- [ ] GitHub and Loom links verified and submitted through the LMS.
- [ ] Submission description mentions challenges, resolutions, assumptions, and limitations, as applicable.

## Notes

This README documents the intended assessment workflow. Replace the placeholder name and URLs with your own details, and ensure the supporting files contain your actual prompts, generated outputs, and evaluation results before submitting.
