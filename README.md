# GitHooks
Some useful hooks for Git.

## Install hooks in a project

```bash
mkdir .githooks & cd .githooks
cp ~/GitHooks/scripts/* ./
chmod +x ./*
cd ..
git config core.hooksPath .githooks
```

## Activate an hook
Hooks match specific names: `pre-commit` `prepare-commit-msg` `commit-msg` `post-commit` `applypatch-msg` `pre-applypatch` `post-applypatch` `pre-rebase` `post-rewrite` `post-checkout` `post-merge` `pre-push` `pre-auto-gc` `pre-receive` `update` `post-receive`.
It depends of when you want the script to be automatically executed.

For example activating the mirror hook:
```bash
mv .githooks/pre-push_to_mirrors .githooks/pre-push
```
