# Week 05 CLI Prompt Log
 
## Tool + environment
- Tools: Gemini CLI, Gemini, Mermaid.ai and Camunda.
- Environment: Visual Studio Code
- Date/time: 2026-02-15 15:30:00 (approx)
- Repo/branch: https://github.com/mesrenyamedogbe/SOP / master
 
## Goal
- What I was trying to generate or change:
  To create a GitHub repository for for an SOP project titled "Creating Beginner-Friendly Open Source Issues". The aim was to push an existing `SOP v1.docx` document (converted to markdown), generate a Mermaid flowchart from the SOP, generate a BPMN 2.0 XML diagram from the SOP, and push all these artifacts, including a two added images, to the GitHub repository.
 
## Inputs (files referenced)
- SOP-v1.md


```
### Prompt 1:
`Read SOP-v1.md and generate Mermaid flowchart code (flowchart TD) that matches the procedure exactly. 
- Include explicit Start and End. 
- Every decision has labeled branches. 
- Do NOT invent steps. If missing, mark as [TBD] as a note.` 

### Output summary 
- What the tool produced:   
 
### Validation performed 
- I checked that it aligned with the SOP
- Made sure that the start, decisions and end were correct 
 
### Human edits I made 
- Specific changes I made after the tool output: 
 
### Result 


```

```
### Prompt 2:
 `Write the output to diagrams/mermaid/process.mmd. in the GitHub repository`
 
### Result

```


```
### Prompt 3:
`Read SOP-v1.md, generate a BPMN 2.0 XML file for the process. - Start event + end event required. 
- Use tasks for steps, gateways for decisions. 
- Use lanes ONLY if roles differ materially. 
- Do NOT invent systems or approvals.`

### Output summary 
- What the tool produced: an xml code that was later refined using Gemini   
 
### Validation performed 
- Used the xml code to generate the bpmn but failed. Therefore I ran the code through Gemini to check for changes. 
 
 
### Result


```
 
## Output summary
- Files created/modified:
    - SOP-v1.md (modified)
    - diagrams/mermaid/process.mmd (created)
    - diagrams/mermaid/image.png (created)
    - diagrams/bpmn/process.bpmn (created)
    - .gitignore (created)
    - prompt-log/week05-cli-log.md (created)
- What the tool produced (high-level):
    The tool initialized a git repository, added a remote GitHub repository, converted a user-provided .docx content to SOP-v1.md, generated a Mermaid flowchart (`process.mmd`), generated a BPMN 2.0 XML diagram (`process.bpmn`), handled git conflicts during pushes, created a `.gitignore` file, and pushed all these changes along with two new images to the GitHub repository.
 
## Validation performed
- What I checked (SOP alignment, decisions, start/end, exceptions):
[Please fill this section after your validation]

- What was wrong / missing:
[Please fill this section after your validation]
 
## Human edits I made
- Specific changes I made after the tool output:
[Please fill this section after your validation]
 
## Result
- Final files committed:
    - SOP-v1.md
    - diagrams/mermaid/process.mmd
    - diagrams/mermaid/image.png
    - diagrams/bpmn/process.bpmn
    - .gitignore
    - prompt-log/week05-cli-log.md
- Commit hash (optional): fd102f2 (last commit for BPMN update)
