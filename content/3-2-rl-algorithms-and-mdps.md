# Reinforcement Learning: MDPs and RL Algorithms

## Learning Goals

By the end of these stages, you will be able to:

1. Explain basic principles of how AI models use data to generate predictions.

| Stage | Topics |
|-------|--------|
| **Stage 1: Markov Decision Processes (MDPs)** | • Markov Decision Process (1): States, Actions, Rewards<br>• Markov Decision Process (2): Policy |
| **Stage 2: RL Algorithms and Techniques** | • Reinforcement Learning Algorithms (overview)<br>• Value-Based (Q-Learning conceptual overview)<br>• Exploration vs. Exploitation |

---

# Background: AI and Machine Learning

## Explanation

**Artificial Intelligence (AI)** is the part of computer science that builds machines and programs able to do tasks that normally need human intelligence, such as understanding language, making decisions, solving problems, and recognizing things they see.

**Machine Learning (ML)** is a part of AI where computers **learn from data** and make predictions, instead of being told exactly what to do for every task. Three key ideas appear in every ML system:

- **Training data**: The examples the computer learns from.
- **Model**: What the computer learns. It is a summary of the patterns found in the data, and it uses those patterns to make predictions.
- **Algorithm**: The step-by-step method the computer follows to learn. It adjusts the model again and again so the predictions get better.

There are three main types of machine learning:

| Type | How it learns | Example |
|------|---------------|---------|
| **Supervised learning** | Learns from **labeled data**, which means examples that already come with the right answer (the **label**). It learns to match inputs to outputs. | Photos labeled "cat" or "dog" teach the model to name new photos |
| **Unsupervised learning** | Learns from **unlabeled data**, with no right answers given. It finds patterns or groups (called **clusters**) on its own. | Grouping customers who buy similar products |
| **Reinforcement learning (RL)** | Learns by **trial and error**, getting rewards for good choices and penalties for bad ones. | A robot learning to walk |

[insert image about supervised learning: labeled shapes train a model, which then predicts test shapes]

[insert image about unsupervised learning: unlabeled data goes into a machine and produces groups]

The main differences between supervised and unsupervised learning:

- Supervised learning **needs labeled data**; unsupervised learning does not.
- Supervised learning is used to **predict an answer**; unsupervised learning is used to **explore and understand** the data.
- Supervised learning uses methods like linear regression and neural networks; unsupervised learning uses methods like k-means clustering.

[insert image about a graph showing supervised learning (line of best fit) next to unsupervised learning (clusters)]

Almost every ML project follows the same **workflow**:

1. **Data collection**: Gather the data needed.
2. **Data preprocessing**: Clean and prepare the data.
3. **Model selection and training**: Pick an algorithm and train the model.
4. **Model evaluation**: Test the model on **unseen data** (data it has not learned from) to check it works well.
5. **Model deployment**: Use the trained model in the real world.

## Worked Example

**Task:** Decide which type of learning fits each problem.

| Problem | Type | Why |
|---------|------|-----|
| Predict whether an email is spam, using thousands of emails already marked "spam" or "not spam" | Supervised | The data has labels |
| Sort news articles into groups of similar topics, with no topics given | Unsupervised | No labels, the model finds groups |
| Teach a program to play a video game by giving points for winning | Reinforcement | Learns from rewards and penalties |

## Activity

Name the type of learning (supervised, unsupervised, or reinforcement) for each case:

a. A model learns to read handwritten numbers from images that each have the correct number attached.
b. A store wants to find groups of similar shoppers, but has no categories ready.
c. A robot vacuum gets a reward each time it cleans a new area without bumping into furniture.

<details>
<summary><b>Answer</b></summary>

a. **Supervised** (labeled examples)
b. **Unsupervised** (no labels, finding groups)
c. **Reinforcement** (learning from rewards and penalties)

</details>

---

# Stage 1: Markov Decision Processes (MDPs)

## Reinforcement Learning in Brief

### Explanation

In reinforcement learning, a program learns by **doing**. It tries something, sees what happens, and gets feedback. The main parts are:

| Part | Meaning | Example (robot learning to walk) |
|------|---------|----------------------------------|
| **Agent** | The decision-maker that learns | The robot |
| **Environment** | The world the agent interacts with | The floor and everything around the robot |
| **State** | The current situation of the environment | The robot's leg positions and balance |
| **Action** | A choice the agent makes in a state | Move the left leg forward |
| **Reward** | Feedback for an action (positive is good, negative is a penalty) | +1 for a step, −5 for a fall |

The agent repeats a loop: it looks at the **state**, picks an **action**, the environment responds, and the agent receives a **reward** and a new state.

