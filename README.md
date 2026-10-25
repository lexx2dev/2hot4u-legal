# 2hot4u

A Discord bot that gives every member their own temporary voice room. Join the hub channel and a room is created for you, with a control panel to lock, trust, block, rename, set limits, kick, transfer ownership and more. Empty rooms are deleted automatically.

## Setup (server admins)

1. Invite the bot with `/invite`.
2. Run `/config` and choose the **hub** voice channel and the **category** for rooms.
3. Run `/panel` to post the control panel, and `/help` for an overview.

## Commands

| Command | Description |
| --- | --- |
| `/config` | Admin dashboard (Administrator only) |
| `/panel` | Post the room control panel |
| `/help` | How everything works |
| `/invite` | Link to add the bot to your server |

## Self-hosting

Requires Node.js 18+ and MySQL.

```bash
cp .env.example .env   # fill in the values
npm install
npm start
```

The database schema is created automatically on first start. Use a process manager such as PM2 to keep the bot running.

The bot needs only the non-privileged intents `Guilds`, `GuildMessages` and `GuildVoiceStates`.

## Legal

See [PRIVACY.md](PRIVACY.md) and [TERMS.md](TERMS.md).
