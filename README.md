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
