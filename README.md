# SOP Documentation Regeneration

This document provides instructions on how to regenerate the documentation artifacts in this repository.

## Prerequisites

-   [Gemini CLI](https://github.com/google/gemini-cli) installed and configured.
-   `git` installed and configured.

## Artifacts

This repository contains the following documentation artifacts:

-   `SOP-v1.md`: The Standard Operating Procedure in Markdown format.
-   `diagrams/mermaid/process.mmd`: A Mermaid flowchart of the SOP.
-   `diagrams/bpmn/process.bpmn`: A BPMN 2.0 XML representation of the SOP.
-   `prompt-log/week05-cli-log.md`: A log of the prompts used to generate the artifacts.

## Regeneration Instructions

### 1. SOP-v1.md

To regenerate `SOP-v1.md`, you need the original `SOP v1.docx` file. Since the `.docx` file is not in this repository, this step is not fully reproducible from the repository content alone. However, if you have the content of the `.docx` file, you can use the following prompt with the Gemini CLI:

```
here is my GitHub repo https://github.com/mesrenyamedogbe/SOP . Help me push the SOP v1 document to this repo as a .md file

[Paste the content of the SOP v1.docx file here]
```

### 2. diagrams/mermaid/process.mmd

To regenerate the Mermaid flowchart, use the following prompt with the Gemini CLI:

```
Read SOP-v1.md and generate Mermaid flowchart code (flowchart TD) that matches the procedure exactly.
- Include explicit Start and End.
- Every decision has labeled branches.
- Do NOT invent steps. If missing, mark as [TBD] as a note.
```

Then, write the output to `diagrams/mermaid/process.mmd`.

### 3. diagrams/bpmn/process.bpmn

To regenerate the BPMN 2.0 XML file, use the following prompt with the Gemini CLI:

```
Read SOP-v1.md, generate a BPMN 2.0 XML file for the process.
- Start event + end event required.
- Use tasks for steps, gateways for decisions.
- Use lanes ONLY if roles differ materially.
- Do NOT invent systems or approvals.
```

Then, write the output to `diagrams/bpmn/process.bpmn`.

### 4. prompt-log/week05-cli-log.md

To regenerate the prompt log, use the following prompt with the Gemini CLI:

```
Create a file prompt-log/week05-cli-log.md and use the structure below to help record all the prompt log then wait for my validation:

[Paste the template from the original prompt here]
```

Then, to update the prompt log with all the prompts used, use the following prompt:

```
gather all the prompts I have used and put them in the "prompt" section in the week05-cli-log.md file
```
