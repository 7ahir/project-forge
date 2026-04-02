# Roadmap

## Question This File Answers

Which bets come first, and how would I sequence them without confusing activity for strategy?

## PM Skills Demonstrated

- `epic-hypothesis`: frames major bets as testable outcomes rather than feature promises
- `prioritization-advisor`: informs the hybrid prioritization logic used for strategic bets and stakeholder pressure
- `roadmap-planning`: turns product strategy into a sequenced narrative roadmap with explicit tradeoffs

## Roadmap Principle

This roadmap follows the logic of the local `roadmap-planning` and `epic-hypothesis` skills:

- start from outcomes, not features
- treat major initiatives as hypotheses
- sequence bets so learning compounds
- keep the roadmap sharp enough to survive executive review

## Planning Horizon

This is an illustrative four-quarter roadmap. It is not a claim about any specific company plan.

## Strategic Themes

| Theme | Why it matters |
|---|---|
| Repo-aware edit loop | Repeated usage starts with trusted code changes in real repositories |
| Debug and test loop | A coding assistant becomes sticky when it helps recover from failure, not just draft code |
| PR and review support | Teams trust the product more when it helps prepare and explain changes cleanly |
| Evaluation legibility | Better bet quality requires better product-facing evals |
| Team rollout and enterprise expansion | Monetization depends on a credible rollout and proof story |

## Roadmap View

| Horizon | Theme | Bet | Why now |
|---|---|---|---|
| Now | Repo-aware edit loop | Trusted multi-file edit quality, inspectability, and reversibility | Highest leverage path to repeated use in real repositories |
| Now | Evaluation legibility | Workflow-level eval stack for edit, debug, test, and PR tasks | Stops roadmap drift and benchmark theater |
| Next | Debug and test loop | Failure diagnosis, fix iteration, and test repair support | Extends the assistant into a daily high-friction workflow |
| Next | PR and review support | PR summary generation, change explanation, and review-response help | Makes the assistant useful later in the coding loop, not just at draft time |
| Later | Team rollout and enterprise expansion | Shared team settings, quality visibility, and pilot-to-rollout tooling | Converts individual pull into pilot expansion |
| Later | Team rollout and enterprise expansion | Governance and integration hardening based on observed pilot blockers | Prevents premature enterprise sprawl |

## Major Bet Hypotheses

### Bet 1: Trusted repo-aware edit loop

**Hypothesis**
If we improve repo-aware edit quality and make changes easier to inspect and reverse, then we will increase repeated weekly usage because developers will trust the assistant on real code changes rather than only low-risk drafting.

**Primary learning metric**
- Edit acceptance rate on assisted changes

**Kill or pivot signal**
- Acceptance improves only marginally while abandonment stays high

### Bet 2: Workflow eval stack

**Hypothesis**
If we instrument workflow-level evaluation for the main jobs users care about, then roadmap decisions will improve because we will see product truth earlier than launch-stage sentiment or generic model benchmarks.

**Primary learning metric**
- Percent of roadmap bets with a workflow-specific success measure and review cadence

**Kill or pivot signal**
- Evals exist but do not change prioritization or release decisions

### Bet 3: Debug and test repair loop

**Hypothesis**
If we improve the assistant's ability to diagnose failures, suggest fixes, and repair tests, then repeated weekly usage will grow because developers will use the assistant for high-friction moments that happen after the first code draft.

**Primary learning metric**
- Issue-to-fix success rate on assisted debug sessions

**Kill or pivot signal**
- Developers try the flow but return to manual debugging because the fix path is noisy or untrustworthy

### Bet 4: PR and review assistance

**Hypothesis**
If we help developers prepare PR summaries, explain diffs, and respond to review comments more effectively, then team trust and downstream usage will improve because the assistant will support how teams actually ship and review code.

**Primary learning metric**
- Percent of assisted changes judged review-ready by developers or leads

**Kill or pivot signal**
- Review support gets used occasionally but does not materially improve shipping or review behavior

### Bet 5: Trusted team rollout and enterprise narrative

**Hypothesis**
If we provide team-level standards, visibility, and rollout guidance tied to the edit, debug, test, and PR workflows already proven useful, then pilot-to-team expansion will improve because leads and rollout owners will have more confidence in how the assistant behaves in shared coding workflows.

**Primary learning metric**
- Percent of pilot teams that expand usage beyond early champions

**Kill or pivot signal**
- High curiosity from buyers but weak expansion after pilot

## Prioritization Logic

I would not use a single scoring framework blindly here.

Per the logic of the local `prioritization-advisor` skill, this roadmap needs a hybrid:

- strategic-first prioritization for category-defining bets
- lightweight scoring for within-theme choices
- explicit executive overrides only when tied to a named strategic reason

The practical rule:

- protect a small number of long-horizon bets
- use evidence to rank options inside those bets
- do not let near-term enterprise pressure erase the wedge

## What I Would Not Put On This Roadmap Yet

- broad marketplace ecosystems
- many niche IDE or workflow surfaces
- large compliance or governance packages without adoption evidence
- generalized "AI for the whole SDLC" claims

Those may matter later, but they are poor early roadmap anchors if the mainline edit, debug, test, and review product is not yet trusted.

## Read Next

[Flagship Initiative](05-flagship-initiative.md)
