# TemplateRepo

Use `rebase and merge` option when merging PR. This will ensure the new commit message for
the merge does not appear.

# If dev and main sync is needed:

Settings -> Actions -> General, set Workflow permissions to Read and write permissions.

Set Personal Access Token as a repository secret. (need to check if this is necessary, might not be.)

```

git checkout main
git pull

git checkout dev
git pull

git rebase origin/main

git push --force-with-lease origin dev

```
