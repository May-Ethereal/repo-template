# Project template

Starting point for a new May Ethereal repository. Creating a repository from
this template gives you the files every project in the organization is expected
to have, already wired to the organization-wide security scan.

## What this template gives you

| File | Purpose |
| --- | --- |
| `README.md` | This file — replace it with the project's own README |
| `LICENSE` | GNU GPL v3.0 text, matching the license most of our repositories use |
| `SECURITY.md` | Points at the organization security policy, so reports reach the right inbox |
| `CONTRIBUTING.md` | Points at the organization contribution guidelines |
| `CODEOWNERS` | Requests review from the organization maintainers |
| `.gitignore` | Build output, editor state and local environment files |
| `.github/workflows/ci.yml` | Runs the organization-wide secret and dependency scan on every pull request |

## Before you use it

1. Replace `README.md` with the project's own README. A good one states what
   the project is, how to build it, how to run it, and what it deliberately
   does not do.
2. Confirm the license. `LICENSE` holds GPL-3.0, the license used by most of
   our repositories. If the project needs a different license, replace the file
   and state the new SPDX identifier in the README.
3. Add the build pipeline for the project's language. The template CI only
   runs the organization security scan; the real build belongs in
   `.github/workflows/`.
4. Adjust `CODEOWNERS` to the people who actually review this project.
5. Set the repository description, enable branch protection, and turn on
   Dependabot alerts. The organization policies are in
   [repository standards](https://github.com/May-Ethereal/.github/blob/main/REPOSITORY-STANDARDS.md)
   and [release policy](https://github.com/May-Ethereal/.github/blob/main/RELEASES.md).

## Suggested README skeleton

```markdown
# <name>

One paragraph: what this project is and who it is for.

## Build
Exact commands that build from a clean checkout.

## Run
Exact commands that run it.

## What it does not do
Platforms that are not supported and behaviour that is intentionally absent.

## Dependencies
Table of dependencies and the versions they are pinned to.

## License
SPDX identifier and a link to the license file.
```
