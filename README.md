# Automated Python Security Scanning with Bandit 🛡️

A simple GitHub Action workflow that performs static security analysis using Bandit on every push to the `main` branch. This is a learning project to understand automated security scanning and CI/CD basics.

## How to Use This Workflow

To use this automated security scan in your own project, follow these steps:

1.  In your repository, create a directory named `.github/workflows/`.
2.  Copy the workflow YAML file (e.g., `bandit-scan.yml`) from this project into that directory.
3.  Commit and push the new file.

That's it. The action will now run automatically on every push to your `main` branch, scanning your code for common security vulnerabilities.

## The Workflow Explained

This repository is configured to run a security scan on every push to the `main` branch. The workflow performs the following steps:

1.  Checks out the repository's code.
2.  Runs the pre-configured Bandit action to scan the entire project for security issues.
3.  The workflow will pass if no vulnerabilities are found at the specified level, or fail if Bandit reports any security issues, preventing insecure code from being merged.

## Technology Used

* [Python](https://www.python.org/)
* [Bandit](https://bandit.readthedocs.io/en/latest/)
* [GitHub Actions](https://github.com/features/actions)