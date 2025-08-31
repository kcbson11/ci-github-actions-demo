# CI GitHub Actions Demo

This repository demonstrates Continuous Integration (CI) with GitHub Actions.

## Part 1: Continuous Integration
### Task 1: Basic Workflow
- Trigger: push to `main`.
- Steps: checkout + echo message.
- Expected log: `Hello, CI with GitHub Actions!`.

### Task 2: Running Tests
- `main.py` contains `add(a, b)`.
- `test_main.py` runs unit tests with `unittest`.
- The CI workflow sets up Python 3.9 and executes tests.

## Part 2: Advanced Features
### Task 3: Cron Scheduling
- A separate workflow runs daily at **00:00 UTC**.
- Prints `Scheduled build completed successfully!`.

### Task 4: Matrix Builds
- CI runs tests on Python **3.7, 3.8, 3.9, 3.10** in parallel.

## How to Run Tests Locally
```bash
python -m unittest discover -v

## Bonus Task: Self-Hosted Runner
- Installed a GitHub Actions runner on my Windows 10 machine.
- Configured it with the token from GitHub.
- Created a workflow (`selfhosted.yml`) that runs on `self-hosted`.
- Verified the job ran locally on my machine instead of GitHub’s hosted runner.

