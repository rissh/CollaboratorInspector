# GitHub Collaborator Finder

This project consists of two shell scripts (`script1.sh` and `script2.sh`) that allow you to list users with read access to a GitHub repository.

## Prerequisites

- Bash (Bourne Again Shell)
- cURL
- jq (a lightweight and flexible command-line JSON processor)

## Getting Started

1. Clone this repository to your local machine.
2. Navigate to the directory containing the scripts.
3. Make sure the scripts have execute permissions.

## Running the Scripts

### Script 1: Dynamic Token from Environment Variables

This script expects the GitHub username and personal access token to be provided as environment variables (`username` and `token`, respectively). You can set these environment variables in your shell or directly before running the script. Here's how to run the script.

    ```bash
        export USERNAME=your_github_username
        export TOKEN=your_personal_access_token
        ./script1.sh <repository_owner> <repository_name>
    ```

Replace your_github_username and your_personal_access_token with your actual GitHub username and personal access token.

### Script 2: Hardcoded Token in Script

This script has the GitHub username and personal access token hardcoded directly into the script. You need to edit the script and replace the placeholders with your actual GitHub username and personal access token before running it. Here's how to run the script.

## Generating GitHub Personal Access Tokens

1. Go to your GitHub account settings.
2. Navigate to "Developer settings" > "Personal access tokens" > "Generate new token."
3. Give your token a descriptive name, select the desired scopes (permissions), and click "Generate token."
4. Copy the generated token and use it as described above.

🚀 Happy coding! 🚀
