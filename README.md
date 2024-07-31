# TemplateRepo

Use `rebase and merge` option when merging PR. This will ensure the new commit message for
the merge does not appear.

```

git checkout main
git pull

git checkout dev
git pull

git rebase origin/main

git push --force-with-lease origin dev

```
