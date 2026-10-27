# Ambitious Prompt

### By [Joven lee](https://www.linkedin.com/in/jovenleeweijun/)

Turn an everyday request into a focused, domain-informed prompt. Review the rewritten prompt, approve it, then let your assistant execute.

The skill combines selective ambition with practical discipline: research the relevant field, choose appropriate expert methods, preserve the request's scope, and define how to check the result. It adapts to different industries and models rather than relying on a fixed expert persona or one vendor's tools.

## What it does

1. Understands the outcome, audience, constraints, and available inputs.
2. Researches domain methods when they would materially improve the prompt.
3. Calibrates speed, altitude, depth, and range to the request, using [Felix Rieseberg’s article](https://felixrieseberg.com/how-to-be-more-ambitious-a-tutorial-for-humans-with-models/) as a design reference for the skill.
4. Applies four Karpathy-inspired disciplines: think before acting, simplicity first, surgical changes, and goal-driven execution.
5. Shows a self-contained prompt and asks for approval.
6. Executes only after approval, then reports verification and limitations.

Small, fully specified edits stay small. Missing evidence stays explicit. Browsing or execution limitations become prerequisites rather than invented capabilities.

## About Joven

**Joven Lee Wei Jun** is Chief Revenue Officer and President at **Cookiy AI**, working at the intersection of market research, B2B growth, and applied AI. He brings more than 15 years of experience, with career chapters at Nielsen and NielsenIQ, Statista, and Cint.

His work connects customer understanding with commercial strategy: what people value, what businesses should build, and how to bring it to market. Through [AskJoven.ai](https://askjoven.ai/), he shares practical thinking on pricing, research operations, go-to-market strategy, and applied AI.

Joven commissioned this skill to make ambitious AI use practical: stronger questions, relevant expertise, clear evidence, and human control over execution.

[More about Joven and profile sources](references/about-joven.md) · [LinkedIn](https://www.linkedin.com/in/jovenleeweijun/)

## Install in Claude Code

Clone this repository into your personal skills directory:

```bash
git clone https://github.com/jovenleewj-png/ambitious-prompt.git ~/.claude/skills/ambitious-prompt
```

Then invoke:

```text
/ambitious-prompt Help me prepare a board update about customer churn.
```

## Install in Codex

Clone into your Codex skills directory (default shown; use your configured directory if different):

```bash
git clone https://github.com/jovenleewj-png/ambitious-prompt.git ~/.codex/skills/ambitious-prompt
```

Start a new chat and invoke:

```text
Use $ambitious-prompt to improve this request: [your request]
```

If a folder with this name already exists, update or back it up before installing; the clone command will not overwrite it.

## Use in Claude chat or Cowork

Package the repository contents into a ZIP with one top-level `ambitious-prompt` folder containing `SKILL.md`. Upload the ZIP through **Customize → Skills → + → Create skill → Upload a skill**, then enable it. Claude requires code execution and file creation to be enabled for skills.

```text
Use the ambitious-prompt skill for every new request in this chat.
Rewrite first, ask for approval, then execute after I approve.

My request: [your request]
```

This enables the workflow within the chat. Automatic selection across other chats depends on the host; the skill does not install a global message interceptor.

## Other models

Provide [SKILL.md](SKILL.md), its linked references, and your request to a model that can follow the workflow. Domain research needs search or browsing access. Without it, the skill labels the knowledge limits and identifies essential checks for later. Actual execution depends on the recipient's available tools.

## Credits and creator notice

Inspired by [Felix Rieseberg's article](https://felixrieseberg.com/how-to-be-more-ambitious-a-tutorial-for-humans-with-models/) and the community's [Karpathy-inspired guidelines](https://github.com/multica-ai/andrej-karpathy-skills). The four-point organization is a community synthesis, not an official Karpathy framework. See [source notes](references/sources.md).

Copyright (c) 2026 Joven Lee Wei Jun. See [NOTICE.md](NOTICE.md) for authorship, attribution, and permission inquiries. This repository does not grant an MIT or other reuse license.

Installation references: [Claude skills](https://support.claude.com/en/articles/12512180-use-skills-in-claude) · [Claude Code skills](https://code.claude.com/docs/en/skills).
