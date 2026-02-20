# Day30 :- Git Reset

## Task:-
Navigate to the Git repository located at /usr/src/kodekloudrepos/demo. Identify the commit with the message "add data.txt file" and reset the branch to that commit so that only two commits remain in the history: "initial commit" and "add data.txt file". Perform a hard reset to move both HEAD and the branch pointer to the specified commit, removing subsequent commits from the history. Finally, force push the updated branch to the remote repository to reflect the rewritten commit history.

## Purpose:-
This task rewrites the repository history to remove unwanted test commits and restore the repository to a clean state. Using a hard reset ensures both the commit history and working directory are aligned with the specified commit. A force push is required because the branch history has been altered, and the remote repository must be updated to match the corrected commit structure.

