# Day24 - Create Git Branche

Project Repository: /usr/src/kodekloudrepos/official

## Task: Create a new branch for feature development without modifying existing code.

## 📋 Requirement Summary
The development team needs a dedicated environment for new features. We will branch off the current master state to ensure the production code remains stable while they work on xfusioncorp_official.

## 💻 Implementation Steps
### 1. Navigate to the Repository
Connect to the Storage Server and move into the project directory:

cd /usr/src/kodekloudrepos/official
### 2. Verify Current State
Before branching, ensure you are starting from the master branch:

git checkout master
### 3. Create the New Branch
Run the following command to create the xfusioncorp_official branch.

Note: The -b flag creates the branch and switches (checkouts) to it immediately.

git checkout -b xfusioncorp_official
### 4. Confirm the Change
List all branches to verify that the new branch exists and is currently active (indicated by an asterisk *):

git branch
## Expected Output:

  master
* xfusioncorp_official

## Notes
Syncing: If this is a shared repository, you may eventually need to push this branch to a remote, but for this local server task, the branch creation is now complete.
