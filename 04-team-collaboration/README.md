# Task4: Collaborate as a Team

This is where you put everything together. Your team will create a shared repository and practice the real collaboration workflow: one person owns the repo, the others contribute through branches and pull requests.

**Team size:** 3 to 5 members.

---

## The Assignment

Your team will create a repository with a README that serves as a **mini knowledge base** on a topic. Each team member writes one section and contributes it via a pull request.

### Suggested Topics (pick one, or choose your own)

- "Useful Tools for Students" — each person writes about a different tool (VS Code, Notion, Canva, ChatGPT, etc.)
- "Programming Languages Overview" — each person covers a different language (Python, JavaScript, Java, etc.)
- "Study Tips and Techniques" — each person shares a different study method
- "Introduction to AI Concepts" — each person covers a different concept (machine learning, neural networks, NLP, etc.)
- "Career Paths in Tech" — each person covers a different role (software engineer, data scientist, UX designer, etc.)

---

## Part 1: Repo Owner Sets Up the Project

**One person on the team does this:**

1. On GitHub, click the **+** button (top right) and select **New repository**.
2. Name it based on your chosen topic (e.g., `useful-tools-for-students`).
3. Make it **Public**.
4. Check **"Add a README file"**.
5. Click **Create repository**.
6. Click the pencil icon on the `README.md` to edit it.
7. Replace the content with a structure for your team. Here is an example for a team of 4 working on "Useful Tools for Students":

```markdown
# Useful Tools for Students

A collaborative guide by [list all team member names].

## Table of Contents
- [Introduction](#introduction)
- [VS Code](#vs-code)
- [Notion](#notion)
- [Canva](#canva)

## Introduction
This guide covers tools that every student should know about.
Each section is written by a different team member.

## VS Code
<!-- [Team Member 1 Name] will write this section -->

## Notion
<!-- [Team Member 2 Name] will write this section -->

## Canva
<!-- [Team Member 3 Name] will write this section -->
```

8. Scroll down, type a commit message (e.g., "Set up project structure"), and click **Commit changes**.
9. **Add your teammates as collaborators:**
   - Go to **Settings** > **Collaborators** (in the left sidebar under "Access").
   - Click **Add people**.
   - Search for each teammate's GitHub username and add them.
   - Each teammate will receive an email invitation — they must **accept** it.

---

## Part 2: Each Team Member Contributes a Section

**Every team member (including the repo owner) does this for their assigned section:**

1. **Accept the collaborator invitation** (check your email or GitHub notifications).
2. Go to the team repository on GitHub.
3. Clone it to your computer:

```bash
git clone https://github.com/owner-username/useful-tools-for-students.git
cd useful-tools-for-students
```

> Replace the URL with your actual repository URL. You can find it by clicking the green **Code** button on the repository page.

4. Create a branch named after your section:

```bash
git checkout -b add-vscode-section
```

> Use a descriptive name like `add-vscode-section`, `add-notion-section`, etc.

5. Open `README.md` in a text editor (Notepad, VS Code, or any editor you have).
6. Find your assigned section and replace the comment with your content. Write **at least a paragraph** about your topic. Use Markdown formatting — headings, lists, links, bold text, etc. Example:

```markdown
## VS Code

**Visual Studio Code** (VS Code) is a free code editor made by Microsoft.
It is one of the most popular editors for programming.

### Why Students Should Use It
- It works on Windows, Mac, and Linux.
- It supports almost every programming language.
- It has a built-in terminal so you can run commands without leaving the editor.
- Thousands of extensions add extra features like themes, linters, and AI assistance.

### How to Get Started
1. Download it from [code.visualstudio.com](https://code.visualstudio.com/).
2. Install the recommended extensions for your programming language.
3. Open a folder and start coding.

### Useful Links
- [VS Code Documentation](https://code.visualstudio.com/docs)
- [VS Code Tips and Tricks](https://code.visualstudio.com/docs/getstarted/tips-and-tricks)
```

7. Save the file. Then stage, commit, and push your branch:

```bash
git add README.md
git commit -m "Add VS Code section"
git push origin add-vscode-section
```

8. Go to the repository on GitHub. You will see a yellow banner saying your branch was recently pushed. Click **"Compare & pull request"**.
9. Fill in the pull request:
   - **Title:** Describe what you added (e.g., "Add VS Code section").
   - **Description:** Briefly explain what your section covers.
10. Click **Create pull request**.

---

## Part 3: Repo Owner Reviews and Merges

**The repo owner does this for each pull request:**

1. Go to the **Pull requests** tab in the repository.
2. Click on a pull request to open it.
3. Click the **Files changed** tab to read through the changes.
4. If the content looks good, click **Review changes** > select **Approve** > click **Submit review**.
5. Click **Merge pull request** > **Confirm merge**.
6. Repeat for each teammate's pull request.

If something needs fixing:
- Click **Review changes** > select **Request changes** > write a comment explaining what to fix > click **Submit review**.
- The contributor edits their branch and pushes again — the pull request updates automatically.

---

## Part 4: Keep Everyone in Sync

After each pull request is merged, every team member should pull the latest changes before starting new work:

```bash
git checkout main
git pull
```

This ensures everyone has the most up-to-date version of the file.

---

## Tips for Good Collaboration

- **Use descriptive branch names:** `add-notion-section`, `fix-typo-in-intro`, not `my-changes`.
- **Write clear commit messages:** Describe *what* you changed (e.g., "Add Canva section with setup instructions").
- **Keep pull requests focused:** One section per PR. Don't change other people's sections.
- **Review each other's work:** Read your teammates' pull requests before they get merged. Leave constructive comments.

---

## Bonus Challenge: Handle a Merge Conflict

Merge conflicts happen when two people edit the same line in a file. To practice:

1. Two team members intentionally edit the **same line** (e.g., both edit the Introduction) on different branches.
2. One person submits and merges their PR first.
3. The second person's PR will now show a conflict.
4. On the PR page, click **"Resolve conflicts"**. GitHub will show both versions — choose which text to keep, remove the conflict markers (`<<<<<<<`, `=======`, `>>>>>>>`), and click **Mark as resolved** > **Commit merge**.

This is a normal part of collaboration. Don't be afraid of conflicts — they are just Git asking you to choose which version to keep.

---

## What to Submit

When you are done, your instructor will check the team repository for:

- [ ] The repository has a **clear README** with a table of contents and organized sections.
- [ ] **Each team member** contributed their section through a **separate pull request** (visible in the Pull requests tab > Closed).
- [ ] Each pull request has a **descriptive title** and was **reviewed before merging**.
- [ ] The final README uses **proper Markdown formatting** (headings, lists, links, bold, etc.).

**Submit:** The team repository link (e.g., `https://github.com/owner-username/useful-tools-for-students`). Make sure to include the GitHub usernames of all team members so contributions can be verified.

---

## Reference

- [About collaborative development models - GitHub Docs](https://docs.github.com/en/pull-requests/collaborating-with-pull-requests)
- [Resolving a merge conflict on GitHub](https://docs.github.com/en/pull-requests/collaborating-with-pull-requests/addressing-merge-conflicts/resolving-a-merge-conflict-on-github)
- [GitHub flow - GitHub Docs](https://docs.github.com/en/get-started/using-github/github-flow)
