# Personal Logs

- Forked the repository.
- Cloned the forked repository to the local machine.
- Created a new directory PersonalLogs/YOUR_USERNAME in the repository root.
- Added a new file log.md inside PersonalLogs/YOUR_USERNAME.
- Documented the steps and actions in the log.md file.
- Added and committed the changes using Git:
  - git add PersonalLogs/YOUR_USERNAME
  - git commit -m "Added personal logs directory and initial log.md"
- Pushed the changes to the forked repository:
  - git push origin main
- Created a Pull Request using GitHub CLI:
  - gh pr create --base main --head myusername:main --title "Added personal logs" --body "Added a directory and log file for personal logs documentation."
- Checked the status of the Pull Request:
  - gh pr status
