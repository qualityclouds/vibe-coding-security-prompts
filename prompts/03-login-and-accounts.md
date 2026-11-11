# Log-in and accounts

If your app shows anything personal, people need to log in. And log-in alone isn't enough: the app also has to check what each user is allowed to do.

## Check

Copy and paste this into your AI tool's chat.

```text
Review sign-up, log-in and user permissions in my app.

Answer these questions:
1. How do people sign up and log in? Which service handles it?
2. Which pages or features can someone use without logging in? Should any of them require log-in?
3. Are there different kinds of users, such as customer, staff or admin? Where in the code is that decided, and is it checked on the server?
4. Could a normal user make themselves an admin, or reach an admin page by typing its address?
5. Is email confirmation switched on? Can someone sign up with an email address they don't own?
6. How does password reset work? Could someone reset another person's password?
7. What happens when a user logs out? Is their session really ended?

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
Fix the log-in and permission problems you found.

Rules for the fix:
- Fix one item at a time, starting with the most urgent.
- Before each change, tell me in one sentence what you are about to change and why.
- After each change, tell me how I can test it myself in the app.
- Do not change how the app looks or behaves for customers unless the fix needs it. If it does, tell me first.
- When you are done, run the check again and show me the new results.
- Use the log-in service the app already has. Do not build a custom password system.
- Every page and every server function that shows or changes private data must check who the user is and what they are allowed to do.
```

## What good looks like

- Private pages and data need log-in.
- Roles like admin are checked on the server.
- Typing an admin page's address as a normal user gets you nowhere.

[Back to all prompts](../README.md#the-prompts)
