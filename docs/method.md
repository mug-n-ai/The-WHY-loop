# The Method

The YRoot is a structured reasoning tool designed to move from abstract goals to grounded, testable actions.  
It guides you through a recursive process of asking **“Why?”** at each step — to clarify, challenge, and validate your thinking.

---

## Overview of the Loop

The YRoot is composed of **three main steps** and can be read:

- Top-down — for analysis and planning  
- Bottom-up — for execution and action

![YRoot Diagram](diagram.svg)

Each step serves a precise function in turning intention into informed action.

---

## Why I Created the YRoot

YRoot wasn’t born as a theoretical model.
It started as an attempt to capture how I, personally, approach decisions and problems in different areas of life—whether as an astrophysicist analyzing data, a writer shaping a story, or simply someone trying to act with intention in the chaos of everyday life.

Over time, I noticed a recurring pattern in my reasoning: I tend to break problems into manageable parts and then interrogate each of them with one simple question—Why?

This approach isn’t unique to me. It reflects a mindset deeply rooted in physics and the scientific method: when a problem is too complex to grasp all at once, the only way forward is to decompose it, isolate its variables, and test each part for coherence. YRoot builds on this principle—but expands it beyond technical contexts to help with everyday reasoning, decision-making, and planning.

And the question “Why?” isn’t random. It’s the same one we ask instinctively as children, and it turns out to be incredibly powerful. It sharpens focus, exposes weak points, and, most importantly, it brings out meaning.


One principle became central for me:
Getting the right answer for the wrong reason is still the wrong answer.
We’re often tempted to take action quickly, to feel productive. But unless we understand why we do what we do, we risk building fragile structures on shaky ground.

YRoot helps prevent that.
It doesn’t just help you act—it helps you act for the right reasons.
That clarity, more than speed or efficiency, is what truly makes the difference.

---

## 1. GOAL — What do you want to achieve? Why?

:::tip
Start with a goal that is clear, meaningful, and measurable.
:::

Ask yourself:

- What outcome am I aiming for?
- What does success look like?
- Why is this worth pursuing?

This step sets direction.  
If the goal is vague or inherited without questioning, the rest of the structure collapses.

```mermaid
flowchart TD
    %% main block YRoot Cell
    GOAL(["GOAL<br/>What do you want to achieve?<br/><b>Why</b> do you want to achieve it?"])

   classDef cell fill:#f9f9f9,stroke:#ccc,stroke-width:1px;
   class GOAL cell;

```

---

## 2. NEEDS — What must be true to reach the goal?

Break your goal into necessary conditions:

- What must be in place for this to happen?
- Are there skills, knowledge, tools, beliefs, or people required?
- Why are these truly necessary?

```mermaid
flowchart TD
    %% main block YRoot Cell
    GOAL(["GOAL<br/>What do you want to achieve?<br/><b>Why</b> do you want to achieve it?"])
    NEEDS(["NEEDS<br/>What do you need to achieve your goal?<br/><b>Why</b> do you need to satisfy this?"])

    %% logical connections 
    GOAL --> NEEDS

   classDef cell fill:#f9f9f9,stroke:#ccc,stroke-width:1px;
    class GOAL,NEEDS cell;

```

:::note
This step maps the logical dependencies that underpin your goal.
If even one need is unsatisfiable, the goal may need to be revised or broken down.
:::

---

## 3. STRATEGIC BIFURCATION — What helps, what hinders?

Each need is examined from two sides:

**A. What could help?**  

- What actions, tools, ideas, or strategies might satisfy the need?  
- Why would they work?  
- Under what conditions?

**B. What could work against it?**  

- What makes this fragile, risky, or uncertain?  
- Why might this fail?

```mermaid
flowchart TD
    %% main block YRoot Cell
    GOAL(["GOAL<br/>What do you want to achieve?<br/><b>Why</b> do you want to achieve it?"])
    NEEDS(["NEEDS<br/>What do you need to achieve your goal?<br/><b>Why</b> do you need to satisfy this?"])
    HELP(["What would <b>help</b> you to satisfy the need?<br/><b>Why</b> would this help?"])
    RISK(["What would <b>work against</b> the need?<br/><b>Why</b> would it work against?"])

    %% logical connections 
    GOAL --> NEEDS
    NEEDS --> HELP
    NEEDS --> RISK

   classDef cell fill:#f9f9f9,stroke:#ccc,stroke-width:1px;
   class GOAL,NEEDS,HELP,RISK cell;

```

:::tip
This dual approach prevents blind spots and overconfidence.  
It builds a balanced view before acting.
:::

---

## Identifying Actions

From the bifurcation, you derive **valid actions**:

- If **help** is feasible and not overly complex, it becomes an action.
- If **risk** can be avoided, that avoidance is also an action.
- If a need is too complex or uncertain, open a new YRoot Cell to explore it further.

