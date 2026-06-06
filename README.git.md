# Git Ignore

## Pattern Matching

| target | how to
|:-------|:-------
| root   | begin with `/`
| folder | end with `/`
| file   | combine file path with folder negation

## Wildcards

| target   | how to
|:---------|:-------
| `?`      | match any ONE character except slash
| `*`      | matches any set of characters except slash
| `**/`    | match any depth of folders
| `/**`    | match everything inside
| `a/**/b` | match anything between a and b

## Rules

Instead of guessing and reactively exluding folders & files from .git we begin by excluding EVERYTHING, and only including items which have been explicitly, intentionally added to this .gitignore file.

This makes it much less likely for files & folders to be accidentally committed to the repository history.
