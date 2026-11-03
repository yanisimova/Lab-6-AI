# Lab 6 — Emerging Technology Adoption Agent

This is a specialist agent folder designed to be copied into `MASY1800_ET_Agent_Scaffold_v1_0-2/agents/adoption_agent/` in the existing course scaffold. **Do not replace or edit frozen core.**

## Run with the course scaffold
From the scaffold root:

```bash
python tools/check_frozen_core.py
python tools/build_prompt.py --agent agents/adoption_agent --case agents/adoption_agent/cases/primary.json
python tools/build_prompt.py --agent agents/adoption_agent --case agents/adoption_agent/cases/contrast.json
python tools/build_prompt.py --agent agents/adoption_agent --case agents/adoption_agent/cases/qualification.json
python tools/validate_response.py agents/adoption_agent/responses/primary_response.json
python tools/validate_response.py agents/adoption_agent/responses/contrast_response.json
python tools/validate_response.py agents/adoption_agent/responses/qualification_response.json
```

Prompt packets should be sent to ChatGPT; responses saved and validated again. Bundled response files are illustrative test responses, **not evidence of live execution**. Verify factual claims and thresholds before any actual management use.

## GitHub and submission
Copy `agents/adoption_agent` into the scaffold, commit it, and record the actual branch/commit in the Word Agent Record. GitHub write access was denied (HTTP 403), so these files are **not uploaded** to the repository.
