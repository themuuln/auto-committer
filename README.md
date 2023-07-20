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

Auto-Committer is a GitHub Action that automates daily commits to your repository. Every 12 hours, it creates a series of empty commits to keep your commit history fresh and active. While the commits are empty and playful in nature, they serve as a motivational reminder to stay committed to your coding endeavors.

## Getting Started

To experience the magic of daily automation, follow these simple steps:

1. **Fork the Repository**:
   Go to the original "Auto-Committer" repository on GitHub (https://github.com/themuuln/auto-committer). Click on the "Fork" button in the top right corner of the repository page. This will create a copy of the repository in your GitHub account.

2. **Configure the Schedule**:
   In your forked repository, navigate to the `.github/workflows/auto_commit.yml` file. This is the workflow file responsible for automating the commits. By default, the workflow runs every three hours. You can customize the schedule by modifying the cron syntax in the file.

   The cron syntax looks like this:
   ```
   * */3 * * *
   | | | | |
   | | | | +----- Day of the week (0 - 7) (Sunday is both 0 and 7)
   | | | +------- Month (1 - 12)
   | | +--------- Day of the month (1 - 31)
   | +----------- Hour (0 - 23)
   +------------- Minute (0 - 59)
   ```
   Update the cron schedule to your preferred timing, if necessary.

3. **Make it Yours**:
   Customize the automation to fit your requirements. The current workflow creates empty commits every three hours. You can modify the workflow to include additional tasks or actions relevant to your personal project needs.

4. **Use GitHub Secrets (Optional)**:
   To enhance security, consider using GitHub Secrets to store sensitive information like Git credentials (username and email) and the Personal Access Token (PAT). Using GitHub Secrets ensures that this sensitive data is not exposed in your workflow files.

5. **Limit Commits (Optional)**:
   The original repository implemented a commit limit to specific intervals (06:00 AM - 06:00 PM UTC) to avoid excessive commits. You can consider keeping this limitation to prevent too many automated commits.

6. **Commit Timestamp (Optional)**:
   To track commit times easily, the original repository added a timestamp to each automated commit. You may choose to keep this feature as it enhances the clarity of your commit history.

7. **Commit Interval Tracking (Optional)**:
   If you want to prevent overcommitting, you can implement a mechanism that tracks the last commit time and enforces a commit limit interval.

8. **Contributing (Optional)**:
   If you have ideas to improve the Auto-Committer workflow or enhance the experience, you can contribute to the project. You can open an issue to discuss your ideas or directly submit a pull request with your improvements.

9. **License**:
   The "Auto-Committer" project is licensed under the MIT License, which allows you to use and modify the code freely. Ensure you comply with the license terms.

10. **Give it a Star**:
    If you find the "Auto-Committer" project helpful, consider giving it a ⭐️ on GitHub.


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
