# Issue tracker: GitHub

Issues and specs live in GitHub Issues for devegoma/github-profile-maker.
Use the gh CLI from this repository.

## Conventions

- Create: gh issue create --title "..." --body-file <file>
- Read: gh issue view <number> --comments
- List: gh issue list --state open --json number,title,body,labels
- Comment: gh issue comment <number> --body-file <file>
- Label: gh issue edit <number> --add-label "..." --remove-label "..."
- Close: gh issue close <number> --comment "..."

For multiline bodies, write the exact text to a temporary file and use
--body-file. Infer the repository from git remote -v.

## Pull requests as a triage surface

PRs as a request surface: no.

## Skill operations

When a skill says "publish to the issue tracker", create a GitHub issue.
When it says "fetch the relevant ticket", read the issue and its comments.
