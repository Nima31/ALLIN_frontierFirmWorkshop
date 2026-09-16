# ALL IN Workshop — Your Lab Instructions


You've just been told that **capability without integration is theatre**, and that reasoning doesn't come from the model alone — it comes from how well context, decisions and actions get captured and embedded into the work. That was the claim. **This session is where it gets tested instead of asserted.**

Over the next ~45 minutes you'll get an answer out of an agent that you'd be willing to put your name on — then take it apart to work out **which half came from the model and which half came from the plumbing.**

Two things have to be true for any of this to work: **the facts have to be reachable, and something has to be able to read across them.** Neither alone is enough. Most people credit the model for both. By the end of this session you'll be able to tell them apart — in your own work, not just in ours.


### What you'll walk out with

1. **A method for redesigning one of your own processes to be AI-first** 
2. The **unit cost** of running work this way

### Redesigning a process to be AI-first

The question most people ask is *"where can I add AI to this?"* That's the trap. Adding an agent to a process you haven't changed just makes the existing dysfunction run faster — and you'll see exactly that happen in Step 3.

You'll run the four moves yourself today, in order. **The order is the method.**

| | Move | Why it comes here |
|---|---|---|
| **1** | **Make the work visible** | Write down the real process, not the documented one — including every point where you stop and wait. Next to each wait, note *why* it's there |
| **2** | **De-waste before you automate** | Remove steps rather than speeding them up. A step you delete is worth more than a step you accelerate |
| **3** | **Make the facts reachable** | Until they are, no agent fixes the waiting. This is usually the largest piece of work and the one people skip |
| **4** | **Reorder — don't just accelerate** | Move validation *before* commitment. That single change is what makes the answer trustworthy, and it isn't a speed improvement at all |

Then grade your result against three buckets:

- A step that got **faster** → that's automation
- A step that **disappeared** → that's redesign
- Something you **could not do at all before** → that's new capability

Follow the steps in order. Your facilitators and experts are circulating — raise your hand any time.

---

## Story

The scenario is a costume. Wear it for an hour.

**The company** — Maison Boréal Holding, a Québec beverage group founded in 1998. *(fictional)*

**You are** — the FP&A lead for your division.

**The situation** — Monday is the group quarterly business review. You have **twenty minutes in front of the holding board**.

**Your mission**

1. **Explain the gap** — your revenue is growing, but your margin rate is falling. Why?
2. **Compare** your division with the group. Are you the outlier, or the pattern?
3. **Validate** the explanation against operational evidence before you commit to it.

> The margin question is the test, not the subject. What you're really measuring is what an agent needed in order to answer it — and whether you'd defend the answer in front of people who can check it.

**How you'll work** — teams of 1-3. Each team members on one lab.

---

## Step 0 — Set up your lab (before we start)

1. **Open Copilot Cowork** and login using the user credential 👉 **https://copilot.microsoft.com/**
2. **Enable the Fabric IQ** by turning the Toggle on  under Cowork - Customize - fabric IQ
![alt text](image-1.png)

✅ **You're ready when:** you're logged into the lab and Copilot Cowork is open and waiting for a prompt.

---

## Step 0.5 — Read the old way *(5 min)*

**Before you touch Cowork.** Nothing to hand out and nothing to fill in. **The map is on the screen.** Your table just has to answer three questions out loud.

### First, the shape of the problem

Strip away the finance vocabulary and this is a situation everyone has been in:

> **You need an answer. The facts live in four different places. Three of those places belong to other people. Other people run on their own clock. The deadline doesn't move.**

A student chasing three teammates the night before a submission. A founder waiting on a customer to confirm a number. A consultant who can't finish the recommendation until the client sends the export. Same shape, different costumes.

### What to do — three questions, called out

Look at **The old way** on screen: how an FP&A lead answers this question today, with no AI. Talk it through at your table, then share your answers when asked.
![alt text](image-3.png)

