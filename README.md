# GitHub Actions CI Workflow Project
🚀 Project Overview

This project demonstrates a basic CI (Continuous Integration) pipeline using GitHub Actions.

Whenever code is pushed to the repository, a workflow automatically runs to:

Install dependencies
Run test cases using pytest

This helps ensure that the code is working properly before merging or deployment.

🛠️ Technologies Used
GitHub Actions
Python
Pytest
Ubuntu (GitHub hosted runner)
📁 Project Structure
.github/
└── workflows/
    └── ci.yml   # CI pipeline configuration
⚙️ CI Workflow Description

The workflow is defined in ci.yml.

🔹 Trigger
on:
  push:
Runs automatically whenever code is pushed to the repository
🔹 Job: test

Runs on:

ubuntu-latest
🔹 Steps
Checkout repository
- uses: actions/checkout@v4
Install dependencies
- name: Install Dependencies
  run: pip install pytest
Run tests
- name: Run Tests
  run: pytest
🔄 CI Flow
Code Push → GitHub Actions Trigger → Install pytest → Run tests → Result (Pass/Fail)
📊 Key Learnings
Basics of CI/CD using GitHub Actions
Automating test execution on push events
Running Python tests in cloud environments
Understanding workflows, jobs, and steps
👨‍💻 Author
Student DevOps / CI-CD Practice Project
Created for learning GitHub Actions automation
