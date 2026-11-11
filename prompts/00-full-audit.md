# Full audit

Start here. This prompt checks the basics across every topic and tells you which detailed prompts to run next.

## Check

Copy and paste this into your AI tool's chat.

```text
I built this app with AI and I am not a developer. Before real customers use it, I want an honest review of whether it is safe.

Look at the whole project and answer these questions:
1. Where is customer data stored? Is it in a real database, or only in the browser?
2. Which parts of the app run in the customer's browser, and which run on a server?
3. Do customers have to log in? Can one customer see or change another customer's data?
4. Are any API keys, passwords or tokens visible in the code or in the browser?
5. Is the database protected so that only allowed users can read and write each record?
6. Do the forms check what people type in before it is saved?
7. What personal data does the app collect, and is any of it more than it needs?
8. If the data were deleted today, could it be recovered?
9. Could a bot or a stranger run up costs, for example by calling an AI or email service thousands of times?
10. Is there anything else a security-minded developer would worry about before launch?

Rules for your answer:
- Do not change any code yet. Only look and explain.
- Write for someone who is not a developer. No jargon without a one-line explanation.
- For each item, answer OK, Problem or Not sure.
- For every Problem or Not sure, give one sentence on what could go wrong for my customers and one sentence on what you would change.
- Finish with a short list of the changes you recommend, most urgent first.
- At the end, tell me which of these topics need a deeper look: client and server, database, log-in, secrets, screens and forms, personal data, payments, backups, cost and abuse.
```

## Fix

Paste this after the check, once you've read the answers.

```text
Fix the problems you found in the audit.

Rules for the fix:
- Fix one item at a time, starting with the most urgent.
- Before each change, tell me in one sentence what you are about to change and why.
- After each change, tell me how I can test it myself in the app.
- Do not change how the app looks or behaves for customers unless the fix needs it. If it does, tell me first.
- When you are done, run the check again and show me the new results.
```

[Back to all prompts](../README.md#the-prompts)
