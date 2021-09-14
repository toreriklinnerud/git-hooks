## What is this?

Tasks that run prior to every commit and helps support typical workflows in a Rails project. There are hooks for:

- Ruby linter (standard)
- JS linter (prettier)
- Model Annotate (adds schema information to AR models)
- Rspec (executes specs touched in the commit)

Only the files involved in the commit will be affected by the hooks (except for the model annotation).

## How do I use this?

Add the files to the .git/hooks/ directory in your project.

Ensure that they are executable:

`chmod +x .git/hooks/pre-commit*`

You can pick and choose which hooks to use by editing the entries in the `pre-commit`file.
