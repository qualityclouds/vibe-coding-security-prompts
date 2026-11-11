# Secrets and API keys

API keys are like passwords for the services your app uses: payments, email, AI models. If a key ends up in the browser, anyone can copy it and use it on your bill.

## Check

Copy and paste this into your AI tool's chat.

```text
Review how my app stores and uses secrets: API keys, passwords, tokens and connection strings.

Answer these questions:
1. List every external service the app uses (for example Stripe, OpenAI, an email service, a maps service) and every key or secret it needs.
2. For each secret: where is it stored? Is it in a code file, an environment variable, or the tool's secrets panel?
3. Which of these secrets end up in the code that runs in the browser? Explain how someone could find them.
4. Which keys are meant to be public (some services have a public key for the browser and a secret key for the server)? Confirm the secret ones are only used on the server.
5. Has any secret ever been written into a file that is saved to GitHub? If so, it should be treated as leaked even if it was deleted later.

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
Move every secret out of the browser and out of the code.

Rules for the fix:
- Fix one item at a time, starting with the most urgent.
- Before each change, tell me in one sentence what you are about to change and why.
- After each change, tell me how I can test it myself in the app.
- Do not change how the app looks or behaves for customers unless the fix needs it. If it does, tell me first.
- When you are done, run the check again and show me the new results.
- Store secrets in the tool's secrets or environment settings, never in code files.
- Any call that needs a secret key must happen on the server.
- Give me a list of every key that was exposed, so I can create new ones in each service and delete the old ones. Tell me where to do that for each service.
```

## What good looks like

- No secret key appears in the code that runs in the browser.
- Secrets live in the tool's secrets settings.
- Any key that was ever exposed has been replaced.

[Back to all prompts](../README.md#the-prompts)
