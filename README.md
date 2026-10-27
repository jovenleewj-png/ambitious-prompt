# Ambitious Prompt

### By [Joven lee](https://www.linkedin.com/in/jovenleeweijun/)

**Turn a rough request into a clear brief with domain expertise, evidence, and a way to check the result.**

Ambitious Prompt is a reusable skill for improving what you ask an AI to do. It reads your context, researches relevant expert methods when needed, and rewrites your request into a prompt you can review. Once you approve, the assistant carries out the agreed task with the tools available to it.

Use it for research, business decisions, product work, writing, analysis, and software tasks. The approach works across industries and models; search and execution depend on your assistant's available tools.

[Download the latest skill ZIP](https://github.com/jovenleewj-png/ambitious-prompt/releases/latest/download/ambitious-prompt.zip) · [Read the skill](SKILL.md) · [Release log](CHANGELOG.md)

## The problem

A short request often leaves the AI to decide what you mean by “good.” It may produce a polished answer while missing the evidence, methods, or decision that matter.

| What goes wrong | What this skill asks for |
| --- | --- |
| The task is clear, but its purpose is missing | The outcome, audience, and decision the work should support |
| The AI sounds knowledgeable without using expert methods | Relevant techniques, suitable inputs, and a reason to use them |
| Assumptions quietly become facts | Clear distinctions between evidence, assumptions, and missing information |
| A useful request grows into an oversized project | A deeper approach within the scope you chose |
| The answer looks convincing but is hard to check | Acceptance criteria and evidence that could confirm or challenge it |

## How it works

1. **Understand the request.** Identify the goal, audience, constraints, deliverable, and available material. Ask about consequential gaps; state sensible assumptions for minor choices.
2. **Bring in domain knowledge.** For substantive specialist work, research relevant primary sources before rewriting. Select methods that change the approach, and explain what inputs they need. A simple edit can skip this research.
3. **Choose the right ambition.** Adapt speed, altitude, depth, and range using [Felix Rieseberg’s article](https://felixrieseberg.com/how-to-be-more-ambitious-a-tutorial-for-humans-with-models/) as a design reference for the skill. Improve the work within the request's boundaries.
4. **Apply practical discipline.** Surface assumptions, choose a simple approach, keep changes focused, and define verifiable goals. These four disciplines adapt the community's Karpathy-inspired guidelines beyond coding.
5. **Show the rewritten prompt.** Return a self-contained brief with the relevant context, methods, constraints, evidence, and completion criteria. Ask for your approval before starting the underlying task.
6. **Execute after approval.** Work from the approved version, check what can be checked, and report results and remaining limitations. If you request revisions, show the revised prompt for approval first.

### Four ways to raise the standard

| Dimension | What it changes | Example |
| --- | --- | --- |
| Speed | Removes avoidable effort | Reuse supplied evidence and organize the work efficiently |
| Altitude | Connects the deliverable to its purpose | Make a board update support a decision about retention investment |
| Depth | Strengthens inputs, methods, and checks | Compare customer cohorts and reconcile billing data before explaining churn |
| Range | Adds a useful technique from another field | Combine financial reconciliation with qualitative analysis of support tickets |

The skill selects what helps. It keeps the requested deliverable, treats stretch targets as proposals, and preserves creative intent. An email edit can remain a two-sentence prompt.

## Before and after

This illustrative example shows a substantial request receiving a substantial brief. It is not a completed diagnosis or a claim that any business records have been inspected. The eventual rewrite should reflect the actual context and verified domain research available in that session.

**Before — your request**

> Our customer onboarding takes too long, and teams keep redoing work. Use our existing onboarding records to find where the process breaks down and propose a better handoff from sales to implementation. Do not add headcount or change our systems.

**After — the rewritten prompt**

<details open>
<summary><strong>Diagnose the handoff, identify the causes of delay, and design a testable improvement</strong></summary>

Work from the onboarding records I provide to determine where the sales-to-implementation handoff creates avoidable delay or rework, and propose a better process within our existing headcount and systems. The outcome is a handoff the implementation team can act on without repeatedly returning to sales for information.

### 1. Establish what the records can tell us

Identify the available source material: signed scope and sales commitments, handoff forms, implementation tickets, milestone histories, customer communications, ownership changes, and any existing process documentation. List what is actually available and the period it covers. Request the smallest set of missing inputs that would materially change the diagnosis.

Recover the agreed meaning of “ready for implementation” and “live” from our existing process. Separate customer-requested pauses, external dependencies, and product limitations from internal handoff failures. Flag inconsistent timestamps and missing histories before comparing projects. Preserve source records and existing versions.

### 2. Reconstruct the work before assigning blame

Build a timeline for each usable onboarding case, from the relevant sales commitment through handoff, implementation, and go-live. Trace each material issue through:

**Commitment → required input → handoff → receiving owner → implementation dependency → customer outcome.**

For each transition, distinguish elapsed time, recorded active work, waiting, and rework. If active effort was not recorded, report it as unknown rather than inferring it from elapsed time.

Compare cases by characteristics supported by the records, such as integration complexity, customer readiness, or implementation type. Show case counts, missing-data coverage, medians, and the distribution of elapsed times where the data supports them. Check whether a few exceptional projects explain the apparent slowdown. Avoid comparing unlike projects or treating the most frequently documented complaint as the largest source of delay.

### 3. Diagnose the failure mechanisms

Evaluate whether each handoff contains the information needed to begin, has a clear receiving owner, matches the signed scope, exposes dependencies, and records acceptance or rejection. Define each criterion and its observable evidence before assessing cases; use “not assessable” when the records cannot support a judgment.

Distinguish recurring mechanisms such as incomplete inputs, conflicting promises, unclear ownership, sequencing errors, approval queues, and capacity constraints. Support each priority diagnosis with source references, an affected-case count, its contribution to observed delay or rework where measurable, and a confidence statement.

Include successful cases and counterexamples. A late project with a complete handoff may challenge a handoff-based explanation. Separate observed failures from hypotheses about their causes; do not attribute poor performance to a team or individual without evidence.

### 4. Design the smallest useful change

For the strongest supported bottlenecks, show:

- **Current practice:** the actual field, instruction, ownership rule, or transition causing difficulty, with its source reference.
- **Failure mechanism:** how it creates waiting, rework, or an incorrect commitment.
- **Proposed change:** revised handoff information, acceptance criteria, routing, or escalation using our existing systems.
- **Expected effect:** the mechanism by which the change could help; quantify only what the records support and label estimates.
- **Cost and tradeoffs:** added work, shifted responsibility, customer friction, and any new failure mode.
- **Verification:** the observation that would confirm or challenge the expected improvement.

Consider information quality and workflow design before adding approvals or forms. Check whether a change removes work or simply moves the queue to another team. Keep headcount and systems fixed; identify any improvement that cannot meet those constraints as outside this proposal.

### 5. Test against history and propose a bounded pilot

Replay the proposed handoff rules against historical cases to see which failures they would have flagged, which successful cases they would have blocked unnecessarily, and which delays they would not address. Where there are enough cases, reserve a separate set for checking the revised rules after development. If the sample is too small, disclose the limit instead of claiming generalization.

Historical replay can test whether missing information would have been detected; it cannot prove that time would have been saved. Design a pilot that measures both go-live time and staff effort, with safeguards for scope errors and customer experience. Account for differences in project complexity and customer readiness; explain the limits of causal inference if comparable allocation is not feasible.

Propose the pilot duration, owners, success thresholds, and rollback triggers from the baseline evidence. Label these as proposals for approval. Do not invent a percentage improvement, promise savings, or claim that the pilot has already run.

### 6. Deliver a decision we can act on

Produce a concise decision brief with:

- A reconciled baseline and the most consequential supported bottlenecks.
- An evidence-linked current-state process map and prioritized diagnosis.
- Concrete before-and-after handoff changes with ownership and tradeoffs.
- The results of any historical checks actually performed.
- A proposed pilot, acceptance criteria, rollback conditions, and remaining evidence gaps.

Keep detailed case tracing in a supporting table so the main brief remains readable. Distinguish verified observations, estimated effects, and proposed actions. If the records do not establish a cause, identify the evidence that would discriminate between the remaining explanations.

Use the supplied records and authorized tools to carry out the diagnosis and prepare the proposal. Stop when the brief and its evidence checks are complete, or report the specific missing inputs that block a defensible conclusion. Obtain separate approval before changing live workflows, contacting staff or customers, or starting the pilot.

</details>

**What changed:** the rewrite defines the operational outcome, names the raw evidence, specifies a diagnostic method, tests alternative explanations, and connects each proposed change to a check. It also asks for historical validation and a bounded pilot without treating either as proof of benefits that have not been observed.

The skill shows this prompt for approval before starting the diagnosis. This level of detail fits a cross-functional operational problem; simpler tasks receive shorter prompts.

### Other requests it can improve

| Your request | A useful improvement |
| --- | --- |
| “Fix duplicate charges when our webhook retries.” | Identify the repeat-payment path, use provider documentation, preserve the payment stack, and specify tests for retries and concurrency |
| “Help me price this research project.” | Identify scope and cost drivers, distinguish supplied costs from estimates, and check the proposed margin |
| “Prepare six slides for the board.” | Define the decision, evidence, narrative, and meeting constraints while retaining the six-slide deliverable |
| “Make the second sentence warmer.” | Preserve the facts and every other sentence, with a short rewrite and no unnecessary research |

## When to use it

Use it when your request has an important outcome but leaves the method or quality bar unclear; when you are entering an unfamiliar field; or when you want to review the brief before an assistant starts work.

For a fully specified, trivial task, the benefit may be small. You can request prompt-only output if you want to take the rewritten brief elsewhere.

## Install and use

### Claude Code

```bash
git clone https://github.com/jovenleewj-png/ambitious-prompt.git ~/.claude/skills/ambitious-prompt
```

Then invoke:

```text
/ambitious-prompt Help me prepare a board update about customer churn.
```

### Codex

Clone into your configured skills directory; the default is shown below:

```bash
git clone https://github.com/jovenleewj-png/ambitious-prompt.git ~/.codex/skills/ambitious-prompt
```

Start a new chat and invoke:

```text
Use $ambitious-prompt to improve this request: [your request]
```

If the destination folder already exists, update or back it up before installing. These clone commands do not overwrite an existing installation.

### Claude chat or Cowork

Download `ambitious-prompt.zip` from the [latest release](https://github.com/jovenleewj-png/ambitious-prompt/releases/latest). Upload it through **Customize → Skills → + → Create skill → Upload a skill**, then enable it. Claude requires code execution and file creation to be enabled for skills.

```text
Use the ambitious-prompt skill for every new request in this chat.
Rewrite first, ask for approval, then execute after I approve.

My request: [your request]
```

### Other models

Provide [SKILL.md](SKILL.md), its linked references, and your request. A host that supports skills can load the folder; other models can follow the supplied instructions within their capabilities.

To request ongoing use in a chat, ask the assistant to apply the skill to each new substantive request. Automatic activation in other chats depends on the host.

## What to expect

- The rewritten prompt makes important assumptions and missing inputs visible.
- Specialist tasks name relevant methods and explain how their results can be checked.
- Small tasks receive short prompts; broader tasks receive enough structure to be actionable.
- Approval applies to the prompt you saw. A revised specification returns to you before execution.
- Verification claims refer to checks actually performed; unavailable checks remain explicit.

Domain research takes time and may use additional tokens. Without browsing, the skill works from supplied context and labels knowledge that has not been verified. Without files or execution tools, it identifies the inputs or checks needed to proceed. It cannot guarantee that any model follows every instruction, or that a better prompt guarantees a correct result.

## About Joven

**Joven lee** is **Chief Research & Revenue Officer of Cookiy Labs** and **President of Cookiy AI**. His background spans more than 15 years in market research and B2B growth, including Nielsen and NielsenIQ, Statista, and Cint.

His work connects customer understanding with commercial strategy, research operations, pricing, and applied AI. He created this project to make ambitious AI use practical: stronger requests, relevant expertise, evidence, and control over execution.

[Connect on LinkedIn](https://www.linkedin.com/in/jovenleeweijun/) · [Creator background](references/about-joven.md)

## Releases

Current version: **1.0.3**. Each published release includes notes about significant changes, any update or reinstallation needed, and an installable skill ZIP.

[Changelog](CHANGELOG.md) · [GitHub Releases](https://github.com/jovenleewj-png/ambitious-prompt/releases)

## Credits and permissions

Felix Rieseberg's article informs the ambition framework. The [Karpathy-inspired guidelines](https://github.com/multica-ai/andrej-karpathy-skills) inform the four behavioral disciplines. That repository is a community adaptation of Andrej Karpathy's observations, not an official Karpathy skill. See [source notes](references/sources.md).

Copyright (c) 2026 Joven Lee Wei Jun. See [NOTICE.md](NOTICE.md) for authorship, attribution, and permission inquiries. This repository does not grant an MIT or other reuse license.

Installation references: [Claude skills](https://support.claude.com/en/articles/12512180-use-skills-in-claude) · [Claude Code skills](https://code.claude.com/docs/en/skills).
