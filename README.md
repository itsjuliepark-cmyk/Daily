# Daily: Email Management Bot

A bot that sorts my school Outlook and personal Gmail (coffee chat) email automatically every morning,
groups it into replies needed / deadlines / events / noise, and sends a summary to KakaoTalk.

## Structure

| File | Role |
|---|---|
| `CLAUDE.md` | The bot's operating rules (classification criteria, safety rules, output format) |
| `rules.md` | Classification rules I edit myself (key senders, keywords, things to ignore) |
| `data/coffee-chats.md` | Coffee chat log: who, when, follow-ups |
| `prompts/daily-brief.md` | Prompt used by the daily morning automated run (Routine) |
| `docs/outlook-setup.md` | How to connect school Outlook without signing in each time |

## Setup steps

1. ✅ Gmail, Google Calendar, and KakaoTalk connected
2. ✅ School email (spark@mba2028.hbs.edu) already arrives in Gmail, so no separate Outlook connection is needed
3. ✅ Gmail labels created: `Daily/🔴답장필요` (reply needed), `Daily/🟠School`, `Daily/🟢이벤트` (events), `Daily/⚪노이즈` (noise)
4. ✅ Automated briefing Routine every morning at 7:52 (ET)

> Gmail label names are kept exactly as they exist in Gmail, since the bot looks them up by name.
