# MATACS-TH-2026-02: AI Proposal Triage Design

**Name:** Abdul Haq
**Reference:** MATACS-TH-2026-02
**Time actually spent:** Approximately 2 hours

## Summary

A design for an AI-assisted proposal triage tool. The principle is **AI reads, code decides, humans approve**: AI only extracts facts (and checks a team checklist) from proposal text, while pass/fail, scoring and ranking are plain code, and a human makes the final award decision.

## Files

| File | Contents |
|---|---|
| [WRITEUP.md](WRITEUP.md) | Answers to the five questions |
| [PROMPTS.md](PROMPTS.md) | The two AI prompts (fact extraction, team checklist) |
| [ranking.json](ranking.json) | Expected ranking of proposals A to E |
| [diagram/Matacs.jpg](diagram/Matacs.jpg) | Process-flow diagram from upload to ranked output |

No prototype is included.

## Sample result

A ranked 1st and E ranked 2nd. C and D are flagged for human review (C for a hidden instruction aimed at automated review, D for a missing timeline). B is ineligible (licence not held by the bidder). Please check the `ranking.json` file.

## How I used AI tools

Used Claude Sonnet 5.5 to mainly enhance my design and confirm whether the answers I wrote for myself for the 5 questions asked are fulfilling the criteria and the design, and properly format the .md files. Claude insisted on using AI for scoring the proposals. I disagreed on this and thought of suggesting some kind of ranking formula because AI can hallucinate in calculating complex mathematical equations but the calculations being done in the code will always give same accurate result.