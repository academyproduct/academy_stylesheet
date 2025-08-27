# Team CSS Workflow – Quickstart

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
