# Cost and abuse

Apps that call AI models, send emails or text messages can run up big bills if a bot finds them. A few limits stop most of it.

## Check

Copy and paste this into your AI tool's chat.

```text
Review whether my app can be abused or run up unexpected costs.

Answer these questions:
1. List every action in the app that costs me money each time it runs (AI calls, emails, text messages, map lookups, file storage).
2. Can someone who is not logged in trigger any of them?
3. Is there any limit on how often one user or one visitor can trigger them? What would happen if a bot did it 10,000 times in an hour?
4. Do my forms have anything to stop bots (for example a captcha or rate limit) on sign-up, contact and password reset?
5. Have I set spending limits or alerts in each paid service?
6. Could someone use my app to send spam to other people, for example through a contact or invite form?

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
Add limits so the app cannot be abused or run up surprise bills.

Rules for the fix:
- Fix one item at a time, starting with the most urgent.
- Before each change, tell me in one sentence what you are about to change and why.
- After each change, tell me how I can test it myself in the app.
- Do not change how the app looks or behaves for customers unless the fix needs it. If it does, tell me first.
- When you are done, run the check again and show me the new results.
- Add rate limits on the server for every action that costs money or sends messages.
- Add bot protection to sign-up, contact and password reset forms.
- Tell me where to set spending limits and alerts in each paid service.
```

## What good looks like

- Every paid action has a limit per user.
- Public forms have bot protection.
- Every paid service has a spending alert.

[Back to all prompts](../README.md#the-prompts)
