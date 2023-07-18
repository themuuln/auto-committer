<div align="center">
  <h1>Auto-Committer 🤖</h1>
  <!-- <img src="https://raw.githubusercontent.com/themuuln/auto-committer/main/assets/logo.png" alt="Auto-Committer Logo" width="200"> -->
  <p>Automate your GitHub commits and keep your repository history active!</p>
  <p>
    <a href="https://github.com/themuuln/auto-committer/actions">View Actions</a> ·
    <a href="https://github.com/themuuln/auto-committer/issues">Report Bug</a> ·
    <a href="https://github.com/themuuln/auto-committer/pulls">Contribute</a>
  </p>
  <p>
    <a href="https://github.com/themuuln/auto-committer/actions/workflows/auto_commit.yml">
      <img src="https://github.com/themuuln/auto-committer/actions/workflows/auto_commit.yml/badge.svg" alt="Auto Commit">
    </a>
  </p>
</div>

## How it Works

Auto-Committer is a GitHub Action that automates daily commits to your repository. Every three hours, it creates a series of empty commits to keep your commit history fresh and active. While the commits are empty and playful in nature, they serve as a motivational reminder to stay committed to your coding endeavors.

## Getting Started

To experience the magic of daily automation, follow these simple steps:

1. **Fork this Repository**: Start by forking this repository to make it your own.

2. **Configure the Schedule**: Customize the scheduled time for daily commits in the `.github/workflows/auto_commit.yml` file. By default, the workflow runs every three hours (e.g., 0:00 AM, 3:00 AM, 6:00 AM, ...).

```
* */3 * * *
| | | | |
| | | | +----- Day of the week (0 - 7) (Sunday is both 0 and 7)
| | | +------- Month (1 - 12)
| | +--------- Day of the month (1 - 31)
| +----------- Hour (0 - 23)
+------------- Minute (0 - 59)
```

3. **Make it Yours**: Customize the automation to your liking. You can update files, run tests, or add other tasks to the workflow to match your personal project needs.

## Improvement Ideas

To enhance the Auto-Committer workflow, we made several improvements:

- **Use GitHub Secrets**: Git credentials (username and email) and the Personal Access Token (PAT) are securely stored as GitHub Secrets for a safer workflow.

- **Limit Commits**: Automated commits are now limited to specific intervals (06:00 AM - 06:00 PM UTC) to avoid excessive commits.

- **Commit Timestamp**: Each automated commit includes the timestamp of when it was made, making it easier to track commit times.

- **Commit Interval Tracking**: The workflow now tracks the last commit time and enforces a commit limit interval to prevent overcommitting.

## Contributing

Contributions to this project are welcome! If you have ideas to improve the automation or enhance the experience, feel free to open an issue or submit a pull request.

## License

This project is licensed under the [MIT License](LICENSE), allowing you to use and modify the code freely.

---

<div align="center">
  <p>If you find this project helpful, please consider giving it a ⭐️</p>
  <p>Follow me on GitHub <a href="https://github.com/themuuln">here</a></p>
</div>