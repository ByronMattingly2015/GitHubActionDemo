# GitHubActionDemo

# Quickstart
https://docs.github.com/en/actions/quickstart

## Creating your first workflow
```
Create a .github/workflows directory in your repository on GitHub if this directory does not already exist.

In the .github/workflows directory, create a file named github-actions-demo.yml. For more information, see "Creating new files."

Copy the following YAML contents into the github-actions-demo.yml file:

YAML
name: GitHub Actions Demo
run-name: ${{ github.actor }} is testing out GitHub Actions 🚀
on: [push]
jobs:
  Explore-GitHub-Actions:
    runs-on: ubuntu-latest
    steps:
      - run: echo "🎉 The job was automatically triggered by a ${{ github.event_name }} event."
      - run: echo "🐧 This job is now running on a ${{ runner.os }} server hosted by GitHub!"
      - run: echo "🔎 The name of your branch is ${{ github.ref }} and your repository is ${{ github.repository }}."
      - name: Check out repository code
        uses: actions/checkout@v3
      - run: echo "💡 The ${{ github.repository }} repository has been cloned to the runner."
      - run: echo "🖥️ The workflow is now ready to test your code on the runner."
      - name: List files in the repository
        run: |
          ls ${{ github.workspace }}
      - run: echo "🍏 This job's status is ${{ job.status }}."

```
Scroll to the bottom of the page and select Create a new branch for this commit and start a pull request. Then, to create a pull request, click Propose new file.

Committing the workflow file to a branch in your repository triggers the push event and runs your workflow.

# Adding a Workflow status badge
https://docs.github.com/en/actions/monitoring-and-troubleshooting-workflows/adding-a-workflow-status-badge

```
![example branch parameter](https://github.com/ByronMattingly2015/GitHubActionDemo/actions/workflows/github-actions-demo.yml/badge.svg?branch=ByronMattingly2015-patch-1)
```
![example branch parameter](https://github.com/ByronMattingly2015/GitHubActionDemo/actions/workflows/github-actions-demo.yml/badge.svg?branch=ByronMattingly2015-patch-1)
