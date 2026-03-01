# Resume Sync

This repo builds `main.tex` into a PDF using GitHub Actions and then publishes the result to `ewu47/resume`.

## How it works

When the workflow runs, it:

1. Checks out this repo.
2. Compiles `main.tex` into `main.pdf`.
3. Clones `https://github.com/ewu47/resume.git`.
4. Copies `main.pdf` to `resume.pdf` in that repo.
5. Commits and pushes if `resume.pdf` changed.

## When it runs

- On every push to `main`
- Manually from the Actions tab (`workflow_dispatch`)