| | Question | You're looking for |
|---|---|---|
| **1** | **How many times does the work stop because you're waiting on another person?** | a count |
| **2** | **Which step number is where the answer gets decided?** | one number |
| **3** | **Which step numbers are where the evidence arrives?** | one or two numbers |

And for each wait you counted, say *why* it's there. The answer is almost always the same: **the facts exist, but you can't reach them yourself.**

### Then compare your two numbers

**Is the decision number bigger or smaller than the evidence numbers?**

That's the finding, and it isn't about finance. In the old way the evidence lands *after* the view is already formed — so it stops testing the answer and starts decorating it.

### ✍️ Write down two numbers

Anywhere — a notepad, a file in that VM, or just remember them. **The decision step, and the first evidence step.** You'll want them in Step 3.

### One round of the table *(60 seconds)*

One sentence each :

> *"The last time I had to decide something before all the facts arrived was…"*

✅ **You're done when:** your table has captured the three answers, everyone has seen the two numbers are in the wrong order, and each person has named their own version of it.

> Making the work visible is the first move in any transformation. You can't see what changed if you never looked at where you started.

---

## Step 1 — Launch your financial investigation *(10 min)*

### What to do

1. **Copy the prompt below into Copilot Cowork.**
   ⚠️ **Do not attach any files.** Let Cowork go and find what it needs.
2. **Let it work.** While it runs, watch **what it goes looking for and where**.
3. **Read the result carefully** — the analysis, the **sources it cites**, and the explanation it builds.
4. **Discuss it as a team** using the questions below.

### 📋 Prompt 01 — copy this

```text
I'm the FP&A lead for my division at Maison Boréal. Monday is the group quarterly
business review and I have twenty minutes in front of the holding board.

Go and find what you need. My division's operating detail is in my files. The group's
consolidated financials are in the Boréal Holding reporting model I have access to;
treat that as the source of truth for anything financial and don't recalculate it
yourself.

Here's what I actually need to know. My revenue grew this quarter and my margin rate
fell. I don't yet know whether that's my problem or the group's problem. Work out what
happened, whether my division is the outlier or the pattern, and what's really driving
it — then pressure-test your theory against my operations notes and customer feedback
before you commit to it.

Add a clear title at the beginning of the response that explicitly names the products
covered by the analysis, such as apples, oranges, bananas, or any other products
identified in the source data.
```

### 💬 Discuss — Explore. Compare. Challenge.

- What is the analysis telling us?
- What evidence supports this explanation?
- **What did it have to be able to reach for this to work at all?** Name the sources.
- What are we confident about, and what remains a hypothesis?
- What information is missing to validate the conclusion?

✅ **You're done when:** your team can state, in one sentence, what drove the margin decline — and name the evidence behind it.

---

## Step 2 — Turn your analysis into an interactive dashboard *(10 min)*

### What to do

1. Once your analysis is available, **enter the second prompt** in the same conversation.
2. **Open the generated dashboard.**
3. **Explore it** — click through, compare, and dig further into the findings.
4. **Discuss the dashboard** as a team.

### 📋 Prompt 02 — copy this

```text
Create an interactive dashboard.
```

### 💬 Discuss — Explore. Compare. Challenge.

- What does the dashboard make easier to understand?
- Do the findings remain consistent with the underlying evidence?
- Does anything in the dashboard change or challenge our initial interpretation?
- **Could a standard BI report have answered your Step 1 question?** If yes, which part? If no, why not?

✅ **You're done when:** you've explored the dashboard and agreed whether it confirms or challenges your Step 1 conclusion.

---

## Step 3 — Live demo & group share *(12 min)*

No prompt to run in this step. **Watch, compare, and speak up.**

### What to do

1. **Watch the live demonstration** on screen.
2. **Compare it against your own result.** Look especially at how these change the outcome:
   - the **data** available and the **period** covered
   - the **scope** of the question
   - the **tools** Cowork had access to
   - the **user's permissions** — two people can ask the same question and get different answers
