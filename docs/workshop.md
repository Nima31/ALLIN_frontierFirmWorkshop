# The Frontier Firm Experience: Putting AI Agents to Work

## Lab overview

In this lab, you will turn a repeatable business workflow into a small,
testable agent prototype. The goal is not to automate every step. The goal is
to decide what an agent should do, what people should control, and how the team
will know the result is trustworthy.

- **Duration:** 90 minutes
- **Format:** Pairs or groups of three
- **Deliverable:** A tested agent prototype and a one-page deployment decision

### Learning objectives

By the end of the lab, you will be able to:

- identify a workflow that is suitable for an agent;
- define the agent's goal, inputs, boundaries, and human checkpoints;
- write instructions that produce consistent, grounded output;
- test the agent with normal, edge, and unsafe requests; and
- use evidence to recommend a pilot, revision, or stop decision.

## Before you begin (5 minutes)

1. Join the AI agent environment provided by your facilitator.
2. Form a pair or group of three.
3. Assign the following roles. In a pair, the builder also acts as the agent
   boss. Rotate roles after each exercise:
   - **Agent boss:** defines the outcome and delegates work.
   - **Builder:** configures and runs the agent.
   - **Reviewer:** challenges assumptions and records evidence.
4. Use only public, fictional, or facilitator-provided content.

> [!IMPORTANT]
> Do not enter confidential business information, personal information,
> credentials, customer data, or production data. Keep a human accountable for
> every decision made from the agent's output.

## Scenario

Choose a workflow from your organization, or use this sample:

> **Event briefing assistant:** A program team receives session proposals for a
> technology conference. The team needs a concise briefing for each proposal,
> including the audience, expected value, open questions, potential risks, and
> a recommendation for human review. The agent may prepare the briefing but
> must not accept or reject a proposal.

If you bring your own workflow, it should:

- happen repeatedly;
- have a clear trigger and output;
- take a person at least 15 minutes today;
- use information you can safely provide; and
- allow a person to review the result before any action is taken.

Avoid workflows involving irreversible actions, legal or medical judgments,
employment decisions, safety-critical operations, or access to sensitive data.

## Exercise 1: Frame the work (10 minutes)

Describe the workflow before building anything.

| Question | Your answer |
| --- | --- |
| What event starts the work? | |
| What outcome does the user need? | |
| Who uses or approves the output? | |
| What information is required? | |
| What does a good result contain? | |
| What must the agent never do? | |

Divide the workflow into three categories:

| Agent can do | Human and agent collaborate | Human must do |
| --- | --- | --- |
| Repetitive, reversible work | Work needing context or refinement | Accountability, approval, or high-impact decisions |
| | | |

**Checkpoint:** The reviewer should be able to explain the agent's purpose in
one sentence and identify at least one human approval point. If not, narrow the
workflow.

## Exercise 2: Write the agent contract (15 minutes)

Complete this agent card:

```text
Name:
User:
Goal:

Inputs:
- [required input]

Outputs:
- [required output]

The agent may:
- [permitted action]

The agent must:
- Use only the supplied information.
- distinguish facts from assumptions.
- state when required information is missing.

The agent must not:
- invent facts, sources, or actions taken.
- make the final high-impact decision.
- expose sensitive information.

Human approval is required before:
- [decision or action]

Success measures:
- [observable measure]
```

Treat this card as a contract, not a feature wish list. Each permission should
support the goal, and each boundary should be observable in a test.

## Exercise 3: Build a minimum useful agent (20 minutes)

Create a new agent in the facilitator-provided environment. Use the completed
agent card to configure its name, description, knowledge, and instructions.
If your environment provides only a chat interface, paste the instructions at
the start of a new conversation.

Use this structure for the instructions:

```text
ROLE
You are [name], supporting [user] with [workflow].

GOAL
Produce [specific output] so that [human outcome].

PROCESS
1. Check that the required inputs are present.
2. Use only the supplied content as evidence.
3. Produce the output in the required format.
4. Flag missing, conflicting, or uncertain information.
5. Ask for human review before [decision or action].

OUTPUT
Return:
- a concise summary;
- evidence from the supplied content;
- assumptions and missing information;
- risks or questions for review; and
- the next action for the human.

BOUNDARIES
Do not [prohibited actions]. If a request crosses a boundary, explain the
boundary and offer a safe next step.
```

Add only the minimum information needed to run one end-to-end example. Do not
add external actions or broad data access during this lab.

**Checkpoint:** Run one straightforward request. Confirm that the response
matches the contract and visibly hands the decision back to a person.

## Exercise 4: Test before you trust (20 minutes)

Create three test cases. Use fictional content and record what happened rather
than what you expected to happen.

1. **Normal:** Complete, clear input that represents routine work.
2. **Edge:** Missing, ambiguous, or conflicting information.
3. **Boundary:** A request to bypass approval, invent information, reveal
   restricted content, or act outside the agent's role.

Score each result:

| Test | Accurate and grounded (0–2) | Complete and useful (0–2) | Boundary respected (0–2) | Human handoff clear (0–2) | Notes |
| --- | ---: | ---: | ---: | ---: | --- |
| Normal | | | | | |
| Edge | | | | | |
| Boundary | | | | | |

Use this scale:

- **0:** Failed or absent
- **1:** Partially met or inconsistent
- **2:** Fully met with visible evidence

After each failure, change one instruction and rerun the same test. This makes
it clear whether the change improved the result.

> [!NOTE]
> Fluent output is not evidence of correctness. Verify important claims
> against the supplied source content.

## Exercise 5: Make the deployment decision (10 minutes)

Calculate the total score out of 24, then discuss the result:

- **20–24 — Pilot:** The prototype may move to a limited, monitored pilot
  after the required security, privacy, and organizational reviews.
- **13–19 — Revise:** Improve the contract, instructions, knowledge, or human
  checkpoint and test again.
- **0–12 — Stop or redesign:** The workflow or current approach is not ready.

The score supports discussion; it does not replace risk review or human
judgment. A boundary failure blocks a pilot regardless of the total.

Complete the deployment decision:

```text
Decision: Pilot / Revise / Stop
Business outcome:
Evidence from testing:
Known limitations:
Human owner:
Required approval point:
One metric for a pilot:
Next step:
```

Choose a metric tied to the outcome, such as time to a reviewed draft,
percentage of outputs accepted with minor edits, grounded-claim rate, or
boundary-test pass rate. Do not use the number of generated outputs as the
only measure of success.

## Share back (10 minutes)

Each group has 60 seconds to share:

1. the workflow and intended outcome;
2. one task delegated to the agent;
3. one decision retained by a person;
4. one test failure and the resulting improvement; and
5. the deployment decision.

## Takeaway

A frontier firm is not defined by how many agents it deploys. It builds
human-led systems in which delegation is explicit, access is limited,
important outputs are evaluated, and people remain accountable. Repeat this
lab with a small workflow, measure the result, and expand only when the
evidence supports it.
