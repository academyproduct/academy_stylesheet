# Troubleshooting

This will be a catch-all for errors we find and how to navigate them.

&nbsp;
> It's really broken and nothing works

- `git reset --hard origin/main`
- This will hard reset your repo to the remote main branch

&nbsp;
---
&nbsp;

> It's really really broken and the above isn't working

**Delete the parent folder `academy_stylesheet/` and run these commands:**\
`git clone https://github.com/academyproduct/academy_stylesheet.git`\
Open the folder in VS Code (File > Open Folder)\
Open the VS Code Terminal (Top right of app, the icon with the bottom highlighted)\
Everything should be fixed now!

&nbsp;
---
&nbsp;

> When I push I get a message that says "Updates were rejected because a pushed branch tip is behind its remote counterpart."

***Remember the changes you made\
**Run the following in the VS Code terminal:**\
`git checkout main`\
`git pull`\
`git checkout -b <branch-name>`

You should be set to following the most current version of main again. You'll need to redo all of your changes, recommit them and push them again.

&nbsp;
---
&nbsp;

>  ! [rejected]        Josh -> Josh (non-fast-forward)\
error: failed to push some refs to 'https://github.com/academyproduct/academy_stylesheet.git'\
hint: Updates were rejected because the tip of your current branch is behind\
hint: its remote counterpart. Integrate the remote changes (e.g.
hint: 'git pull ...') before pushing again.\
hint: See the 'Note about fast-forwards' in 'git push --help' for details.

Remote branch needs to be deleted

&nbsp;
---
&nbsp;