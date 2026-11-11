# Payments

When money is involved, the browser must never decide the price, and your app must only treat an order as paid when the payment provider confirms it.

## Check

Copy and paste this into your AI tool's chat.

```text
Review how my app handles payments.

Answer these questions:
1. Which payment provider does the app use? Walk me through what happens, step by step, from clicking Pay to the order being marked as paid.
2. Where is the price calculated? Could a customer change the price, quantity or discount in their browser?
3. How does the app know a payment succeeded? Does it wait for a confirmation from the payment provider (often called a webhook), or does it trust the browser?
4. Could someone get an order marked as paid without paying, or pay once and get two orders?
5. Are card details ever stored by my app, or does the payment provider handle them?
6. Is the app using test keys or live keys, and are the live secret keys only on the server?
7. What happens with refunds and failed payments?

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
Fix the payment problems you found.

Rules for the fix:
- Fix one item at a time, starting with the most urgent.
- Before each change, tell me in one sentence what you are about to change and why.
- After each change, tell me how I can test it myself in the app.
- Do not change how the app looks or behaves for customers unless the fix needs it. If it does, tell me first.
- When you are done, run the check again and show me the new results.
- Prices and totals must be calculated on the server from the product data, never taken from the browser.
- Mark an order as paid only after the payment provider confirms it to the server.
- Never store card details in my app.
```

## What good looks like

- Prices come from the server.
- Orders are marked paid only after the provider confirms it.
- Card details never touch your database.

[Back to all prompts](../README.md#the-prompts)
