# Team CSS Workflow

## USE THIS IF:
1. Your git account is already setup.
2. The git repo is already cloned.
3. You're familiar with the detailed process.
> Otherwise use 'help_guides/DETAILED_GUIDE.md'


&nbsp;

## IMPORTANT
Each time you make updates run this sequence into VS terminal (exclude '<', '>'):\
`git checkout main`\
`git branch -D <branch-name>`\
`git pull`\
`git checkout -b <branch-name>`


&nbsp;

## Edit CSS
> Make sure you are in a working branch: `git checkout -b <branch-name>`
- Add any updates into the css file.

&nbsp;

## Save and Commit Changes
**After saving, run this sequence into terminal:**\
`git add academy_stylesheet_2024.css`\
`git commit -m "<summarize-your-changes-here>"`\
`git push origin <branch-name>`

&nbsp;

## Open a Pull Request
Navigate to https://github.com/academyproduct/academy_stylesheet/branches
- Select your \<branch-name>
### There's a green 'compare and pull request' button
- Select 'Compare and Pull Request'
- Submit the Pull Request
### The green button isn't there
- Select 'Contribute'
- Select 'Open Pull Request'
- Submit the Pull Request

The change will need to get reviewed and merged by a team member. Once it has been merged the classes in the stylesheet will apply to OEX.
