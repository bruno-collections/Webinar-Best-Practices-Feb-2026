# Bruno Live Workshop — Best Practices Webinar (Feb 18, 2026)

A hands-on workshop repository for the Bruno webinar series. This session was presented on **February 18th, 2026**.

## What's Included

- **Bruno Collection** (`collections/Bruno Live Workshop/`) — A structured collection of API requests organised into modules covering getting started, variables, authentication, tests & assertions, scripts & chaining, and the collection runner.
- **JSON Data File** (`users.json`) — A sample dataset of users used during the workshop exercises.
- **GitHub Actions Workflow** (`.github/workflows/collection-runner-tests.yml`) — A CI workflow that runs the Collection Runner section using the Bruno CLI.

## Workshop Structure

Each section (01 → 06) includes:

- **Instruction docs** — Open a section folder in Bruno and select the **Docs** tab to see step-by-step instructions for completing the exercises.
- **Solution folder** — Every section contains a `Solution` subfolder with fully completed versions of the requests. Use these as a reference if you get stuck.

## Getting Started

1. Clone this repository.
2. Open the collection folder in [Bruno](https://github.com/usebruno/bruno).
3. Follow along with the workshop modules in order (01 → 06).
4. Read the docs on each section folder for exercise instructions, and check the Solution folder if needed.

## 🤖 GitHub Actions

This repo includes a CI workflow that demonstrates running Bruno collections in a CI/CD pipeline with the [Bruno CLI](https://docs.usebruno.com/bru-cli/overview).

**What it does:**
- Installs `@usebruno/cli` and runs the **06-Collection Runner/Solution** folder
- Uses `users.json` as a data file to iterate through 5 users (data-driven testing)
- Generates JSON and HTML test reports, uploaded as build artifacts

**Triggers:** push to `main`, pull requests to `main`, or manual dispatch via the Actions tab.

For more on integrating Bruno with GitHub Actions, see the [Bruno docs](https://docs.usebruno.com/bru-cli/gitHubCLI).
