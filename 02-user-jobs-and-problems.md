# User Jobs and Problems

## Question This File Answers

Whose jobs matter most, and what problem is actually worth solving?

## PM Skills Demonstrated

- `jobs-to-be-done`: identifies the functional, social, and emotional jobs across developers, leads, and enterprise stakeholders
- `problem-statement`: frames the adoption and trust problem without solution smuggling
- `proto-persona`: keeps the user set specific enough to be actionable rather than generic "developers"

## Primary Users and Stakeholders

This category succeeds only if it works for more than one actor.

| Actor | Why they matter |
|---|---|
| Individual developer | Creates pull, habit, and daily usage truth |
| Tech lead or engineering manager | Decides whether the product improves or degrades team output |
| Platform, security, or tooling lead | Determines whether rollout feels safe and supportable |
| Enterprise buyer | Converts trusted usage into budget and expansion |

## Primary Workflow Map

The product is not one generic AI moment. It sits across a concrete development loop:

1. Understand the task, issue, or failing behavior
2. Pull the right repo and file context
3. Propose or apply a code diff
4. Run or repair tests and fix failures
5. Explain changes clearly enough for review
6. Help the developer prepare or respond in a PR flow

This workflow map is where product strategy should live.

## Jobs-To-Be-Done

This section follows the logic of the local `jobs-to-be-done` skill.

### 1. Individual developer

**Functional jobs**
- Draft, edit, and refactor code without losing repo context
- Debug faster when the failure mode is unclear
- Prepare tests, docs, or review notes with less manual setup
- Move from issue or task to review-ready diff with less context switching

**Social jobs**
- Look competent and fast without appearing careless
- Contribute at senior quality even when the problem space is messy

**Emotional jobs**
- Feel confident that using the assistant is helping, not adding hidden cleanup
- Avoid the anxiety of shipping AI-assisted mistakes into a shared codebase

### 2. Tech lead or engineering manager

**Functional jobs**
- Improve team throughput without lowering code quality
- Introduce assistance in a way that aligns with standards and review practices
- See where the tool is helping versus creating rework
- Understand whether the assistant improves merge-ready output or just creates cleanup

**Social jobs**
- Be seen as modern and pragmatic, not reckless or gullible

**Emotional jobs**
- Feel in control of the rollout rather than surprised by it

### 3. Platform, security, or tooling lead

**Functional jobs**
- Understand what the assistant can access, change, and suggest
- Reduce policy and governance friction during rollout
- Support usage without creating a parallel operational burden
- Know how the assistant behaves across IDE, repo, terminal, and PR surfaces

**Social jobs**
- Be seen as enabling progress without compromising guardrails

**Emotional jobs**
- Avoid becoming the team that has to clean up product shortcuts later

## The Core Problem Statement

This section follows the logic of the local `problem-statement` skill.

**I am:** a software team trying to increase coding speed without losing control of code quality, standards, or review trust.

**Trying to:** use AI assistance for real development work such as repo-aware edits, debugging, test repair, and PR support.

**But:** current products often feel strong in demos and uneven in live workflows. Developers do not always trust the output, leads cannot always see the value clearly, and rollout owners worry about quality drift or governance risk.

**Because:** the product experience, trust signals, and rollout model are not yet designed tightly enough around how software teams actually code and ship.

**Which makes us feel:** interested but cautious, excited but unconvinced, and unwilling to standardize on the tool until it proves itself.

## Final Problem Statement

Software teams need an AI coding assistant that helps them move from task to review-ready code inside real repository workflows, because current category experiences often generate code but do not reliably support editing, debugging, testing, and review with enough trust for standard team adoption.

## What This Means For Product Strategy

The product does not need to solve every coding job first.

It needs to win where three conditions overlap:

1. The workflow is frequent enough to create habit.
2. Trust can be earned through product behavior.
3. Team-level rollout value can be made visible.

## Wedge Recommendation

I would start with the workflows where trust and utility can compound:

- repo-aware code edits
- debugging and fix iteration
- test generation and repair
- review preparation, PR summaries, and review-response assistance

These are stronger wedge candidates than broad "do anything in code" positioning because they:

- happen repeatedly
- surface quality quickly
- allow better evaluation design
- connect more directly to team standards

## Anti-Patterns

### Building for generic "developers"

The category looks broad, but the work is too different across junior devs, staff engineers, startups, and regulated teams for vague persona language to be useful.

### Treating trust as a compliance checklist

Trust is experienced in use, not inferred from policy language.

### Mistaking one user's delight for organizational readiness

Solo enthusiasm matters, but it does not prove rollout readiness.

## Read Next

[Strategy, GTM, and Operating Model](03-strategy-gtm-and-operating-model.md)
