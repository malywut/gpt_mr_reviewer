# gpt_mr_reviewer
A Gitlab merge request reviewer that uses GPT3 models from openai. This extremely simple script gets the MR diffs from Gitlab API, and generates a comment in the merge request.
The default model used is text-davinci-003. The prompt used is "Analyze the following code changes and find issues that need fixing if any. The code changes are in git diff notation, lines starting with - are deleted, lines starting with + are added"

## Prerequisites
- A gitlab API token, set in environment variable GITLAB_ACCESS_TOKEN
- An OpenAI api key, set in environment variable OPENAI_API_KEY
- Gitlab informations in environment variables : GITLAB_URL, GITLAB_PROJECT_ID


## Usage
python mr_reviewer.py

## About
Original blog post with how this repo was created: https://medium.com/@mariealice.blete