[insert image about the reinforcement learning loop: Agent -> Action -> Environment -> Reward and new State -> Agent]

Reinforcement learning has been used in many fields:

- **Games**: Google's **AlphaGo** beat top Go player Lee Sedol in 2016. IBM's **Deep Blue** also beat world chess champion Garry Kasparov in 1997, although Deep Blue relied mostly on searching through moves rather than on learning from rewards.
- **Robotics**: Robots learn to walk by trying movements and being rewarded for steps.
- **Self-driving cars**: Cars learn to drive safely, with rewards for safe driving and penalties for accidents.
- **Finance**: Trading programs learn to make better trades from market data.

[insert image about Deep Blue vs. Garry Kasparov and AlphaGo vs. Lee Sedol]

### Worked Example

**Task:** Identify the parts of reinforcement learning for a self-driving car.

| Part | In this example |
|------|-----------------|
| Agent | The car's driving program |
| Environment | Roads, traffic, and pedestrians |
| State | Current speed, lane, and distance to other cars |
| Action | Speed up, slow down, or turn |
| Reward | Positive for safe driving, negative for accidents or breaking traffic rules |

### Activity

A program learns to play a simple game where it moves a character to collect coins and avoid traps. Name the agent, environment, one possible action, and one possible reward.

<details>
<summary><b>Answer</b></summary>

- **Agent**: the program controlling the character
- **Environment**: the game world with coins and traps
- **Action**: move left, right, up, or down (or jump)
- **Reward**: positive for collecting a coin, negative for hitting a trap

</details>

---

## Markov Decision Process (1): States, Actions, Rewards

### Explanation

A **Markov Decision Process (MDP)** is a mathematical way of describing a decision problem where results are **partly random and partly controlled by the decision-maker**. Reinforcement learning problems are usually written as MDPs.

An MDP has these building blocks:

| Component | Symbol | Meaning |
|-----------|--------|---------|
| **States** | S | All the different situations that can happen |
| **Actions** | A | The choices available in each state |
| **Transition model** | P | The **probability** (chance) of ending up in each new state after taking an action |
| **Reward function** | R | The immediate reward received after an action moves the agent from one state to another |
| **Policy** | π | The strategy for which action to pick in each state (covered in the next section) |

[insert image about the Markov Decision Process components: states, actions, transition model, rewards, policy]

The word **Markov** means that the next state depends only on the **current state** and the action taken, not on everything that happened before.

### Worked Example

**Task:** Describe a traffic light as an MDP.

| Component | Traffic light example |
|-----------|-----------------------|
| **States (S)** | Red, Yellow, Green |
| **Actions (A)** | Stay in the current color, or switch to the next color |
| **Transition model (P)** | Set by rules such as how long each light lasts. For example, if the light is Green and the action is "switch", it moves to Yellow with a probability of 100% |
| **Reward function (R)** | Positive reward when traffic flows smoothly, negative reward when cars are stuck in a long queue |

The goal is to pick actions that keep traffic flowing smoothly.

### Activity

A robot moves along a hallway with three spots: **A**, **B**, and **C**. It can **move right** or **stay**. Reaching spot C gives a reward of +10, and every other step gives −1.

a. List the states.
b. List the actions.
c. What is the reward for moving from A to B?
d. What is the reward for moving from B to C?

<details>
<summary><b>Answer</b></summary>

a. States: **A, B, C**
b. Actions: **move right, stay**
c. **−1** (any step that does not reach C)
d. **+10** (reaching spot C)

</details>

---

## Markov Decision Process (2): Policy

### Explanation

A **policy** is the agent's strategy: a rule that says **which action to take in each state**. It is written as π(S) → a, which reads "in state S, take action a". The best possible policy, which collects the most reward over time, is called the **optimal policy** and is written π*.

To find a good policy, the agent needs to know how good each state is. A **value function** estimates the **total reward the agent can expect to collect in the future** starting from a given state. States that lead to big rewards get high values.

Future rewards are usually counted a little less than immediate ones, because rewards now are more certain. The number used for this is called the **discount factor** (written γ, a value between 0 and 1). The total reward, called the **return**, is:

**Return = R₁ + γ·R₂ + γ²·R₃ + ...**

There are two main methods for solving an MDP:

- **Value iteration**: Update the value of every state again and again until the values stop changing (this is called **convergence**). Then pick the best action for each state.
- **Policy iteration**: Switch between two steps: **evaluate** how good the current policy is, then **improve** it. Repeat until the policy can't be improved.

[insert image about a policy: arrows in each state showing the chosen action]

### Worked Example

