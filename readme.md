# Commit-Aid - Automated Commit Message Generator

Commit-Aid is a Node.js-based application that generates commit messages from code diffs using the OpenAI API. It aims to streamline the process of creating meaningful and descriptive commit messages for your Git repositories.

## Installation

To use Commit-Aid, you need to have Node.js installed. You can install Commit-Aid globally by running the following command:

```bash
npm install -g commit-aid
```

Alternatively, you can run Commit-Aid without installing it globally using npx:

```bash
npx commit-aid
```

## Usage

1. **First-Time Setup**: When running Commit-Aid for the first time, it will prompt you to provide an API key for the OpenAI API.

2. **Generating Commit Messages**: To generate a commit message, navigate to a Git repository with uncommitted staged changes and run Commit-Aid with the appropriate commit type:

```bash
commit-aid <type>
```

Replace `<type>` with the type of commit you want to make. The available commit types are: "feat", "fix", "docs", "style", "refactor", "test", or "chore".

3. **Multi-Line Commit Body**: If you wish to include a multiline commit message body, you can use the `--force-body` flag:

```bash
commit-aid <type> --force-body
```

4. **Debug Mode**: To see the intermediate steps and debug information, use the `--debug` flag:

```bash
commit-aid <type> --debug
```

## Example

To generate a commit message for a new feature, you would run:

```bash
commit-aid feat
```

This will create a commit message based on the changes you've staged for the "feat" (feature) type.

## Note

Commit-Aid relies on the OpenAI API for generating commit messages, so you may need to manage your API usage and consider any potential costs associated with API calls.

---

Commit-Aid simplifies the process of generating informative commit messages for your Git repositories, making it easier to maintain a clean and well-documented project history. Happy coding! :rocket: