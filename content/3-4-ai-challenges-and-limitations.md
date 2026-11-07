# Stage 1: Challenges and Limitations of Behaviorist AI

## Learning Goals

By the end of this stage, you will be able to:

1. Explain basic principles of how AI models use data to generate predictions.
2. Identify the main challenges of Behaviorist AI.
3. Describe the limitations of the technology.

**Topics covered:**

- Challenges (reward design, exploration vs. exploitation, data and computing cost)
- Limitations (safety, generalization, explainability)

---

# 6.3 Challenges and Limitations

## Introduction

### Explanation

**Behaviorist AI** (also called **behavioral AI**) is a kind of AI where a program, called an **agent**, learns how to act by **trying things out and getting feedback**. The feedback is usually a **reward** (a score for a good action) or a **penalty** (a negative score for a bad action). Robots, game characters (called **NPCs**, or non-player characters), and self-driving cars can all learn this way.

This kind of AI is growing quickly, but it still has important problems. In this chapter, we split them into two groups:

| Group | Meaning | Topics |
|-------|---------|--------|
| **Challenges** | Difficulties that make it **hard or costly to build** these systems | Reward design, exploration vs. exploitation, data and computing cost |
| **Limitations** | Weak spots that remain **even after** a system is built | Safety, generalization, explainability |

[insert image about a behaviorist AI agent learning from rewards and facing challenges and limitations]

### Worked Example

**Task:** A company builds a robot that learns to deliver packages. Sort these problems into *challenges* or *limitations*.

| Problem | Group |
|---------|-------|
| It is hard to decide how many points the robot should earn for each action | Challenge (reward design) |
| Training the robot takes weeks of computer time | Challenge (computing cost) |
| The robot works in the office but gets confused in a new building | Limitation (generalization) |

### Activity

Is each problem a **challenge** or a **limitation**?

a. Collecting enough training data is very expensive.
b. A trained robot makes a dangerous choice that nobody expected.
c. Nobody can explain why the robot chose a certain path.

<details>
<summary><b>Answer</b></summary>

a. **Challenge** (data cost)
b. **Limitation** (safety)
c. **Limitation** (explainability)

</details>

---

# Challenges

## Reward Design

### Explanation

**Reward design** (also called **reward shaping**) means deciding **what rewards and penalties the agent gets** for its actions. This is hard because the agent only learns what the reward tells it. If the reward is badly designed, the agent may find a **shortcut** that earns lots of points but does **not** do what we really wanted. This can lead to **suboptimal behavior** (behavior that works, but is not the best) or **unintended consequences** (results nobody planned).

A good reward should:

- Match the **real goal**, not just something easy to measure.
- Not be **easy to cheat**.
- Give feedback often enough for the agent to learn.

[insert image about a robot earning points by taking a shortcut instead of reaching the real goal]

### Worked Example

**Task:** A robot vacuum is rewarded **+1 for every piece of dust it collects**.

| What we wanted | What the robot may actually do |
|----------------|--------------------------------|
| A clean room | Dump the dust out, then collect it again and again to earn more points |

**Fix:** Change the reward so the robot earns points for **the room being clean at the end**, instead of for each piece collected.

### Activity

A game character is rewarded **+10 for every coin it touches**. It learns to run in circles around one coin that keeps reappearing.

a. What did we really want the character to do?
b. Why did the reward fail?
c. Suggest a better reward.

<details>
<summary><b>Answer</b></summary>

a. We wanted it to **finish the level** (for example, explore and reach the goal).
b. The reward was easy to cheat: touching the same coin again and again gave points without making progress.
c. Examples: give a large reward for reaching the end of the level, or give coin points only the **first** time each coin is collected.

</details>

---

## Exploration vs. Exploitation

### Explanation

Every agent has to balance two choices:

- **Exploration**: Trying **new** actions to discover whether they work better.
- **Exploitation**: Using the action that is **already known** to give a good reward.

This is a challenge because the agent cannot be sure which choice is better. If it explores too much, it wastes time and makes many mistakes. If it exploits too much, it may never find a better way. In the real world, exploring can also be **expensive or risky** (for example, a robot that tries a random move might break something).

[insert image about exploring a new path versus taking the known best path]

### Worked Example

**Task:** A delivery robot knows Route A takes 10 minutes. It has never tried Route B.

| Choice | Type | Possible outcome |
|--------|------|------------------|
| Always take Route A | Exploitation | A steady 10 minutes, but it might miss a 6-minute route |
| Try Route B sometimes | Exploration | It might find a faster way, or a slower one |

A balanced plan is to take Route A most of the time and try Route B once in a while.

### Activity

A music app learns what songs you like. For each case, say whether it is **exploring** or **exploiting**:

a. It plays your most-played song again.
b. It plays a song from a style you have never listened to.

<details>
<summary><b>Answer</b></summary>

a. **Exploiting** (using what it already knows you like)
b. **Exploring** (testing something new to learn more)

</details>

---

## Data and Computing Cost

### Explanation

**Data dependency** means the agent needs **a lot of data** and **continuous feedback** to learn well. In the real world, collecting this data can be **expensive or impractical** (not realistic to do). For example, a robot cannot safely crash a thousand times just to learn how to avoid obstacles.

**Computational complexity** means the algorithms need a lot of **computing power** (the processing ability of a computer) and **time** to learn good behavior. Many reinforcement learning methods repeat the same task thousands or millions of times.

