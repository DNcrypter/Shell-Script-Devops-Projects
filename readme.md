
# Github-API Script : list the users of given repository 

## Introduction
This is a Bash script designed to fetch a list of GitHub users with read access to a specific repository. The script uses the GitHub API to query for users who have "read" permissions in the specified repository. It is particularly useful for repository administrators or owners who need to track and manage access levels of collaborators in a project.

## Prerequisites
* GitHub username and personal access token.
* jq command-line tool for parsing JSON responses from the GitHub API (can be installed with ***sudo apt-get install jq*** on Linux-based systems).

## Setup
1. Clone the repository or download the script file.
bash.
```
git clone https://github.com/your-repository.git
```

2. Install the required tools:
Make sure you have the jq tool installed to process the JSON data returned by the GitHub API.
```
sudo apt-get install jq
```

3. Usage:
To run the script, you need to provide two arguments:

Repository Owner: The GitHub username of the repository owner.
Repository Name: The name of the repository you want to check.

```
./fetch_read_access_users.sh <repository_owner> <repository_name>
```

4. Authentication:
Before running the script, ensure that you set your GitHub username and personal access token in the script. Replace the placeholders:
```
USERNAME=$username
TOKEN=$token
```
You can create a personal access token on GitHub by following the steps outlined in [GitHub's documentation](https://docs.github.com/en/github/authenticating-to-github/creating-a-personal-access-token).

## Conclusion 
This script provides a quick and efficient way to list users with read access to a GitHub repository. It simplifies access management and helps repository owners easily track permissions.

