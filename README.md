# Standard Operating Procedure for Creating Beginner-Friendly Open Source Issues

This readme provides instructions on how to regenerate the documentation artifacts in this repository.

Before we start, the repository contains the documentation and process models for a Standard Operating Procedure (SOP) on "Creating Beginner-Friendly Open Source Issues". It is a non-code project focused on documenting a process for open-source maintainers. The repository includes the SOP itself, visual diagrams of the process in Mermaid and BPMN formats, and a log of the prompts used to generate these artifacts.

## Usage
This repository serves as a reference for open-source maintainers who want to create a welcoming environment for new contributors. The `SOP-v1.md` file can be used as a guide for creating "good first issues". The diagrams in the `diagrams` directory can be used to visualize and understand the process. The `prompt-log` can be used as a learning resource for using the Gemini CLI for similar documentation and process modeling tasks.

## Artifacts
This repository contains the following documentation artifacts:

-   **`SOP-v1.md`**: The main Standard Operating Procedure document. It outlines the purpose, scope, roles, and a step-by-step process for creating beginner-friendly issues on GitHub.
-   **`diagrams/mermaid/process.mmd`**: A Mermaid flowchart that provides a simple visual representation of the process described in `SOP-v1.md`. An image of the Mermaid diagram is also available at `diagrams/mermaid/image.png`.
-   **`diagrams/bpmn/process.bpmn`**: A BPMN 2.0 XML file that provides a more formal and detailed model of the process, including lanes for roles and gateways for decisions. An image of the BPMN diagram is also available at `diagrams/bpmn/image.png`.
-   **`prompt-log/week05-cli-log.md`**: A detailed log of the prompts and interactions with the Gemini CLI that were used to generate the artifacts in this repository. This file is useful for understanding the history of the project and for regenerating the artifacts.

## Regeneration Instructions

### Prerequisites
-   Gemini CLI installed and configured.
-   `git` installed and configured.
-   A work environment of your choice (I used VS Code)

### 1. SOP-v1.md
To regenerate `SOP-v1.md`, you need to define 


### 2. diagrams/mermaid/process.mmd
To regenerate the Mermaid flowchart code, use the following prompt with the Gemini CLI:

```
Read SOP-v1.md and generate Mermaid flowchart code (flowchart TD) that matches the procedure exactly.
- Include explicit Start and End.
- Every decision has labeled branches.
- Do NOT invent steps. If missing, mark as [TBD] as a note.
```

Then, write the output to `diagrams/mermaid/process.mmd`.

### 3. diagrams/mermaid/image.mmd
To regenerate the Mermaid flowchart, use Mermaid.ai to generate the flowchart using the code.


### 4. diagrams/bpmn/process.bpmn
To regenerate the BPMN 2.0 XML file, use the following prompt with the Gemini CLI:

```
Read SOP-v1.md, generate a BPMN 2.0 XML file for the process.
- Start event + end event required.
- Use tasks for steps, gateways for decisions.
- Use lanes ONLY if roles differ materially.
- Do NOT invent systems or approvals.
```

Then, write the output to `diagrams/bpmn/process.bpmn`.

### 5. diagrams/bpmn/image.mmd
To regenerate the BPMN image, use Camunda to generate it using the .xml code that was generated.


### 6. prompt-log/week05-cli-log.md
Ensure that you keep a prompt log to capture your process as seen in the prompt-log
```
