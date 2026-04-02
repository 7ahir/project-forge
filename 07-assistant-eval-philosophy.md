# Assistant Eval Philosophy

## Question This File Answers

How would I evaluate an AI coding assistant as a product, not just as a model?

## PM Skills Demonstrated

- `epic-hypothesis`: ties evaluation to product bets instead of abstract model quality
- `product-strategy-session`: connects discovery, workflow value, and roadmap consequence
- `roadmap-planning`: turns evaluation outcomes into prioritization and sequencing decisions

## Core Thesis

An AI coding assistant should be evaluated on whether it helps developers move through real coding workflows with enough quality, speed, and trust to change behavior.

That means the eval system should answer product questions such as:

- Did the assistant help produce a useful diff?
- Did it make debugging faster or noisier?
- Did it improve test repair or create cleanup?
- Did it help the developer get to a review-ready change?

If the eval stack cannot answer those questions, it is not sufficient for product management.

## What I Would Not Optimize For Alone

- benchmark scores detached from live workflows
- prompt-level thumbs-up rates
- raw prompt volume
- isolated code-generation tasks with no repo or review context
- internal excitement about model upgrades without product consequence

These signals may matter, but they are weak foundations for roadmap and launch decisions.

## Product Eval Stack

I would use four layers.

### 1. Workflow evals

These are the center of gravity.

| Workflow | Questions the eval should answer | Example measures |
|---|---|---|
| Repo-aware edit loop | Did the assistant pull the right context and produce a useful, inspectable diff? | accepted diff rate, file-reference accuracy, time to first useful diff |
| Debug loop | Did the assistant help diagnose and fix the problem with less wasted effort? | issue-to-fix success rate, failed-fix retry rate, root-cause usefulness |
| Test loop | Did the assistant help create, repair, or stabilize tests in a meaningful way? | test repair success, test usefulness rating, baseline-check pass contribution |
| PR and review loop | Did the assistant help the developer explain and ship the change more cleanly? | PR-summary usefulness, review-ready rate, review-response quality |

### 2. Trust evals

These tell me whether stronger capability is actually becoming safer to rely on.

| Trust dimension | Example measures |
|---|---|
| Confidence and control | rollback frequency, assisted-change rejection rate, reversibility usage |
| Context trust | file-reference accuracy, context-miss reports, irrelevant-context frequency |
| Review trust | reviewer confidence rating, explanation usefulness, review churn after assisted changes |

### 3. Product behavior evals

These answer whether the assistant fits the real product experience.

| Dimension | Example measures |
|---|---|
| Latency tolerance | time to first useful diff, drop-off before first action |
| UX clarity | confusion points, mis-click or abandonment patterns, source-visibility usage |
| Surface fit | usage across IDE, repo, terminal, and PR surfaces |

### 4. Business evals

These keep PM honest about whether workflow value is converting into a business.

| Business question | Example measures |
|---|---|
| Is usage repeating? | weekly active developers, repeat workflow completion |
| Is team adoption growing? | pilot expansion rate, active teams, lead confidence |
| Is enterprise motion grounded? | pilots with workflow-specific value cases, rollout decision rate |

## Evaluation Principles

### Principle 1: Evaluate at the workflow level

Coding assistants are not one product moment. Edit, debug, test, and review work should be measured separately before being rolled up.

### Principle 2: Separate model quality from product quality

A model upgrade may improve raw generation quality while leaving repo-context retrieval, latency, or review usefulness unchanged.

### Principle 3: Measure usefulness before delight

If the assistant does not help with high-friction work, delight is not a durable moat.

### Principle 4: Use evals to kill bets, not just justify them

An eval system that only supports launch arguments is governance theater.

### Principle 5: Tie every major bet to one or two governing metrics

If a roadmap bet cannot name the workflow evals that will validate it, it is not ready.

## What Good PM Use Of Evals Looks Like

| Situation | Good PM behavior | Bad PM behavior |
|---|---|---|
| Repo edit loop improves on benchmarks but not in live repos | Hold the launch scope, fix repo-context quality, instrument the misses | Broaden the release because the model improved |
| PR summaries get strong qualitative feedback but weak repeat usage | Treat it as promising but not yet wedge-worthy | Declare it a core surface because users said it was cool |
| Debug support is messy but high-frequency | Protect the bet if the workflow is strategically important and the failure mode is fixable | Kill it too early because it is harder than draft generation |

## How Evals Should Change The Roadmap

- If edit-loop evals are weak, do not broaden into more agentic behavior.
- If debug support strengthens repeat usage, protect that wedge even if it is messier to build.
- If review assistance helps team trust materially, move it earlier in the roadmap.
- If enterprise buyers love the story but workflow evals stay weak, slow the GTM promise.

## What This Proves In A Hiring Process

- I know how to turn model progress into product questions.
- I understand that eval design is part of product strategy in AI-native products.
- I would govern a coding assistant with workflow truth, not benchmark theater.

## Read Next

[Competitive Wedge Memo](08-competitive-wedge-memo.md)

