# Academy Stylesheet Repo

**Important note:**
Always start new work by pulling the latest main branch, then create a new branch from there.

**Branch Name Examples:**
- john-button-fix
- jane-new-accordion
---

\
These are steps to modify academy_stylesheet_2024.css

## 1. Build & test your CSS changes

1. Start in OEX Authoring, keeping all new CSS inside a `<style>` block.

2. Use **View Live** to make sure new styles work as expected.

3. Test the styles/components in our prod **ZZ - Live Testing** course.

4. Open the course in an incognito window with a student account to confirm:

    - Functionality works

    - Layout looks good on both desktop and mobile

    - For mobile, use BrowserStack (or your own device).



## 2. Create a Git branch

We use branches so multiple people can work at once without overwriting each other.

Run these commands in your terminal, or VS Code:

1. Make sure you are on main and up to date
    - `git checkout main`
    - `git pull origin main`

2. Create your own branch (replace "yourname-feature" with something descriptive)
    - `git checkout -b yourname-feature`

## 3. Make your stylesheet edits

1. Open academy_stylesheet_2024.css in VS Code.

2. Add your changes.

3. Save the file.

## 4. Commit your changes in terminal of the correct folder
1. (if needed) `cd ~/Desktop/folder_path..`
2. `git add academy_stylesheet_2024.css`
3. `git commit -m "changes description here"`

## 5. Push your branch to GitHub

`git push origin yourname-feature`

## 6. Open a Pull Request (PR)

1. Go to our repo on GitHub.

2. Select “Compare & pull request”

3. Add a short description of your changes.

4. Request a reviewer.

5. Submit the PR.

## 7. Teammate reviews and merges
This will merge the branch over to main, the main branch will then automatically push to s3 and reflect the updates.

## 8. Verify
Once merge and deployment are successful a message will be sent out confirming.\

To see the changes you will need to:
- remove the original `<style>` block containing your code.
- clear your browser cache.
- refresh the page.

