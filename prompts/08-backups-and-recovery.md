# Backups and recovery

Things go wrong: a bad change, a deleted table, a service outage. Find out now whether you can recover, before you need to.

## Check

Copy and paste this into your AI tool's chat.

```text
Review whether my app's data can be recovered if something goes wrong.

Answer these questions:
1. Is the database backed up automatically? How often, and how long are backups kept? Does my current plan include backups?
2. If I deleted a table by mistake right now, what exactly would I do to get it back, and how much data would I lose?
3. Are uploaded files (images, documents) backed up too?
4. Is the app's code saved somewhere outside the AI tool, for example on GitHub?
5. If the app breaks after a change, how do I go back to the last working version?
6. Is there a test or preview version of the app, separate from the one customers use, where I can try changes first?

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
Set up the missing backup and recovery steps.

Rules for the fix:
- Fix one item at a time, starting with the most urgent.
- Before each change, tell me in one sentence what you are about to change and why.
- After each change, tell me how I can test it myself in the app.
- Do not change how the app looks or behaves for customers unless the fix needs it. If it does, tell me first.
- When you are done, run the check again and show me the new results.
- Where a backup depends on my plan or a setting I have to change, tell me exactly where to click.
- Write me a one-page recovery note: what to do, step by step, if data is lost or the app breaks.
```

## What good looks like

- Backups run automatically and you know how to restore one.
- Your code is saved outside the AI tool.
- You have a one-page recovery note.

[Back to all prompts](../README.md#the-prompts)