| Problem | What it means | Result |
|---------|---------------|--------|
| **Data dependency** | Needs huge amounts of examples and feedback | High cost, long collection time |
| **Computational complexity** | Needs powerful computers and long run times | High cost, slow progress |

One way to reduce these costs is to train agents inside a **simulation** (a computer program that copies the real world), where trials are cheap and safe.

[insert image about a robot training in a simulation instead of the real world]

### Worked Example

**Task:** An agent needs 1,000,000 practice trials. Each trial takes 2 seconds. How long will training take?

1. Total time = 1,000,000 × 2 seconds = **2,000,000 seconds**
2. One day has 24 × 60 × 60 = **86,400 seconds**
3. Days = 2,000,000 ÷ 86,400 ≈ **23 days**

So even this simple example needs more than three weeks of nonstop practice.

### Activity

An agent needs 500,000 trials, and each trial takes 3 seconds.

a. How many seconds will training take?
b. About how many days is that? (1 day = 86,400 seconds)
c. Give one way to reduce the cost.

<details>
<summary><b>Answer</b></summary>

a. 500,000 × 3 = **1,500,000 seconds**
b. 1,500,000 ÷ 86,400 ≈ **17.4 days**
c. For example: train in a **simulation**, run many trials at the same time on more computers, or reuse data the agent has already collected.

</details>

---

# Limitations

## Safety

### Explanation

In critical areas such as **healthcare**, **autonomous driving** (cars that drive themselves), and **finance**, an AI system must act **reliably**. If the agent shows **unintended behavior** (doing something nobody expected) or makes a wrong decision, people could get hurt or lose money.

There are also **ethical** concerns. **Ethics** means questions of what is right and wrong. For example, who is responsible if an AI system makes a harmful choice?

Ways to improve safety include:

- Testing carefully in simulations before using the AI in the real world.
- Adding **rules the agent can never break** (for example, "never go over the speed limit").
- Keeping a human in charge who can step in.

[insert image about a self-driving car with safety checks and a human supervisor]

### Worked Example

**Task:** A hospital AI suggests medicine doses. Identify the safety risk and a protection.

| Item | Description |
|------|-------------|
| Risk | The AI suggests a wrong dose because it saw an unusual patient it was never trained on |
| Protection | A doctor must **review and approve** every suggestion before it is used |

### Activity

A self-driving car learns by trial and error. Why is it unsafe to let it explore randomly on a real road, and what is a safer option?

<details>
<summary><b>Answer</b></summary>

A random action on a real road could cause an accident and hurt people. A safer option is to let the car do most of its exploring in a **simulation**, and to add fixed safety rules and a human backup for real driving.

</details>

---

## Generalization

### Explanation

**Generalization** is the ability of an AI system to work well in **new situations** that it was not trained on. Behaviorist AI often struggles here. An agent trained in one environment may perform well there but **fail in a different environment or on a different task**. Robots and NPCs may do well in the conditions they practiced in, but fail when they meet something **unfamiliar**.

[insert image about a robot working well in a training room but failing in a new environment]

### Worked Example

**Task:** A robot learns to walk on a smooth indoor floor.

| Situation | Likely result |
|-----------|---------------|
| Smooth indoor floor (same as training) | Walks well |
| Grass, sand, or stairs (new) | May slip, fall, or freeze |

To improve generalization, the robot can practice on many different surfaces during training.

### Activity

A game character is trained on a map with no enemies. It is then placed in a map with many enemies and performs badly.

a. What limitation does this show?
b. How could training be improved?

<details>
<summary><b>Answer</b></summary>

a. **Generalization**: the character could not handle a new situation.
b. Train it on **many different maps**, including ones with enemies, so it learns to deal with variety.

</details>

---

## Explainability

### Explanation

**Explainability** means being able to **understand and explain why** an AI system made a certain decision. Many advanced AI models, such as deep neural networks, work like a **black box**: we can see what goes in and what comes out, but not clearly what happens inside.

This is a limitation because:

- People find it hard to **trust** a decision they cannot understand.
- When something goes wrong, it is hard to find **the cause**.
- In areas like healthcare or finance, people often need a **clear reason** for each decision.

[insert image about a black box AI model where the reasoning is hidden]

### Worked Example

**Task:** A bank's AI rejects a customer's loan request.

| Without explainability | With explainability |
|------------------------|---------------------|
| "The AI said no." | "The loan was rejected because the monthly payments would be more than half of the customer's income." |

The second answer lets the customer understand the decision, and lets the bank check whether the decision was fair.

### Activity

A hospital uses an AI to flag patients at risk. A doctor asks, "Why did it flag this patient?" and nobody can answer.

a. Which limitation is this?
b. Give one reason why it matters.

<details>
<summary><b>Answer</b></summary>

a. **Explainability**
b. For example: the doctor cannot judge if the AI is right, patients may not trust the result, and mistakes are hard to find and fix.

</details>

---

## Summary

- **Behaviorist AI** learns how to act through trial, error, and feedback (rewards and penalties).
- **Challenges** make these systems hard or costly to build:
  - **Reward design**: A badly designed reward can lead to shortcuts and unintended results.
  - **Exploration vs. exploitation**: The agent must balance trying new things with using what it knows.
  - **Data and computing cost**: Training needs large amounts of data, powerful computers, and a lot of time.
- **Limitations** remain even after the system is built:
  - **Safety**: Wrong or unexpected decisions can cause harm in critical areas.
  - **Generalization**: Agents may fail in new environments or tasks.
  - **Explainability**: It is often hard to understand why the AI made a decision.
