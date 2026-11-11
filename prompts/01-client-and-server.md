# Client and server

Some code runs in your customer's browser, where anyone can read and change it. Some runs on a server, where they can't. Prices, permissions and anything secret must be decided on the server.

## Check

Copy and paste this into your AI tool's chat.

```text
Review how my app is split between the browser (client) and the server.

Answer these questions:
1. List the main things the app does (for example: show products, place an order, apply a discount, send an email). For each one, say whether it runs in the browser or on a server.
2. Does any important decision happen only in the browser? For example: calculating a price, applying a discount, checking whether someone is an admin, or deciding what a user is allowed to see.
3. Could a customer change something in their browser (using the browser's developer tools) to get a lower price, see hidden data or skip a step?
4. Does the app talk to the database directly from the browser? If so, what stops someone from sending their own requests to it?
5. Is there anything that should move to a server function or backend, and why?

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
Move the important decisions from the browser to the server.

Rules for the fix:
- Fix one item at a time, starting with the most urgent.
- Before each change, tell me in one sentence what you are about to change and why.
- After each change, tell me how I can test it myself in the app.
- Do not change how the app looks or behaves for customers unless the fix needs it. If it does, tell me first.
- When you are done, run the check again and show me the new results.
- After the fix, the browser should only show information and send requests. Prices, permissions and anything secret should be decided on the server.
```

## What good looks like

- Prices, totals and discounts are calculated on the server.
- The server checks who the user is before doing anything for them.
- Changing something in the browser can't change what the server does.

[Back to all prompts](../README.md#the-prompts)
