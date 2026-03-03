# Agent Instructions

## README Maintenance

After making any significant change to the project, check whether `README.md` still accurately reflects the current state. Update it if:

- Files or directories listed in the **Repository Contents** table have been added, removed, or renamed.
- Build commands, targets, or the build pipeline have changed (e.g. new Makefile targets, changed output paths).
- The draft revision number has been bumped — do NOT hardcode the revision in prose; refer to `make version` instead.
- Key protocol concepts described in the README no longer match the draft source (`draft-zzn-dvs.md`).
- Prerequisites or setup instructions have changed.

## Versioning

- The draft revision is tracked by `REVISION` in the `Makefile`. Never hardcode the revision number in documentation — use `make version` or generic placeholders like `XX`.
- Use `make tag` to create annotated git tags and `make bump` to increment the revision.

## Git

- Always ask for user approval before running `git commit`, `git add`, `git push`, or any database migration command.
- Use `--no-pager` with git commands that may enter interactive mode.
