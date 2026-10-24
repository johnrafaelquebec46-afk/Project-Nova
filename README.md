Problem 9: Deleted files on local computer, marked as deleted on git status but is still on the repository
Commands:
git add -u: to tell git to mark the file deletion adn prepare for staging
git commit -m "pushing deleted files": save the staged files
git push origin feature/payment-gateway: pushes the changes which then reflects the deleted files.