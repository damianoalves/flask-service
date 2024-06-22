# Contributing to Flask API

First off, thank you for considering contributing to Flask API. It's people like you that make Flask API such a great tool.

## Getting Started

- Fork the repository on GitHub
- Clone your forked repository (not my original one) to your hard drive with `git clone https://github.com/YOURUSERNAME/PROJECTNAME.git`
- `cd PROJECTNAME`
- Install the project's development and runtime requirements: `pipenv install`

## Making Changes

- Create a branch for your changes: `git checkout -b my-feature-branch`
- Make your changes and commit them with a descriptive message. I prefer the use of [Conventional Commits](https://www.conventionalcommits.org/) for commit messages.
- Push your changes to your forked repository.

## Submitting Changes

- Submit a pull request from your forked repository to my original repository.
- I will review your changes and provide feedback. If everything looks good, I will merge your changes.

## Code Style

- I use `flake8`, `black`, `isort`, `mypy`, and `pylama` for code linting and formatting. Run `pipenv run lint` to check your code for any style issues.
- I also use `black` and `isort` for code formatting. Run `pipenv run format` to automatically format your code.

## Testing

- I expect all contributions to maintain the current test coverage. If you add new code, please add tests for it.

## Questions

- If you have any questions, please open an issue and I will get back to you.

Thank you again for your interest in contributing to Flask API!
