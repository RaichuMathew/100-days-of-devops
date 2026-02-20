## 1. Preparation & Local Check (SSH)
Before touching the UI, Max needs to verify the work locally on the Storage Server.

Host: Storage Server

User: max | Pass: Max_pass123

Action: * cd ~/repo-name (Navigate to the cloned repo).

git log --oneline(Confirm the story/fox-and-grapes branch exists and see Sarah’s previous history).

## 2. Create the Pull Request (Max)
Login to the Gitea UI to start the formal merge process.

Login: max / Max_pass123

Source Branch: story/fox-and-grapes

Destination Branch: master

PR Title: Added fox-and-grapes story

Assign Reviewer: On the right-hand sidebar of the PR, click Reviewers and select tom.

## 3. Review and Merge (Tom)
Now, switch roles to simulate the "Approver" workflow.

Logout as Max and Login as tom / Tom_pass123.

Navigate to the Pull Requests tab in the repository.

Action: * Open the PR "Added fox-and-grapes story".

Click Files Changed to review the code.

Click Approve (or the "Checkmark" icon).

Click Merge Pull Request to finalize the change into master.

Key Takeaways for Max
The Repository: Remains the same (/home/max/repo), but the Master Branch is now protected.

The Pull Request: Acts as a "waiting room" where code stays until a second pair of eyes (Tom) confirms it's ready.

The "Source": Always the feature branch (story/fox-and-grapes).

The "Destination": Always the stable branch (master).
