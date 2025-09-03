# Quickstart Guide

This repo holds our shared CSS.  
Each teammate works on **their own branch** named after their first name (e.g., `daniel`, `tony`, `robert`) and opens a Pull Request (PR) into `main`.

Repo: https://github.com/academyproduct/academy_stylesheet.git  
Main CSS file: `academy_stylesheet_2024.css`

## ONE-TIME SETUP

1. **Install tools**

   - [Git](https://git-scm.com/downloads)
   - [VS Code](https://code.visualstudio.com/)
   - GitHub account (USE WORK EMAIL)

2. **Configure Git**
   git config --global user.name "Your Name"  
   git config --global user.email "you@work-email.com"  
   git config --global init.defaultBranch main

3. **Clone the repo**
   git clone https://github.com/academyproduct/academy_stylesheet.git  
   cd academy_stylesheet  
   code .

4. **Create your branch (first name only)**
   git checkout -b yourfirstname  
   git push -u origin yourfirstname

---

## DAILY WORKFLOW

1. **Update your branch**
   git checkout main  
   git pull origin main  
   git checkout yourfirstname  
   git rebase main

2. **Make changes**

   - Edit `academy_stylesheet_2024.css`
   - Save your work

3. **Commit & push**
   git add academy_stylesheet_2024.css
   git commit -m "Describe your change"  
   git push -u origin yourfirstname

4. **Open PR**
   - On GitHub → _Compare & pull request_
   - Title + description → Create PR
   - Reviewer approves → merged to `main`


&nbsp;
\
&nbsp;
\
&nbsp;
\
&nbsp;


# Detailed Guide

This repo holds our shared CSS. Each teammate works on their own branch named after their first name (e.g., daniel, lisa, robert) and opens a Pull Request (PR) to merge changes into main.

Replace the placeholders below:
REPO_URL → the HTTPS URL of this repo (https://github.com/academyproduct/academy_stylesheet.git)
RELATIVE_PATH_TO_CSS → path to the CSS file (e.g., assets/styles.css)

0. What you’ll need (once)

   - A GitHub account
   - Git installed on your computer
   - Visual Studio Code (VS Code)
   - (Recommended) Sign into GitHub inside VS Code

1. Create a GitHub account

   - Go to github.com and create an account (use your work email).
   - Verify your email.

2. Install Git
   Windows - Download and install: https://git-scm.com/download/win - Accept defaults. If asked about a default editor, choose VS Code.
   macOS - Install via Homebrew: - Or download from https://git-scm.com/download/mac.
   Verify
   git --version

3. Configure Git (work identity)
   Set your name and work email so commits are attributed correctly.
   git config --global user.name "Your Name"git config --global user.email "you@your-work-email.com"git config --global init.defaultBranch main
   You can check at any time:
   git config --global --list

4. Install VS Code & sign in to GitHub (recommended) - Download VS Code: https://code.visualstudio.com/ - Open VS Code → bottom-left Accounts icon → Sign in to GitHub - Install these extensions (open VS Code → Extensions):
   GitHub Pull Requests and Issues (official)
   GitLens (optional but helpful)
   Signing in lets VS Code handle GitHub authentication in the background.
   If you’re prompted for a username/password on push, use your GitHub username and a Personal Access Token (PAT). VS Code can also open a browser to authenticate.

5. First-time: clone the repo
   You only do this once per computer.
   Option A: VS Code (easiest) 1. Ctrl/Cmd + Shift + P → type “Git: Clone” → Enter. 2. Paste https://github.com/academyproduct/academy_stylesheet.git and select a local folder. 3. When VS Code asks, click Open the cloned repo.
   Option B: Command line
   cd path/to/your/projects
   git clone REPO_URLcd REPO_FOLDER
   code .

6. Create your branch (first name)
   Naming convention: lowercase first name (no spaces). Example: daniel
   From VS Code terminal (or any terminal opened in the repo folder): # Make sure you're on main and up to dategit checkout main
   git pull origin main # Create and switch to your branchgit checkout -b yourfirstname # Publish your branch to GitHub and set upstreamgit push -u origin yourfirstname
   **YOU WILL ONLY WORK ON YOUR BRANCH. We’ll merge via Pull Requests.**

7. Make your change (CSS)

   1. Open the CSS file: academy_stylesheet_2024.css
   2. Edit as needed.
   3. Save.

8. Commit and push your change
   You can use the VS Code terminal or Source Control panel (left sidebar):
   Terminal (easiest)
   git status
   git add academy_stylesheet_2024.css
   git commit -m "Short message: what you changed"
   git push -u origin your_name
   VS Code UI
   Source Control → + (stage) your changed file(s)
   Enter a commit message (short but clear)
   Click Commit, then Sync/Push

9. Open a Pull Request (PR) 1. In GitHub, you’ll see a prompt: “Compare & pull request” for your branch → click it. 2. Title: short summary (e.g., “Update button styles”) 3. Description: what changed and why (mention any related tickets). 4. Click Create pull request. 5. Request a reviewer if needed.
   **The PR will be reviewed. If approved, it’s merged into main.**

10. Keep your branch up to date (important!)
    **Before you start work each day (and before opening a PR), update your branch:**

# Get the latest from the servergit fetch origin

# Update local maingit checkout main

    git pull origin main

11. Pull the latest changes (ongoing)
    Whenever you just need the latest main locally:
    git checkout main
    git pull origin main
    If you already cloned earlier and just want the newest changes in your working branch:
    git fetch origin
    git checkout yourfirstname
    git rebase main
    git push --force-with-lease

12. Daily workflow (cheat sheet)
    Here are the following daily steps simplified: 1. Update your local .css file daily:
    git pull origin main 2. Edit academy_stylesheet_2024.css as needed → save the file when done 3. Commit and push you changes to Github:
    git add academy_stylesheet_2024.css
    git commit -m "Message explaining the changes you made"
    git push -u origin your_name 4. Open PR in GitHub → request review → address feedback → merge

13. Branch naming & commit message tips
    Branch: first-name only (e.g., daniel) for this project.
    Commit messages:
    Imperative voice: “Change button hover color”
    Small, focused changes are easier to review.

14. Troubleshooting
    I get a 403 or permission error when pushing - Make sure you were added as a collaborator to the repo or have access via your team. - Confirm you cloned with the HTTPS URL and you’re signed into GitHub in VS Code. - Try re-authenticating: In VS Code, sign out/in of GitHub. - Or set a Personal Access Token and use it in place of a password when prompted.
    It keeps asking for a password - Use GitHub authentication via VS Code’s GitHub sign-in. - If using command line, create a Personal Access Token (PAT) and paste it when prompted.
    Wrong email/name on commits
    git config --global user.name "Correct Name"
    git config --global user.email "you@your-work-email.com"
    Stuck in a merge or rebase
    VS Code will show conflicts in the editor. Choose the correct lines, save, then:
    I don’t see my branch on GitHub
    git push -u origin yourfirstname

15. Quick commands reference

# One-time setup after clonegit checkout -b yourfirstname

    git push -u origin yourfirstname

# Daily updategit checkout main

    git pull origin main
    git checkout yourfirstname
    git rebase main

# Make changegit add RELATIVE_PATH_TO_CSS

    git commit -m "Describe your change"
    git push

    git rebase --abort# orgit merge --abort
    git add academy_stylesheet_2024.css

    git rebase --continue   # or: git merge --continue

    git commit --amend --reset-author
    git push --force-with-lease

    git add academy_stylesheet_2024.css
    git commit -m "Describe your change"
    git push

    git checkout main
    git pull origin main
    git checkout yourfirstname
    git rebase main

    brew install git