3. **Be ready to share.** 2–3 teams will be invited to present their findings and any differences they noticed.
4. **Ask your questions** — the floor opens for Q&A.

### 💬 Think about

- Where did our result differ from the demo — and why?
- What in the setup (data, period, scope, permissions) explains the difference?

### 📊 The scorecard — filled in together, on screen

One scorecard for the whole room.

| | **A** · The old way<br><sub>from Step 0.5</sub> | **B** · The old way + an assistant<br><sub>same steps, AI drafts the deck</sub> | **C** · What you just did |
|---|---|---|---|
| Elapsed time | `5 days` | ? | ? |
| Times you stopped and waited | `3` | ? | ? |
| Evidence checked **before** or **after** you decided? | `after` | ? | ? |
| One thing you **could not do at all** | | | |

**Column A is already answered** — those are the numbers you called out in Step 0.5. Fill in B and C from the room.

### 🔍 The main event — what actually removed each thing?

**This is the part to get right.** The time savings are the headline; this is the finding.

**Get out of your chair for this one.**

Your table has **1–2 post-its**. Each one is a step that disappeared between column A and column C. **Decide as a table which bucket it belongs in, then send one person to the front to stick it up.**

| | Bucket | The test |
|---|---|---|
| 🗄️ | **The facts became reachable** | Would this step still have gone away if a well-built data platform had existed — and **no AI at all**? |
| 🤖 | **Something could read across them** | Does this step need judgement, or reading something written in prose, or forming a theory and then attacking it? |

**Argue about it before you send your runner.** The argument is the exercise — the post-it is just the receipt.

> Speeding up a step is automation. Removing a step is redesign. Doing something you couldn't do before is new capability. It's probably all three, in different places — and they don't all come from the same source.

---

## Step 4 — Assess the value *(10 min)*

Your result has value. What did it take to produce it?

### What to do

1. **Enter the prompt below** in Copilot Cowork.
2. **Observe** the metrics and units actually displayed — read what's really there.
3. **Compare**: time saved · output quality · human review effort.
4. **Decide**: is this a useful, sustainable workflow?

### 📋 Prompt 03 — copy this

```text
/Cost
```

### 💬 Discuss

- What value did this approach create?
- What human review or correction was still required?
- **What isn't in this number?** The reporting model, the permissions, the connected sources — none of that shows up in `/Cost`, and none of it was free.
- Would this be a workflow worth repeating?

### Good to know — where the cost comes from

Copilot credits reflect four inputs *(1 credit = $0.01)*:

| Input | What it covers |
|---|---|
| **Models** | The AI model chosen for each task — it varies with the quality, speed and cost the task demands |
| **Context** | Understanding of the people, roles and collaboration behind the work — from emails, files, meetings and past interactions |
| **Tools** | Actions taken to get work done: sending emails, scheduling meetings, updating documents |
| **Runtime** | Managed cloud orchestration that runs agents and keeps them working, including long-running tasks |

**And the cost that isn't shown:** getting the facts reachable in the first place. That work happened before you sat down, and for most organizations it's the larger of the two bills.

### Wrap-up — the box you're actually in
Before you go, find yourself on this grid. Not Maison Boréal. **You.**

| | **No AI** | **With AI** |
|---|---|---|
| **Facts not reachable** | **The old way**<br>Slow, and the evidence arrives too late to matter | **Confident nonsense**<br>Fast, fluent, unsupported — where a lot of AI work actually is |
| **Facts reachable** | **Self-serve BI**<br>Good — but only for questions someone already modelled | **What you just did**<br>Twenty minutes, and defensible |

**Neither axis alone gets you to the bottom-right.** Data readiness buys back the elapsed time. AI buys back the hours — and removes the requirement that somebody anticipated your question. Move on one axis only and you land in a box nobody wants.

> The takeaway isn't "AI is fast." It's that **the model was never the hard part** — and now you know how to tell which half of your own problem is which.

