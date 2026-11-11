# Vibe coding security prompts

Copy-paste prompts that help you make an app built with Lovable, Replit, Bolt, v0, Cursor or Claude Code safe to put in front of real customers. No coding knowledge needed.

You built an app with AI. It works. Before real people sign up, pay, or type in their details, you need to know a few things the AI may not have told you: where your data lives, who can see it, whether your keys are exposed, and what happens if something breaks.

These prompts ask your AI tool to check its own work and explain the answers in plain English.

## How to use them

1. Open your project in the tool you built it with.
2. Paste a **Check** prompt into the chat. It tells the AI to look and explain, without changing anything.
3. Read the answers. If something says **Problem** or **Not sure**, paste the matching **Fix** prompt.
4. Run the Check prompt again until everything comes back **OK**.

If your tool has a chat-only or plan mode (one that talks without editing), use it for the Check prompts.

## Start here

If you only do one thing, run the [full audit](prompts/00-full-audit.md). It covers the basics in one go and tells you which topics to look at next.

## The prompts

| Topic | What it checks |
|---|---|
| [Full audit](prompts/00-full-audit.md) | Everything below, at a high level |
| [Client and server](prompts/01-client-and-server.md) | Which code runs in the customer's browser and which runs on a server |
| [Database and data access](prompts/02-database-and-data-access.md) | Whether one user can read or change another user's data |
| [Log-in and accounts](prompts/03-login-and-accounts.md) | Sign-up, log-in, passwords, roles such as admin |
| [Secrets and API keys](prompts/04-secrets-and-api-keys.md) | Keys and passwords visible in your code or in the browser |
| [Screens and forms](prompts/05-screens-and-forms.md) | What your forms accept, error messages, what the screen shows |
| [Personal data and GDPR](prompts/06-personal-data-and-gdpr.md) | What personal data you collect, why, and how people can delete it |
| [Payments](prompts/07-payments.md) | How money moves, and what stops someone paying less or nothing |
| [Backups and recovery](prompts/08-backups-and-recovery.md) | What happens if data is deleted or the app goes down |
| [Cost and abuse](prompts/09-cost-and-abuse.md) | Bots, spam, and surprise bills from AI or email services |
| [Before go-live](prompts/10-before-go-live.md) | A final pass the day before you launch |

## The 10-question checklist

Answer yes or no before real customers arrive. If you can't answer one, run the matching prompt.

See [checklist.md](checklist.md).

## When to ask a person

The prompts get you a long way. Ask someone who knows software architecture to look at your app before you:

- take payments,
- store health, financial or children's data,
- connect the app to your company's other systems, or
- give it to more than a few hundred users.

One review at that moment is enough for most small apps. A freelancer, a developer friend or your company's IT team can do it in an afternoon if you hand them the results of the full audit.

## Tool-specific notes

See [platforms.md](platforms.md) for where to paste the prompts in each tool.

## Contributing

Found a prompt that works better, or a problem these miss? Open an issue or a pull request. Plain-English improvements are as welcome as technical ones.

## Want an automatic check?

These prompts rely on your AI tool reviewing its own work, which is a good start but not a guarantee. For a check that runs the same rules every time:

- [Production-ready check](https://github.com/qualityclouds/Skill-production-ready-check) is a free Agent Skill that scores your project from 0 to 100. No account needed.
- [State of AI code 2026](https://github.com/qualityclouds/state-of-ai-code-2026) is our open dataset of 424 AI-generated projects, if you want to see which problems come up most often.

## About

Maintained by [Quality Clouds](https://qualityclouds.ai). We build tools that check AI-written code. These prompts are free to use, copy and adapt under the MIT license.
