# Before go-live

Run this the day before you launch, and again before any big change.

## Check

Copy and paste this into your AI tool's chat.

```text
I am about to launch this app to real customers. Do a final review.

1. Re-check every topic: client and server, database access, log-in, secrets, forms, personal data, payments, backups, and cost limits. Mark each one OK, Problem or Not sure.
2. List anything that is still a Problem, most urgent first, and say whether it should stop the launch.
3. Check that the version customers will use has the right settings: live keys only on the server, test data removed, debug messages switched off.
4. Write a short summary I can send to a developer or my IT team so they can review the app quickly. Include what the app does, what data it holds, which services it uses, and any open problems.

Rules for your answer:
- Do not change any code yet. Only look and explain.
- Write for someone who is not a developer. No jargon without a one-line explanation.
- For each item, answer OK, Problem or Not sure.
- For every Problem or Not sure, give one sentence on what could go wrong for my customers and one sentence on what you would change.
- Finish with a short list of the changes you recommend, most urgent first.
```

## Fix

Paste this after the check, once you've read the answers.

```text
Fix the remaining launch blockers.

Rules for the fix:
- Fix one item at a time, starting with the most urgent.
- Before each change, tell me in one sentence what you are about to change and why.
- After each change, tell me how I can test it myself in the app.
- Do not change how the app looks or behaves for customers unless the fix needs it. If it does, tell me first.
- When you are done, run the check again and show me the new results.
```

[Back to all prompts](../README.md#the-prompts)
