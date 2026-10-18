# Group Work Manual

> [!IMPORTANT]
> **The Workflow Has Changed.** We are no longer editing files on the GitHub website. We use **VS Code** and **Git** for all normal work. Read this manual carefully. If you are confused, ask @Infektt.

## 1. Setup
Every team member must do this on their own laptop:
1. **Download Git:** Install from `git-scm.com`.
2. **Download VS Code:** Install from `code.visualstudio.com`.
3. **Install Extension:** Open VS Code, go to Extensions (`Ctrl+Shift+X`), search for **GitHub Pull Requests** (by GitHub), and install it.
4. **Configure Git:** Open the Terminal in VS Code (`Ctrl+~`) and enter:
   `git config --global user.name "Your Name"`
   `git config --global user.email "your-noreply-email@users.noreply.github.com"`
5. **Clone the Repo:** Open VS Code, press `Ctrl+Shift+P`, type `Git: Clone`, paste our repository URL, and click **Open** when finished.

---

## 2. The Daily Workflow
**Never work directly on `main`.**

### Step 1: Pull the Latest Work
Click the branch name in the bottom left corner of VS Code (it probably says `main`). Click **Sync Changes** (or Pull) to download your teammates' latest work.

<img width="326" height="159" alt="4c01ae14-20c1-477f-8482-862d9fcfd761" src="https://github.com/user-attachments/assets/7638fe2a-47b6-452c-bb79-fab8304e8513" />


### Step 2: Create a Branch
Click `main` in the bottom left again, select **Create new branch**, and name it after your task (e.g., `add-spam-example`, `fix-logs`). 
- **Rule:** One task = one branch. Use lowercase and hyphens. Do not mix unrelated tasks.

### Step 3: Work & Commit
Write your Markdown, add images, and save (`Ctrl+S`). 
1. Go to the **Source Control** tab (left sidebar).
2. Click the `+` next to your changed files to stage them.
3. Type a clear commit message (e.g., "Draft spam filter explanation") and click **Commit**.

### Step 4: Push & Create a Pull Request (PR)
Click **Publish Branch** (or Push). Then:
1. Click the **GitHub Pull Requests** icon on the left.
2. Click **Create Pull Request**.
3. Add a title and description, and request a teammate to review it. 

### Step 5: Review & Merge
When a teammate approves your PR, click **Merge Pull Request**. 
**Important:** Once merged, click **Delete Branch**. The work is safely saved in `main`, and this cleans up the temporary workspace.

---

## 3. Understanding Branches & PRs
- **What is a Branch?** A safe, parallel copy of the project. It lets you experiment without breaking `main`.
- **What is a Pull Request (PR)?** A request to merge your branch into `main`. It forces a teammate to check your work before it becomes official.
- **Forgot to make a branch?** Don't panic. Just create the branch now. VS Code will bring your unsaved changes over to it automatically.

---

## 4. Role Responsibilities

### 1. CEO
- Responsible for the overall vision and goals of the project.
- Creates and manages the GitHub repository and folder structure.
- Assigns tasks through `master-task-list.md`, tracking statuses (`To Do` → `In Progress` → `Done`).
- Sets deadlines properly to ensure the final documents are submitted in Lexue on time.
- Acts as the main communicator with the professor.
- Ensures all members consistently update the project log, their personal logs, and AI-use records.
- Writes meeting notes and summaries in `/logs/meetings/`.

### 2. Repository & Submission Lead (CIO)
- Manages team documentation and file organization in GitHub (ensuring `/content/` and `/assets/` are clean).
- Collects all final deliverables (ZIPs, Word/PDFs, Logs) for compilation.
- Handles submissions exclusively on Lexue, ensuring all files are named correctly and sent on time.
- Tracks deadlines, updates, and notifications on Lexue to prevent delays.
- Cross-checks GitHub progress against the `master-task-list.md` to ensure nothing is missing before submission.

### 3. Content Lead / Writer
- Drafts and organizes reports and learning content.
- Writes the shared learning material in `/content/` as Markdown (`.md`) files.
- Proofreads and edits deliverables.
- Hands over finalized written materials in `/content/` to the Visual and Video leads so they can build the deliverables.
- Supports the Quality Lead by refining written materials flagged for improvement.
- Updates `master-task-list.md` changing the tasks status to either  "In progress" or "Waiting for review".

### 4. Visual Design Lead
- Designs visual elements for slides, reports, and the study guide.
- Produces graphics, charts, diagrams, and flowcharts, uploading them to `/assets/`.
- Enhances presentations with animations, layouts, and visual consistency.
- Collaborates with the Content Lead to transform Markdown text from `/content/` into visually appealing slides in `/slides/`.
- Updates `master-task-list.md` changing the tasks status to either  "In progress" or "Waiting for review".

