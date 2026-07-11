# Hunter Terry

I build reliable AI automations — and I follow the same process every
time to make sure they're actually safe to ship. Local-first, safe by
default, documented in plain language.

**Currently looking for remote AI implementation / automation work.**

**Anthropic certified:** Claude 101 · Claude Code 101 ·
AI Fluency: Framework & Foundations · Intro to Claude
Cowork

## The process, not just the tools

The repeatable part — applied the same way on every project below,
whether it's a Python script or an n8n workflow:

- **Preview before action** — nothing changes on disk, or fires a real
  request, without showing you first
- **Never delete, never silently overwrite** — files get moved or
  numbered, not destroyed
- **Validate AI output, never trust it** — every model reply is
  checked against hard rules before it moves on. A model *will* say
  things it shouldn't; the check downstream is what actually holds
  the line
- **QA + security review before shipping** — fail-clean error
  handling, secrets never hardcoded, tested against real failure
  cases (bad input, model unreachable, malformed output) before
  anything goes public
- **Local-first** — inference runs on-device via Ollama/faster-whisper;
  nothing leaves the machine unless a project explicitly calls for it

## Projects

| Repo | What it does |
|---|---|
| [inquiry-triage](https://github.com/hunter-terry/inquiry-triage) | Self-hosted n8n workflow: local AI drafts a customer reply, validated against business rules before a human ever sees it. Caught a real prompt-injection attempt in testing. |
| [lead-qualifier](https://github.com/hunter-terry/lead-qualifier) | Self-hosted n8n workflow: local AI scores incoming leads, a native Switch node (not custom code) routes hot leads one way, cold/invalid another. |
| [auto-summary](https://github.com/hunter-terry/auto-summary) | Watches a folder, transcribes + summarizes audio/video locally, fully unattended. |
| [listit](https://github.com/hunter-terry/listit) | Turns a plain description into an Etsy-ready listing, validated against Etsy's rules rather than trusting the model's reply. |
| [hub](https://github.com/hunter-terry/hub) | Menu-driven launcher for my automation tools; every action needs explicit confirmation. |
| [printpack](https://github.com/hunter-terry/printpack) | Prepares images for print at standard sizes and ratios. |

Built with Claude Code, across Python and n8n. Every repo has a
README that says exactly what the tool does, how it fails, and what
was actually tested — not just what it's supposed to do.

📫 hunterterry234@gmail.com
