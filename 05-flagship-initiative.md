# Flagship Initiative: Trusted Edit-to-PR Loop

## Question This File Answers

Can I take the category thesis and turn it into a concrete, cross-functional initiative with real product judgment?

## PM Skills Demonstrated

- `epic-hypothesis`: defines the initiative as a bet with a measurable outcome
- `prd-development`: gives the initiative product-goal, scope, users, risks, and decision-gate depth
- `user-story`: translates the initiative into concrete user-facing needs rather than abstract strategy language

## Why This Initiative

This is the best showcase initiative because it proves I understand the core product surface of a coding assistant:

- repo context
- inspectable code edits
- test and review readiness

If the assistant can reliably help a developer move from task to review-ready diff, a large share of the category's strategic friction starts to drop with it.

## Problem

Many AI coding assistants can generate code in isolation but struggle in the actual repo workflow.

The usual failure pattern:

- the assistant pulls incomplete or noisy context
- the first diff looks plausible but needs heavy cleanup
- tests fail or are not addressed cleanly
- the developer still has to manually explain the change in review
- trust drops before the product becomes habit

## Product Goal

Create a trusted edit-to-PR loop that helps developers move from task to review-ready change with better repo context, stronger diffs, test awareness, and clearer explanations.

## Epic Hypothesis

If we improve the assistant's repo-context retrieval, diff quality, test awareness, and PR explanation flow, then repeated usage and team trust will improve because developers will be able to use the assistant on real code changes instead of one-off draft moments.

## Desired Outcomes

These metrics are illustrative.

| Outcome | Illustrative target |
|---|---|
| Assisted diffs accepted with minor or no modification | 42% -> 60% |
| Time to first useful diff | -30% |
| Assisted changes passing baseline checks before handoff | +20 points |
| Sessions ending in abandonment after low-trust output | -25% |
| Review-ready PR summary usefulness | +25 points |

## In Scope

- repo-context assembly and visibility
- multi-file edit flow with inspectable, reversible diffs
- baseline test and validation awareness before handoff
- PR summary and change-explanation support
- workflow-specific trust signals for edit, test, and review outcomes

## Out Of Scope

- full autonomous software engineering agent behavior
- complex policy engines for every customer archetype
- broad custom controls requested by one buyer
- replacing human review or code ownership models

## Key Users

### User 1: Individual developer

Needs the assistant to understand repo context, produce useful diffs, and reduce cleanup before review.

### User 2: Tech lead

Needs to know whether assistant-generated changes are improving throughput without degrading code quality.

### User 3: Reviewer or team lead

Needs changes and explanations to be clear enough that review does not become harder.

## Core User Stories

### Story 1: Developer

As a developer, I want the assistant to pull the right repo context and propose an inspectable diff so that I can get to a useful code change faster.

### Story 2: Developer

As a developer, I want the assistant to surface likely test impact and help repair failures so that I spend less time bouncing between generation and manual cleanup.

### Story 3: Reviewer or tech lead

As a reviewer or tech lead, I want a clear explanation of the assistant-generated change so that I can review faster without losing confidence.

### Story 4: Product and engineering leadership

As product and engineering leadership, we want workflow-specific success signals so that we can decide whether this loop deserves broader rollout.

## MVP Shape

The first version should stay narrow and prove one strong coding-assistant loop.

### v1 components

- rollout template for one or two core workflows
- repo-context visibility for the files and symbols used
- inspectable, reversible diff application
- baseline test-awareness and failure surfacing
- PR summary and explanation generation
- lightweight trust dashboard with edit, test, and review signals

### Why this is enough

This version is large enough to test the core hypothesis and small enough to avoid pretending the product is a full autonomous coding agent before the edit-to-PR loop is proven.

## Decision Gates

| Gate | Question |
|---|---|
| Gate 1 | Do developers reach a useful diff faster with enough repo context and control? |
| Gate 2 | Are assisted changes passing baseline checks and holding up in review? |
| Gate 3 | Does stronger edit-to-PR quality improve repeated usage and team trust? |

## Risks

| Risk | Mitigation |
|---|---|
| Repo context retrieval is slow or noisy | Bound v1 to the most common developer workflows and instrument context quality directly |
| Diff quality improves in demo cases but not real repos | Evaluate on live workflow tasks rather than benchmark-style prompts |
| Test awareness becomes cosmetic instead of useful | Measure check-pass contribution and failure-repair usefulness explicitly |
| PR explanations sound polished but miss engineering substance | Validate review usefulness with actual engineers, not just PM taste |

## Why This Proves PM Value

This initiative demonstrates the real work of a strong coding-assistant PM:

- choosing the right assistant surface to win first
- translating trust into repo, diff, test, and review behavior
- aligning product, science, engineering, and GTM around the same bet
- defining success in coding-workflow outcomes, not launch activity

## Read Next

[Scorecard and 90-Day Plan](06-scorecard-and-90-day-plan.md)