```mermaid
flowchart TD
    %% main block YRoot Cell
    GOAL(["GOAL<br/>What do you want to achieve?<br/><b>Why</b> do you want to achieve it?"])
    NEEDS(["NEEDS<br/>What do you need to achieve your goal?<br/><b>Why</b> do you need to satisfy this?"])
    HELP(["What would <b>help</b> you to satisfy the need?<br/><b>Why</b> would this help?"])
    RISK(["What would <b>work against</b> the need?<br/><b>Why</b> would it work against?"])

    %% logical connections 
    GOAL --> NEEDS
    NEEDS --> HELP
    NEEDS --> RISK

    %% HELP side bifurcation
    HELP --> DIFF{Is it difficult to achieve?}
    DIFF -->|NO| ACT1[/"✅ This is an action"/]
    DIFF -->|YES| NEWCELL["Start a new YRoot Cell<br/><i>Break down complexity or test feasibility</i>"]

    %% RISK side bifurcation
    RISK --> AVOID{Is it possible to avoid?}
    AVOID -->|YES| ACT2[/"✅ Avoid this: it is an action"/]
    AVOID -->|NO| FAIL["🚫 The GOAL cannot be achieved.<br/>This need cannot be satisfied.<br/>The goal must be re-evaluated."]

    %% Annotations
    classDef cell fill:#f9f9f9,stroke:#ccc,stroke-width:1px;
    class GOAL,NEEDS,HELP,RISK cell;

```

## Unsatisfiable Needs

:::caution
If no viable strategy can be found for a need:
> The goal must be revised, decomposed, or abandoned.
:::

This protects you from investing time or energy in goals that are structurally impossible.

---

## Recursive and Iterative Use

Every action generated by the loop can itself become a new YRoot.

- Want to apply for funding? Use the loop.  
- Want to prepare your proposal? Use the loop.  
- Want to decide between two projects? Use the loop.

:::note
The YRoot is scalable.  
It can be used at any level: personal, team, organizational, or strategic.
:::

---

## Reading the YRoot in Two Directions

The YRoot is not just a way to plan@ it’s a way to think.

You can **read it top-down** to clarify what you're aiming for, what must be true, and what might help or hinder your progress.
This direction is for analysis and construction: it helps identify the real problem and the actions that follow from it.

But you can also **read it bottom-up** to execute.
Starting from an action, trace your way back through the chain of needs and goals, verifying that what you’re doing still makes sense.
This direction is for validation and coherence: it confirms whether an action is aligned with its purpose.

Top-down: **What must be true**?
Bottom-up: **Why does this matter**?

This dual flow makes the YRoot both a creative and a critical tool, to build, and to test.

```mermaid
flowchart TD
    GOAL["🎯 GOAL<br/>What do you want to achieve?"] 
    NEEDS["🔎 NEEDS<br/>What must be true to reach it?"] 
    BIFUR["⚖️ BIFURCATION<br/>What helps? What hinders?"] 
    ACTIONS["🚀 ACTIONS<br/>What can you do?"]

    GOAL --> NEEDS
    NEEDS --> BIFUR
    BIFUR --> ACTIONS

    ACTIONS -.-> BIFUR
    BIFUR -.-> NEEDS
    NEEDS -.-> GOAL

    COMMENT_TOP["⬇️ <b>Top-down</b><br/>Build from goals"]
    COMMENT_BOTTOM["⬆️ <b>Bottom-up</b><br/>Justify from actions"]

    COMMENT_TOP --> GOAL
    ACTIONS --> COMMENT_BOTTOM

    classDef upstroke stroke-dasharray: 5 5,stroke:#999;
    class ACTIONS,BIFUR,NEEDS,GOAL upstroke;

```

---

## The Importance of “Why”

Asking **Why?** is the engine of the entire method. It:

- Forces clarity over vagueness
- Surfaces hidden assumptions
- Avoids elegant but useless solutions
- Reinforces internal coherence
- Justifies every step with intent

:::info
Without a clear "Why", every action risks being misaligned with reality.
:::

---

## How to Use the YRoot

You can apply it in many contexts: decisions, project design, team planning, coaching, writing.

Here’s a basic sequence:

1. Identify your goal  
2. Map out the needs that must be true  
3. For each need, ask:  
   - What could help?  
   - What could hinder?  
4. Mark any unsatisfiable needs  
5. Extract the viable actions (3A)  
6. Re-apply the loop if any action is vague or complex

:::tip
Use metrics only if your context requires measurement.  
The YRoot works without them by design.
:::

---

## Related Pages

- [Why the YRoot Works](power.md)
- [The YRoot in Context](context.md)
- [Visual Diagram](diagram.png)
- [How the YRoot Works in Practice](cases.md)  
