# Week 05 CLI Prompt Log
 
## Tools + environment
- Tools: Gemini CLI, Gemini, Mermaid.ai and Camunda.
- Environment: Visual Studio Code
- Date/time: 2026-02-15 15:30:00 (approx)
- Repo/branch: https://github.com/mesrenyamedogbe/SOP / master
 
## Goal
What I was trying to generate or change:
To create a GitHub repository for for an SOP project titled "Creating Beginner-Friendly Open Source Issues". The aim was to push an existing `SOP v1.docx` document (converted to markdown), generate a Mermaid flowchart from the SOP, generate a BPMN 2.0 XML diagram from the SOP, and push all these artifacts, including a two added images, to the GitHub repository.
 
## Inputs (files referenced)
- [SOP-v1.md](SOP-v1.md)

### Prompt 1:
`Read SOP-v1.md and generate Mermaid flowchart code (flowchart TD) that matches the procedure exactly. 
- Include explicit Start and End. 
- Every decision has labeled branches. 
- Do NOT invent steps. If missing, mark as [TBD] as a note.` 

#### Output summary 
- What the tool produced: [Mermaid Process](diagrams/mermaid/process.mmd)   
 
#### Validation performed 
- I checked that it aligned with the SOP
- Made sure that the start, decisions and end were correct. 
 
#### Human edits I made 
- Specific changes I made after the tool output: None 
 
#### Result: [Mermaid Process](diagrams/mermaid/process.mmd)



### Prompt 2:
Write the output to diagrams/mermaid/process.mmd. in the GitHub repository
 
#### Result: [Mermaid Process](diagrams/mermaid/process.mmd)


### Prompt 3:
`Read SOP-v1.md, generate a BPMN 2.0 XML file for the process. - Start event + end event required. 
- Use tasks for steps, gateways for decisions. 
- Use lanes ONLY if roles differ materially. 
- Do NOT invent systems or approvals.`

#### Output summary 
- What the tool produced: an xml code that was later refined using Gemini   
 
#### Validation performed 
- Used the xml code to generate the bpmn but it failed on my first and second try. Therefore I ran the code through Gemini to check for the errors, using this prompt: "I tried to run this xml code on bpmn.io but I faced an error. Check and rectify all the errors."
 
#### Result: [BPMN Process](diagrams/bpmn/process.bpmn)

 
## Output summary
- Files created/modified:
    - SOP-v1.md (modified)
    - diagrams/mermaid/process.mmd (created)
    - diagrams/mermaid/image.png (created)
    - diagrams/bpmn/process.bpmn (created)
    - diagrams/bpmn/process.png (created)
    - .gitignore (created)
    - prompt-log/week05-cli-log.md (created)
    - readme (created)
      
- What the tool produced (high-level):
    The tool converted a user-provided .docx content to SOP-v1.md, generated a Mermaid flowchart (`process.mmd`), generated a BPMN 2.0 XML code (`process.bpmn`), handled git conflicts during pushes, created a `.gitignore` file, and pushed these changes along with two new images to the GitHub repository.
 
 
## Results
- Final files committed:
    - [SOP-v1.md](SOP-v1.md)
    - [diagrams/mermaid/process.mmd](diagrams/mermaid/process.mmd)
    - [diagrams/mermaid/image.png](diagrams/mermaid/image.png)
    - [diagrams/bpmn/process.bpmn](diagrams/bpmn/process.bpmn)
    - [diagrams/bpmn/image.png](diagrams/bpmn/image.png)
    - [.gitignore](.gitignore)
    - [prompt-log/week05-cli-log.md](prompt-log/week05-cli-log.md)
    - [readme](prompt-log/week05-cli-log.md)
    - [glossary](Project_Glossary.md)