**Task:** Work out the return for rewards of 2, 4, and 10 using a discount factor of 0.9.

| Step | Reward | Discount | Value counted |
|------|--------|----------|---------------|
| 1 | 2 | 1 | 2 |
| 2 | 4 | 0.9 | 3.6 |
| 3 | 10 | 0.9 × 0.9 = 0.81 | 8.1 |

Return = 2 + 3.6 + 8.1 = **13.7**

**Policy example (traffic light):**

| State | Policy (action to take) |
|-------|-------------------------|
| Green, and the queue on the other road is long | Switch to Yellow |
| Green, and few cars are waiting | Stay Green |
| Red, and the time is up | Switch to Green |

### Activity

a. A robot gets rewards of 1, 2, and 3 over three steps. With a discount factor of 0.5, what is the return?
b. Write a simple policy for a robot vacuum with two states: **Battery low** and **Battery OK**.

<details>
<summary><b>Answer</b></summary>

a. 1 + (0.5 × 2) + (0.25 × 3) = 1 + 1 + 0.75 = **2.75**

b. One possible policy:

| State | Action |
|-------|--------|
| Battery low | Go back to the charging station |
| Battery OK | Keep cleaning |

Any policy that gives one clear action for each state is correct.

</details>

---

# Stage 2: RL Algorithms and Techniques

## Reinforcement Learning Algorithms (Overview)

### Explanation

In a real problem, the agent usually does **not** know the transition model or rewards ahead of time. It must learn them by playing. A **learning algorithm** is the method the agent uses to update its **policy** and its **value function** based on the rewards it receives.

RL algorithms are often grouped by what they learn:

| Group | What the agent learns | Idea |
|-------|-----------------------|------|
| **Value-based** | How valuable each state or action is | Pick the action with the highest value |
| **Policy-based** | The policy directly | Learn which action to take without first scoring everything |
| **Model-based** | A model of how the environment works | Plan ahead using the model |

In this stage, we focus on the **value-based** group.

[insert image about three groups of RL algorithms: value-based, policy-based, model-based]

### Worked Example

**Task:** Match each description to a group.

| Description | Group |
|-------------|-------|
| "I keep a score for every action and choose the highest one." | Value-based |
| "I learn directly which action to pick in each situation." | Policy-based |
| "I build a map of how the world reacts, then plan with it." | Model-based |

### Activity

Which group does each agent belong to?

a. An agent that writes down a score for every move in a board game and picks the best score.
b. An agent that practices a robot arm movement and directly adjusts its action rules.

<details>
<summary><b>Answer</b></summary>

a. **Value-based**
b. **Policy-based**

</details>

---

## Value-Based Learning: Q-Learning (Conceptual Overview)

### Explanation

**Q-learning** is a popular value-based algorithm. The "Q" stands for **quality**, meaning how good an action is. The agent keeps a table called a **Q-table**, which stores a **Q-value** for every pair of *(state, action)*. A higher Q-value means a better choice.

At first, all Q-values are zero. As the agent plays, it updates the Q-value of the action it just used:

**New Q = Old Q + α × ( Reward + γ × Best next Q − Old Q )**

Here is what each part means:

- **α (alpha)**, the **learning rate**: How much the agent changes its mind after each experience (between 0 and 1).
- **γ (gamma)**, the **discount factor**: How much future rewards matter.
- **Best next Q**: The highest Q-value available in the next state.

In simple words: the agent compares **what it expected** with **what it actually got** and moves its estimate a little closer to the real result.

| State | Action: Left | Action: Right |
|-------|--------------|---------------|
| A | 0 | 0 |
| B | 0 | 0 |
| C | 0 | 0 |

*(An empty Q-table at the start of learning.)*

[insert image about a Q-table being updated as the agent moves between states]

### Worked Example

**Task:** The agent is in state B and takes action "Right". It receives a reward of 10. The best Q-value in the next state is 0. Use α = 0.5, γ = 0.9, and an old Q-value of 0.

1. Calculate the target: Reward + γ × Best next Q = 10 + (0.9 × 0) = **10**
2. Find the difference from the old value: 10 − 0 = **10**
3. Multiply by the learning rate: 0.5 × 10 = **5**
4. New Q = 0 + 5 = **5**

The Q-value for (B, Right) is now **5**, so the agent sees this action as worth taking.

### Activity

The old Q-value for (state C, "Left") is 5. The agent receives a reward of 2, and the best Q-value in the next state is 10. Use α = 0.5 and γ = 0.9. What is the new Q-value?

<details>
<summary><b>Answer</b></summary>

