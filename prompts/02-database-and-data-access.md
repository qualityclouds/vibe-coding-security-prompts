# Database and data access

The most common problem in AI-built apps is a database that answers anyone who asks. If your app uses Supabase or Firebase, the protection is a setting you have to switch on and configure.

## Check

Copy and paste this into your AI tool's chat.

```text
Review how my app stores data and who can read or change it.

Answer these questions:
1. What database does the app use? List every table (or collection) and say in one line what it stores.
2. For each table: can someone who is not logged in read it? Can a logged-in user read rows that belong to other users? Can they change or delete them?
3. If the app uses Supabase: is row level security switched on for every table? List the policies for each table and explain each one in plain English.
4. If the app uses Firebase: what do the security rules allow? Are any rules open to everyone?
5. Is any table readable or writable by anyone with the public key that ships in the browser?
6. Is there any data stored only in the browser (for example local storage) that would be lost or exposed?

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
Lock down the database so each user can only reach their own data.

Rules for the fix:
- Fix one item at a time, starting with the most urgent.
- Before each change, tell me in one sentence what you are about to change and why.
- After each change, tell me how I can test it myself in the app.
- Do not change how the app looks or behaves for customers unless the fix needs it. If it does, tell me first.
- When you are done, run the check again and show me the new results.
- Switch on row level security (or the equivalent) for every table that holds user data.
- Write policies so users can only read and change their own rows. Admin access must check that the user really is an admin, on the server.
- Show me each policy and explain it in plain English before you apply it.
```

## What good looks like

- No table can be read by someone who is not logged in, unless it is meant to be public (like a product list).
- Logged-in users can only see and change their own records.
- You can explain every database rule in one sentence.

[Back to all prompts](../README.md#the-prompts)
