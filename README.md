# CI GitHub Actions Demo

This repository demonstrates Continuous Integration using GitHub Actions.

## Workflows

### 1. Simple Workflow (`simple-workflow.yml`)
Runs on every push to `main`. Checks out the code and prints "Hello, CI with GitHub Actions!".

### 2. Python Tests (`python-tests.yml`)
Runs on every push to `main`. Sets up Python, installs dependencies from `requirements.txt`,
and runs unit tests defined in `test_main.py` using a matrix build across Python 3.8, 3.9, 3.10, and 3.11.

### 3. Nightly Build (`nightly-build.yml`)
Scheduled to run daily at midnight UTC (cron `0 0 * * *`), and can also be triggered manually
via `workflow_dispatch`. Prints "Scheduled build completed successfully!".

## Files
- `main.py` — simple add function
- `test_main.py` — unittest tests for `main.py`
- `requirements.txt` — dependencies
