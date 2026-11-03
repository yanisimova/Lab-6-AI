# Assignment 6 — upload instructions

This ZIP contains the **actual specialist agent files** nested under the correct GitHub scaffold path.

1. Extract this ZIP on your computer.
2. In GitHub, open `MASY1800_ET_Agent_Scaffold_v1_0-2/agents/` on branch `main`.
3. Use **Add file → Upload files**. Drag the extracted **`adoption_agent` folder** from inside the ZIP (not just the README files) into the upload area. If GitHub does not preserve the folder, drag all files/folders from inside `adoption_agent` while you are at `agents/adoption_agent/`.
4. Commit. Confirm these paths exist:
   - `MASY1800_ET_Agent_Scaffold_v1_0-2/agents/adoption_agent/agent_metadata.json`
   - `MASY1800_ET_Agent_Scaffold_v1_0-2/agents/adoption_agent/specialist_instructions.md`
   - `MASY1800_ET_Agent_Scaffold_v1_0-2/agents/adoption_agent/cases/primary.json`
   - `MASY1800_ET_Agent_Scaffold_v1_0-2/agents/adoption_agent/responses/primary_response.json`
5. Run from the scaffold root: `python tools/check_frozen_core.py`.
6. Build each prompt with `python tools/build_prompt.py --agent agents/adoption_agent --case agents/adoption_agent/cases/primary.json` (repeat with `contrast.json` and `qualification.json`).
7. Submit each generated prompt to ChatGPT, save its actual JSON output, then run `python tools/validate_response.py agents/adoption_agent/responses/primary_response.json` (repeat for contrast and qualification).
8. Update the Word Agent Record with your actual branch, commit and test evidence before submission.

The bundled response JSON files are **illustrative**, not proof of fresh agent executions. The agent is prompt-based and uses ChatGPT as runtime; it is not a standalone API application. Do not change frozen `core/` files.
