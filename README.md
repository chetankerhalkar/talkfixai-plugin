# TalkFixAI plugin

Fix things at home, safely. TalkFixAI gives Claude, ChatGPT and other AI
assistants tested step-by-step repairs, the safety precautions for the job, the
parts you'll need, and an honest answer on when to stop and call a professional.

Free, with no sign-in. Every tool is read-only.

## What it does

- **Tested repairs**: WiFi router, phone screen, leaky faucet, tubelight, water
  filter, air conditioner, circuit breaker and door lock, one step at a time.
- **Safety first**: a gas smell, a carbon monoxide alarm, a swollen battery,
  water on live electrics or bare wiring gets a fixed, checked reply before any
  repair advice.
- **Any other repair**: the assistant writes the guide in TalkFixAI's format,
  with the precautions for that job.

Try: "My kitchen tap keeps dripping, help me fix it."

## Install

### Claude Code

```
/plugin marketplace add chetankerhalkar/talkfixai-plugin
/plugin install talkfixai@talkfixai
```

### Claude (web, desktop, mobile) and ChatGPT

Add a custom connector with this address:

```
https://talkfixai-api-h0byf7cuaah4gmab.centralus-01.azurewebsites.net/mcp
```

## What's in this repo

| Path | What it is |
|---|---|
| `.claude-plugin/marketplace.json` | The marketplace Claude Code reads |
| `talkfixai/.claude-plugin/plugin.json`, `talkfixai/.mcp.json` | The Claude plugin and its MCP server address |
| `talkfixai/plugin.json`, `talkfixai/mcp.json` | The same plugin in the Agent Plugins format |
| `talkfixai/skills/fix-it/SKILL.md` | The skill that tells the assistant when and how to use TalkFixAI |

The MCP server itself is hosted by AICK Studio; this repo only points to it.

## The app

TalkFixAI is also a free phone app: talk through the repair out loud while your
hands are busy, and show it the problem with the camera.
[aickstudio.ai/talkfixai](https://aickstudio.ai/talkfixai)

## Safety

TalkFixAI is guidance, not a substitute for a qualified professional. Stop and
call one for gas, mains wiring you are unsure about, and anything that smells
of burning. [Support](https://aickstudio.ai/talkfixai/support) ·
[Privacy](https://aickstudio.ai/talkfixai/privacy) ·
[Terms](https://aickstudio.ai/talkfixai/terms)