### 5. Video Lead
- Creates and edits video tutorials to explain the module.
- Writes video scripts based on the shared Markdown in `/content/`.
- Records narration and screen demonstrations, ensuring clear pacing and readable visuals.
- Collaborates with the Visual Lead for graphics and the Content Lead for script accuracy.
- Updates `master-task-list.md` changing the tasks status to either  "In progress" or "Waiting for review".

### 6. Quality Lead / Tester (QA)
- Monitors the `master-task-list.md` for tasks marked with "Waiting for review".
  - Marks tasks with "Done" if they pass the review
  - Either opens an issue or notifies the member if the work fails the review
- Reviews the final quality of each member's work (reports, Markdown content, slides, videos).
  - Checks deliverables for mistakes, missing content, or lack of clarity.
  - Ensures outputs meet the requirements set by the CEO and the course rubric.
- Monitors the `/logs/` folder:
  - Checks the credibility of log entries, verifying that attached evidence (screenshots, commits) actually supports the claims made.
  - Checks that commit messages, attached screenshots, and personal logs actually match the real work done. If a commit claims "finished slides" but the file is empty, they flag it by opening an issue or just notifying the team via wechat.
- Acts as the last checkpoint before the CIO submits to Lexue.

> [!IMPORTANT]
> **Everyone must:**
> - Study the module and contribute substantive work.
> - Understand the core content and be able to explain their own contributions.
> - Learn the wider course content outside the team’s module.

---

## 5. How to use GitHub Issues (Web Interface)
GitHub Issues are like **sticky notes** for the project. Instead of managing tasks in a separate chat or spreadsheet, you create an Issue for every task, bug, or idea directly inside the repository.
> I.e., opening an issues is like marking a specific problem in a separate document to tracking its progress separately.

> [!IMPORTANT]
> For this project issues will be predominantly opened by Quality Lead / Tester (QA).
>
> The most of the roles just need to be able to properly commit changes to the issues.

### How to create:

![](assets/manual/manual-github-6.png)

![](assets/manual/manual-github-8.png)

> [!IMPORTANT]
> ![](assets/manual/manual-github-9.png)
> For this project you will receive issues with these labels only, and this is what they mean.

---

**The 5-Step Issue Lifecycle:**
1. **The Quality Lead Opens the Issue**
The Quality Lead reviews a draft (e.g. `/content/hardware.md`) and finds a problem. They go to the Issues tab and click New Issue.
2. **The Member Does the Work**
They get a notification. They go to the actual draft `hardware.md`, draw a diagram, upload it to `/assets/`, link it in the Markdown, and commit the changes.
3. **The Member Replies to the Issue**
They go back to the Issue on GitHub and types a comment at the bottom (e.g. "I've added the diagram and linked it in the file.)
4. **The Quality Lead Verifies (The Important Part)**
The Quality Lead does not just take their word for it. He clicks on the commit link, reads the updated `hardware.md`, and checks that the image actually displays correctly.
5. **The Quality Lead Closes the Issue**
If everything is fixed correctly, the Quality Lead types a final comment ("Looks great. Verified."), and click the "Close issue" button.

Else, the Quality Lead would leave another comment (e.g. "The image is broken, please fix it") and leave the Issue open.

---

## 6. Logging & AI Rules
- **Project Log (`/logs/project-log.md`):** Record team progress, problems, and AI use. Evidence (screenshots) must sit beside the entries.
- **Meeting Summaries (`/logs/meetings/`):** Record decisions, attendees, and action items.
- **Personal Logs:** **DO NOT put these in GitHub.** Write them in Word and submit them via Lexue.
- **AI Use:** All significant AI use must be recorded in the logs (Date, tool, purpose, prompts, verification, outcome). Missing AI records = reduced scores.

---

## 7. Troubleshooting & Emergency Web Editing
- **Git not found:** Restart VS Code after installing Git.
- **Publish Branch is missing:** Make sure you are on a non-main branch and have made a commit.
- **Broken Image:** Check the relative path (e.g., `../assets/image.png`) and ensure the image file was actually committed.
- **Merge Conflict:** Stop. Ask the CEO for help. Do not delete anything or force push.

> [!WARNING]
> **Emergency Only:** If you are away from your laptop and need to fix a 1-letter typo, you can use the GitHub Web interface (click the pencil icon). For any real work, you must use VS Code.
