# Where to paste the prompts

The prompts are plain text, so they work in any AI coding tool with a chat. A few notes per tool:

## Lovable

- Paste the prompt into the project chat. If chat-only mode is available, use it for the Check prompts so nothing changes until you've read the answers.
- Lovable runs a security scan before you publish. Read every warning it shows. If you can't explain a warning in your own words, paste it into the chat and ask: "Explain this warning in plain English and tell me what happens if I ignore it."
- Many Lovable apps use Supabase for the database. The [database prompt](prompts/02-database-and-data-access.md) asks specifically about row level security, the Supabase setting that decides who can read which rows.

## Replit

- Paste the prompt into the Agent or Assistant chat.
- Replit keeps secrets in a separate Secrets panel. The [secrets prompt](prompts/04-secrets-and-api-keys.md) checks they are stored there and not in your files.

## Bolt and v0

- Paste the prompt into the chat for your project.
- These tools often generate the browser side first. Run the [client and server prompt](prompts/01-client-and-server.md) early.

## Claude Code, Cursor and other editors

- Paste the prompt into the agent chat with your project open.
- Ask the agent to put its findings in a file such as `SECURITY_REVIEW.md` so you can share it with someone who reviews your app.

## Connected to GitHub?

If your tool saves your project to GitHub, you can share the repository with a reviewer. You don't need to learn Git to do this. Add them as a collaborator and send them the results of the full audit.
