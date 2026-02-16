# Week 05 CLI Prompt Log
 
## Tool + environment
- Tool: Gemini CLI
- Date/time: 2026-02-15 15:30:00 (approx)
- Repo/branch: https://github.com/mesrenyamedogbe/SOP / master
 
## Goal
- What I was trying to generate or change:
  The user wanted to create a GitHub repository for their project, push an existing `SOP v1.docx` document (converted to markdown), generate a Mermaid flowchart from the SOP, generate a BPMN 2.0 XML diagram from the SOP, and push all these artifacts, including a newly added image, to the GitHub repository.
 
## Inputs (files referenced)
- SOP-v1.md
- diagrams/mermaid/process.mmd
- diagrams/bpmn/process.bpmn


```
Create a file prompt-log/week05-cli-log.md and use the structure below to help record all the prompt log then wait for my validation: 

# Week 05 CLI Prompt Log 
 
## Tool + environment 
- Tool: [Claude Code / other] 
- Date/time: [timestamp] 
- Repo/branch: [main / feature-branch-name] 
 
## Goal 
- What I was trying to generate or change: 
 
## Inputs (files referenced) 
- SOP.md 
- diagrams/... 
 
## Prompt 
[Paste the exact prompt] 
 
## Output summary 
- Files created/modified: 
- What the tool produced (high-level): 
 
## Validation performed 
- What I checked (SOP alignment, decisions, start/end, exceptions): 
- What was wrong / missing: 
 
## Human edits I made 
- Specific changes I made after the tool output: 
 
## Result 
- Final files committed: 
- Commit hash (optional):
```

 
## Prompt2
1. `how can I create a GitHub Repository for this project?`
2. `here is my GitHub repo https://github.com/mesrenyamedogbe/SOP . Help me push the SOP v1 document to this repo as a .md file`
3. `Read SOP-v1.md and generate Mermaid flowchart code (flowchart TD) that matches the procedure exactly. - Include explicit Start and End. - Every decision has labeled branches. - Do NOT invent steps. If missing, mark as [TBD] as a note.`
4. `Read SOP-v1.md and generate Mermaid flowchart code (flowchart TD) that matches the procedure exactly. - Include explicit Start and End. - Every decision has labeled branches. - Do NOT invent steps. If missing, mark as [TBD] as a note.`
5. `Write the output to diagrams/mermaid/process.mmd. in the GitHub repository`
6. `I just added an image to the diagrams/mermaid/ foler, push it to GitHub.`
7. `Read SOP-v1.md, generate a BPMN 2.0 XML file for the process. - Start event + end event required. - Use tasks for steps, gateways for decisions. - Use lanes ONLY if roles differ materially. - Do NOT invent systems or approvals.`
8. `I just made some edits to the process.bpmn file. Check it out.`
9. `Create a file prompt-log/week05-cli-log.md and use the structure below to help record all the prompt log then wait for my validation: ...`
10. `gather all the prompts I have used and put them in the "prompt" section in the week05-cli-log.md file`
 
## Output summary
- Files created/modified:
    - SOP-v1.md (modified)
    - diagrams/mermaid/process.mmd (created)
    - diagrams/mermaid/image.png (created)
    - diagrams/bpmn/process.bpmn (created)
    - .gitignore (created)
    - prompt-log/week05-cli-log.md (created)
- What the tool produced (high-level):
    The tool initialized a git repository, added a remote GitHub repository, converted a user-provided .docx content to SOP-v1.md, generated a Mermaid flowchart (`process.mmd`), generated a BPMN 2.0 XML diagram (`process.bpmn`), handled git conflicts during pushes, created a `.gitignore` file, and pushed all these changes along with a new image to the GitHub repository.
 
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
