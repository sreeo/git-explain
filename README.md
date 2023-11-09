
# Git Explain Script

This script allows you to get explanations for the differences between two Git commits using the OpenAI API.

## Setup
1.  ### Add script to the PATH
	Place the script in your system's PATH. For Mac machines, you can do this by placing this in the `/usr/local/bin` directory.

2. ### Make the Script Executable:
   Make the `git-explain` script executable by running the following command:

   ```bash
   chmod +x /path/to/git-explain

3. ### Set OPENAI key
	`export OPENAI_API_KEY=your_api_key_here`

## Usage
1. ### With `--to` Flag
	To get an explanation for the differences between two specific commits:
	
	`git explain --from <commit_id1> --to <commit_id2>`
	
	Replace `<commit_A>` and `<commit_B>` with the commit IDs you want to compare.
2. ### Without `--to` Flag
	If you omit the `--to` flag, the script will automatically use the latest commit as the second commit:

	`git explain --to <commit_id1>`

	This will compare commit `<commit_A>` with the latest commit (`HEAD`).
	
