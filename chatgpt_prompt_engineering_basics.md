# ChatGPT Basics and Foundational Prompt Engineering

**Project:** Prompt Engineering Basics\
**Prepared by:** \[Your Name\]\
**Purpose:** Complete the five foundational prompt exercises and
document the setup, prompt log, recording, and GitHub submission
workflow.

> **Before submitting:** Replace `[Your Name]`, add your own Loom share
> URL to `README.md`, and capture the actual outputs returned by your
> ChatGPT session if your assessor requires raw session outputs.

## Exercise 1 --- Register a ChatGPT Account and Understand the Interface

### Task

Register a free ChatGPT account, verify the email address, and identify
the Sidebar, New Chat button, and Settings.

### Setup steps

1.  Open a browser and visit <https://chatgpt.com/>.
2.  Select **Sign up** and register with an email address, or continue
    with an existing Google, Microsoft, or Apple account.
3.  If registering by email, create a secure password and follow the
    verification instructions sent to your inbox.
4.  Complete any requested profile details and phone verification, if
    prompted.
5.  Confirm that the ChatGPT main chat screen appears.
6.  Locate the Sidebar, conversation history, **New Chat** button, and
    profile menu/settings.
7.  Select **New Chat** to begin with a clean conversation.

**Verification:** The ChatGPT main chat screen is accessible and the key
interface elements have been located.

## Exercise 2 --- Execute the Five Foundational Prompts

The following prompts are ready to run. Example outputs are provided for
reference; replace them with the raw outputs from your own ChatGPT
session if required.

### Task 1: Text Summarization

#### Prompt Input

``` text
Summarize the text below in exactly three bullet points.

Text: "Remote work has rapidly expanded, introducing both opportunities and obstacles for modern businesses..."
```

#### Example ChatGPT Output

-   Remote work has expanded and created new opportunities for
    businesses.
-   It can offer flexibility and reduce some workplace constraints.
-   Businesses may also need to address collaboration, communication,
    and employee-engagement challenges.

**Note:** The source text supplied in the exercise is abbreviated with
an ellipsis, so this output is illustrative rather than a summary of a
complete passage.

### Task 2: Information Extraction

#### Prompt Input

``` text
Extract the customer's name, email address, and order ID from the support request below.

Support Request: "Hello FlexTime, my name is John Doe (john.doe@email.com). I haven't received my shipment updates for order FT-99881. Please check."
```

#### Example ChatGPT Output

-   **Customer name:** John Doe
-   **Email address:** john.doe@email.com
-   **Order ID:** FT-99881

### Task 3: Formatting Conversion

#### Prompt Input

``` text
Convert the list of product prices below into a markdown table with two columns: "Item" and "Price".

List:
- Wireless Mouse: $25.00
- Ergonomic Keyboard: $70.00
- Insulated Water Bottle: $18.00
```

#### Example ChatGPT Output

  Item                         Price
  ------------------------ ---------
  Wireless Mouse             \$25.00
  Ergonomic Keyboard         \$70.00
  Insulated Water Bottle     \$18.00

### Task 4: Tone Editing

#### Prompt Input

``` text
Act as an Editor. Rewrite the draft text below to sound like a professional, polite B2B email sent to a client.

Draft: "hey, sorry we are late on the report. it had bugs. we will send it tomorrow. thanks."
```

#### Example ChatGPT Output

**Subject: Update on Report Delivery**

Dear \[Client Name\],

I apologize for the delay in delivering the report. We identified a few
issues that required additional attention, and we are working to resolve
them. We expect to send the completed report tomorrow.

Thank you for your patience and understanding.

Best regards,\
\[Your Name\]

### Task 5: Constraint-Driven Output

#### Prompt Input

``` text
Summarize the sentence below in under 20 words. Do not use the word "help" or "assist".

Sentence: "Our customer success managers are available 24 hours a day to guide new users and resolve technical account disputes."
```

#### Example ChatGPT Output

Customer success managers are available 24/7 to guide new users and
resolve technical account disputes.

## Exercise 3 --- Create the Basic Prompt Log Portfolio File

### Task

Save all five prompt inputs and outputs in a Markdown file named
`basic_prompt_log.md`.

### Suggested project structure

``` text
prompt-engineering-basics/
├── basic_prompt_log.md
└── README.md
```

### Checklist

-   [ ] Use a top-level title and headings for all five tasks.
-   [ ] Include a **Prompt Input** and **ChatGPT Output** section for
    each task.
-   [ ] Put prompt text in fenced code blocks.
-   [ ] Keep a blank line before Markdown tables.
-   [ ] Review all five entries for completeness.
-   [ ] If raw outputs are required, replace the illustrative outputs
    above with the exact responses from your own session.

## Exercise 4 --- Record and Share a Loom Presentation

### Task

Record a 1.5--2.5-minute video showing the ChatGPT workspace and a live
prompt execution.

### Recording timeline

-   **0:00--0:30:** Introduce yourself and state that you are validating
    Lesson 1: ChatGPT Basics.
-   **0:30--1:00:** Show the ChatGPT workspace and profile/settings
    menu. Avoid exposing passwords or other sensitive information.
-   **1:00--2:00:** Open `basic_prompt_log.md`, copy Prompt 1, paste it
    into ChatGPT, submit it, and show the result.
-   **2:00--2:15:** Thank the viewer, stop the recording, and copy the
    Loom share link.

### Sharing checklist

1.  Visit <https://www.loom.com/> and sign in.
2.  Start a screen recording and configure webcam options as desired.
3.  Record the walkthrough using the timeline above.
4.  Set access to **Anyone with the link can view**, if that option is
    available for your account.
5.  Copy the share URL and add it to `README.md`.

**Loom share URL:** `[Paste your public Loom URL here]`

## Exercise 5 --- Organize Deliverables and Push to GitHub

### Task

Create a local project folder, add `basic_prompt_log.md` and
`README.md`, initialize Git, and push the project to a public GitHub
repository.

### README template

``` markdown
# Prompt Engineering Basics

**Name:** [Your Name]

## Overview
This project documents five foundational ChatGPT prompting exercises:
summarization, information extraction, formatting conversion, tone editing,
and constraint-driven output.

## Loom Presentation
[Watch the presentation](PASTE_YOUR_PUBLIC_LOOM_URL_HERE)

## Files
- `basic_prompt_log.md` — prompts and example outputs for all five exercises.
```

### Git commands

Run these commands from inside the `prompt-engineering-basics` folder.
Replace `YOUR_USERNAME` with your GitHub username.

``` bash
git init
git add .
git commit -m "Initialize Prompt Engineering Basics project"
git branch -M main
git remote add origin https://github.com/YOUR_USERNAME/prompt-engineering-basics.git
git push -u origin main
```

If Git reports that the remote already exists, update it with
`git remote set-url origin https://github.com/YOUR_USERNAME/prompt-engineering-basics.git`.

### Final verification checklist

-   [ ] The GitHub repository is set to **Public**.
-   [ ] `basic_prompt_log.md` and `README.md` appear in the repository.
-   [ ] The README contains the correct public Loom URL.
-   [ ] The Loom URL opens without requiring the assessor to sign in.
-   [ ] The repository can be viewed in a private/incognito browser
    window.

## Submission Deliverables

1.  `basic_prompt_log.md` --- prompt inputs and outputs.
2.  `README.md` --- project overview and Loom URL.
3.  Public GitHub repository URL.
4.  Public Loom presentation URL.

**Important:** This document provides example outputs and templates. It
does not create a ChatGPT account, record a Loom video, or publish a
GitHub repository on your behalf.
