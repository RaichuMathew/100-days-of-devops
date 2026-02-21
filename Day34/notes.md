# Day34 :- Git Hook

## Task:-
Navigate to the repository cloned under /usr/src/kodekloudrepos that corresponds to /opt/official.git. Merge the feature branch into the master branch locally without pushing yet. In the bare repository /opt/official.git, create a post-update hook inside the hooks directory that automatically creates a release tag named release-YYYY-MM-DD whenever changes are pushed to the master branch, where YYYY-MM-DD represents the current system date. Ensure the hook script is executable. After configuring the hook, push the master branch to trigger the hook and verify that a release tag for the current date is successfully created.

## Purpose:-
This task implements automation using Git hooks to enforce release tagging upon updates to the master branch. Merging the feature branch integrates development changes into the main branch. The post-update hook ensures that every push to master automatically generates a date-based release tag, enabling consistent version tracking and release management. Testing the hook confirms proper automation and validates correct server-sid

