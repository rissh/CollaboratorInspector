# CollaboratorInspector

Collaborator Inspector is a collection of shell scripts designed to help you manage access control for your GitHub repositories. These scripts allow you to easily list users with read access to a GitHub repository, providing a convenient way to monitor and manage collaboration.

## Features

- **List Collaborators**: Quickly fetch and display a list of users with read access to a GitHub repository.
- **Dynamic Token Support**: Use environment variables to provide your GitHub username and personal access token securely.
- **Simple and Lightweight**: Written in Bash and utilizes common command-line tools like cURL and jq for ease of use and portability.

## Prerequisites

- **Bash (Bourne Again Shell)**: The scripts are written in Bash, so you'll need a Bash-compatible shell to run them.
- **cURL**: Used for making HTTP requests to the GitHub API.
- **jq**: A lightweight and flexible command-line JSON processor used for parsing API responses.

## Getting Started

1. **Clone the Repository**: Clone this repository to your local machine using the following command:

   ```bash
   git clone <repository_url>
   ```

2. **Set Permissions**: Ensure that the scripts have execute permissions. You can do this by running the following command:

   ```bash
   chmod +x script1.sh script2.sh
   ```

3. **Set Environment Variables**: Export your GitHub username and personal access token as environment variables:

   ```bash
   export USERNAME=your_github_username
   export TOKEN=your_personal_access_token
   ```

4. **Run the Scripts**: Execute the scripts to list collaborators for your GitHub repository.

## Usage

### Script 1: Dynamic Token from Environment Variables

This script expects the GitHub username and personal access token to be provided as environment variables (USERNAME and TOKEN, respectively). You can set these environment variables in your shell or directly before running the script. Here's how to run the script:

    ```bash
    ./script1.sh <repository_owner> <repository_name>
    ```

### Script 2: Hardcoded Token in Script

This script has the GitHub username and personal access token hardcoded directly into the script. You need to edit the script and replace the placeholders with your actual GitHub username and personal access token before running it. Here's how to run the script:

    ``` bash
    ./script2.sh <repository_owner> <repository_name>
    ```

Replace <repository_owner> with the owner of the GitHub repository and <repository_name> with the name of the repository.

## Generating GitHub Personal Access Tokens

To use these scripts, you'll need to generate a personal access token from your GitHub account. Here's how to do it:

1. Go to your GitHub account settings.
2. Navigate to "Developer settings" > "Personal access tokens" > "Generate new token".
3. Give your token a descriptive name, select the desired scopes (permissions), and click "Generate token".
4. Copy the generated token and use it as described above.

## How to Contribute

Contributions to GitHub Collaborator Finder are welcome! If you'd like to contribute, here's how you can get involved:

1. Fork the repository.
2. Create a new branch (`git checkout -b feature/improvement`).
3. Make your changes.
4. Commit your changes (`git commit -am 'Add new feature'`).
5. Push to the branch (`git push origin feature/improvement`).
6. Create a new pull request.

Please make sure to follow the code of conduct and contribution guidelines in the project.
