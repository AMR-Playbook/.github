# Contributing to Kaduna AMR Watch

Thank you for helping. This project handles health data, so a few rules matter more here than in most repositories.

## Rules we never break

1. **Synthetic is never evidence.** Every output built from practice data says `SYNTHETIC`. Practice results never appear in a grant, report, post or conversation as a real finding.
2. **No identifiable patient data.** Names, phone numbers and addresses never enter any repository. Real patient IDs are hashed before loading. Follow the Nigeria Data Protection Act 2023.
3. **No percentage without its count.** Every number shown to anyone says how many isolates it's based on.
4. **No hidden changes.** Raw data is never edited. Every change to data is logged.
5. **Three tools, one number.** Your results must match the answer key (sheet `11_ANSWER_KEY` of the [Clean Handoff Pack](https://github.com/AMR-Playbook/.github/releases/tag/excel-handoff-v2)). If they don't, stop and find out why. Don't adjust a number to make it match.
6. **Say what we don't know.** Write uncertainty down. "We are not sure" is a professional sentence.
7. **Clinical decisions belong to clinicians.** We inform. We never give medical advice.

## Data

- The source data is the Excel squad's **Clean Handoff Pack v2**, published as a [release](https://github.com/AMR-Playbook/.github/releases/tag/excel-handoff-v2). Download it. **Don't commit it, or any data file, to a repository.**
- Sheets `4_ISOLATES` and `5_AST_RESULTS` are read-only source. Load them, don't change them.
- Never commit passwords, connection strings or `.env` files.

## How work flows

1. Pick an open issue. Comment that you're taking it, and assign yourself.
2. Create a branch: `area/short-description`, for example `views/antibiogram`.
3. Before asking for help, write three lines in the issue: what you're trying to do, what you tried, and what happened.
4. Open a pull request that links the issue (`Closes #12`). Fill in the checklist.
5. **Every pull request is reviewed by someone from a different squad** before it's merged. Reviewing work in a tool you don't know yet is how you learn it.

## Labels

| Label | Meaning |
|---|---|
| `must-have` | Required for the project to be finished |
| `answer-key` | Output must match sheet `11_ANSWER_KEY` |
| `privacy` | Touches patient privacy or access control |
| `clinical-safety` | Could mislead a clinician if done wrongly |
| `documentation` | The deliverable is a document |
| `good first issue` | A sensible place to start |

Milestones mark the two checkpoints: **Check 1 — Three tools, one number** and **Check 2 — Rebuild from zero & final demo**.