1. Target = 2 + (0.9 × 10) = 2 + 9 = **11**
2. Difference = 11 − 5 = **6**
3. Multiply by α: 0.5 × 6 = **3**
4. New Q = 5 + 3 = **8**

</details>

---

## Exploration vs. Exploitation

### Explanation

An agent faces a tricky choice every time it acts:

- **Exploration**: Try a **new** action to discover whether it might give a better reward.
- **Exploitation**: Choose the action that is **already known** to give a good reward.

If the agent only exploits, it may miss better options. If it only explores, it never takes advantage of what it has learned. A good agent balances the two.

A simple way to balance them is the **ε-greedy** method (ε is the Greek letter *epsilon*). The agent picks a small number ε, such as 0.1:

- With probability **ε** (10% of the time), it **explores** by picking a random action.
- With probability **1 − ε** (90% of the time), it **exploits** by picking the action with the highest Q-value.

Often, ε starts high and becomes smaller as the agent learns more.

[insert image about exploration vs. exploitation: trying a new path versus taking the known best path]

### Worked Example

**Task:** You are choosing where to eat lunch. Your favorite café gives a reward of 8 out of 10 every time.

| Choice | Type | Result |
|--------|------|--------|
| Go to your favorite café | Exploitation | A reliable 8 |
| Try a new restaurant | Exploration | Could be a 4, or it could be a 10 |

If you always go to the café, you may never find a restaurant you like even more. If you always try something new, you often get meals worse than your favorite. With ε = 0.1, you would try something new about **1 day out of every 10**.

### Activity

An agent uses ε-greedy with ε = 0.2.

a. What percentage of the time does it explore?
b. What percentage of the time does it exploit?
c. Is "choosing the action with the highest Q-value" exploration or exploitation?

<details>
<summary><b>Answer</b></summary>

a. **20%**
b. **80%** (1 − 0.2)
c. **Exploitation**

</details>

---

# Related Ideas: Deep Learning, Neural Networks, and NLP

## Explanation

Some AI systems learn in a much deeper way:

- **Neural network**: A model built to loosely copy the human brain. It is made of connected **nodes** (also called **neurons**) that pass information along, process it, and produce a prediction.
- **Deep learning**: A type of machine learning that uses neural networks with **many layers**. The layers between the input and the output are called **hidden layers**. More layers let the model learn more complex patterns.

[insert image about a neural network with an input layer, hidden layers, and an output layer]

When reinforcement learning is combined with deep learning, an agent can learn from very complex situations, such as the images on a video game screen.

**Natural Language Processing (NLP)** is the part of AI that helps machines **understand, interpret, and create human language**. It is used on **unstructured data** such as reviews, call transcripts, and social media posts (data that does not fit neatly into rows and columns). NLP has three key parts:

| Part | Meaning | Example |
|------|---------|---------|
| **Computational linguistics** | Uses language science and computing to study human language with computers | Studying how sentences are built |
| **Natural Language Understanding (NLU)** | Machines figure out meaning and context from text and speech | A voice assistant understanding your question |
| **Natural Language Generation (NLG)** | Machines write or speak human-like language | A program writing a short report or speaking an answer |

## Worked Example

**Task:** A customer writes the review: "The battery dies too fast." A company uses NLP to handle it.

| Step | NLP part | What happens |
|------|----------|--------------|
| 1 | NLU | The system works out that the customer is unhappy about **battery life** |
| 2 | NLG | The system writes a reply apologizing and offering help |

## Activity

Decide whether each task is NLU or NLG:

a. A smart speaker figures out that you asked for tomorrow's weather.
b. A program turns sales numbers into a written summary.

<details>
<summary><b>Answer</b></summary>

a. **NLU** (understanding speech)
b. **NLG** (creating text)

</details>

---

## Summary

- **Machine learning** lets computers learn from data using **training data**, **models**, and **algorithms**. The three types are **supervised**, **unsupervised**, and **reinforcement** learning.
- In **reinforcement learning**, an **agent** takes **actions** in an **environment**, moves between **states**, and receives **rewards**.
- A **Markov Decision Process (MDP)** describes the problem with **states, actions, a transition model, and a reward function**.
- A **policy** says which action to take in each state. A **value function** estimates future reward, and the **discount factor** makes later rewards count a little less.
- **Value iteration** and **policy iteration** are two ways to solve an MDP.
- **Q-learning** keeps a **Q-table** of scores for each (state, action) pair and updates it after every experience.
- Agents must balance **exploration** (trying new things) with **exploitation** (using what they know), for example with the **ε-greedy** method.
- **Neural networks** and **deep learning** let models learn complex patterns, and **NLP** helps machines work with human language.