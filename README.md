Problem 9: Deleted files on local computer, marked as deleted on git status but is still on the repository
Commands:
git add -u: to tell git to mark the file deletion adn prepare for staging
git commit -m "pushing deleted files": save the staged files
git push origin feature/payment-gateway: pushes the changes which then reflects the deleted files.

Problem 10: Accidentally pushed a branch name "testing junks" for all collaborators to see.
Commands: 
git push origin --delete testing-junks: to delete the file on remote/shared repository
git push origin --d testing-junks: to clean my local view

Problem 7: I solved this by using git revert <buggy-commit-hash>. This command safely creates a new commit that undoes the changes made by the mistake, ensuring the repository's history remains intact instead of forcing a deletion.

Problem 8: I recovered the deleted branch by first running git reflog to trace the repository's local history and locate the exact commit hash before the deletion occurred. After finding the hash, I used git branch <deleted-branch-name> <commit-hash> to successfully restore the branch.
