# Regulatory Change Agent

A Microsoft Copilot Studio agent that compares two editions of AER Directive 071 (Feb 2023 and Dec 2025), maps each change to a company's procedures and requirements, drafts change requests, and routes them for human approval in Microsoft Teams, with every decision recorded in SharePoint.

**Case study:** https://avinashkavirajan.github.io/regulatory-change-agent/

## What it does
1. Analyses a company procedure against the new Directive and lists changed requirements and new obligations, with citations.
2. Drafts a change request in the company template.
3. Asks for confirmation, then saves the request to SharePoint and starts a Teams approval (Power Automate).
4. Records the approver's decision, name, date and comments as an audit trail.

## Results (3 runs x 6 procedures, scored against a hand-built answer key)
| Measure | Result |
|---|---|
| Found the right new clause | 92% |
| Chose the right change type | 71% |
| Trap questions handled | 6 of 6 |
| Function and safety tests | 14 of 16 passed, 0 failed |

## Built with
Microsoft Copilot Studio · SharePoint Online · Power Automate · Microsoft Teams Approvals

## Files
- `index.html`: the case study page (served by GitHub Pages)
- `agent-instructions.txt`: the agent's full instructions
- `1.png` to `12.png`: stills from the demo; `demo.mp4`: the demo video

Prairie Ridge Energy is a fictional company created for this project. Directive 071 is a public document from the Alberta Energy Regulator; this project is not affiliated with the AER.
