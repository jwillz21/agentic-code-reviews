---
description: Review the latest commit(s) on the dev branch of jwillz21/agentic-code-reviews
---

# Review Commit Workflow

When this workflow is triggered, perform the following steps:

1. **Read the code-reviewer skill** by viewing the file at `.agents/skills/code-reviewer/SKILL.md` to load the full review instructions.

2. **Fetch the latest commits** on the `dev` branch of `jwillz21/agentic-code-reviews` using `mcp_github_list_commits` with `sha: dev` and `perPage: 5`.

3. **Identify the newest commit** that has not yet been reviewed (check for existing review comments/issues).

4. **Follow the review process** defined in the code-reviewer skill:
   - Get the commit diff
   - Analyze for security, bugs, performance, and style issues
   - Generate the structured review report

// turbo
5. **Post the review comment** directly on the GitHub commit.

// turbo
6. **Open a summary issue** on the repository with the review findings.

7. **Report back** to the user with a summary of what was reviewed and the verdict.
