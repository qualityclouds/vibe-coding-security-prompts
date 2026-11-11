# Screens and forms

Everything a person types into your app can be wrong, huge or harmful. Your forms should check it, and your error messages should help customers without telling attackers how the app works.

## Check

Copy and paste this into your AI tool's chat.

```text
Review the screens and forms in my app.

Answer these questions:
1. List every form and input field. For each one, what does it accept, and what does it reject?
2. Is the input checked on the server as well as in the browser? (Checks in the browser alone can be skipped.)
3. Could someone type something that breaks the page, shows up as code on another user's screen, or changes a database query?
4. Can people upload files? What types and sizes are allowed, and where are the files stored? Can other users see them?
5. What do error messages show? Do any of them reveal technical details, database names or other users' information?
6. Does any screen show more data than that user should see, even if it is hidden on the page?
7. Can the app be used with a keyboard only, and does it work on a phone?

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
Fix the form and screen problems you found.

Rules for the fix:
- Fix one item at a time, starting with the most urgent.
- Before each change, tell me in one sentence what you are about to change and why.
- After each change, tell me how I can test it myself in the app.
- Do not change how the app looks or behaves for customers unless the fix needs it. If it does, tell me first.
- When you are done, run the check again and show me the new results.
- Check every input on the server, not only in the browser.
- Error messages for customers should be short and friendly and must not include technical details. Log the details where only I can see them.
```

## What good looks like

- Every input is checked on the server.
- Uploaded files are limited by type and size, and private files stay private.
- Error messages help the customer and reveal nothing about how the app is built.

[Back to all prompts](../README.md#the-prompts)
