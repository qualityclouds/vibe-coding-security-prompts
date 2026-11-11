# Personal data and GDPR

If your customers are in the EU or the UK, data protection law applies to you even if your app is small. Collect only what you need, protect it, and let people see and delete their data. This prompt is not legal advice.

## Check

Copy and paste this into your AI tool's chat.

```text
Review what personal data my app collects and how it handles it. My customers are in [country or region].

Answer these questions:
1. List every piece of personal data the app collects or stores: names, emails, phone numbers, addresses, payment details, location, photos, anything else.
2. For each one: why does the app need it? Is any of it more than the app needs?
3. Where is each piece stored, and in which country are those servers?
4. Which outside services receive personal data (analytics, email, AI models, payment providers)? What do they get?
5. Can a customer see the data I hold about them, and can they ask me to delete it? How would I do that today?
6. Is there a privacy notice, and does it match what the app really does?
7. Is any sensitive data collected (health, children, financial details)? If yes, flag it clearly.

Rules for your answer:
- Do not change any code yet. Only look and explain.
- Write for someone who is not a developer. No jargon without a one-line explanation.
- For each item, answer OK, Problem or Not sure.
- For every Problem or Not sure, give one sentence on what could go wrong for my customers and one sentence on what you would change.
- Finish with a short list of the changes you recommend, most urgent first.
- Remind me that this is not legal advice and tell me which points I should check with someone who knows data protection law.
```

## Fix

Paste this after the check, once you've read the answers.

```text
Fix the personal data problems you found.

Rules for the fix:
- Fix one item at a time, starting with the most urgent.
- Before each change, tell me in one sentence what you are about to change and why.
- After each change, tell me how I can test it myself in the app.
- Do not change how the app looks or behaves for customers unless the fix needs it. If it does, tell me first.
- When you are done, run the check again and show me the new results.
- Stop collecting anything the app does not need.
- Add a simple way for me to export and delete one customer's data.
- Draft a plain-English privacy notice that matches what the app really does, and mark it as a draft for me to check.
```

## What good looks like

- You know every piece of personal data you hold and why.
- You can delete one customer's data on request.
- Your privacy notice matches what the app does.

[Back to all prompts](../README.md#the-prompts)
