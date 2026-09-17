# [MAIN educational 2025](https://main-educational.github.io/2025)

This is the archived website of the 2025 edition of the educational workshop of the Montreal Artificial Intelligence and Neuroscience (MAIN) conference.
The website is built with the [jupyter book](https://jupyterbook.org/) project (v2, MyST), and deployed using github pages at <https://main-educational.github.io/2025>.

### Build the book locally
- Clone this repository
- Run `pip install jupyter-book` (recommended in a virtual environment).
- For a fresh build, remove the `_build/` directory
- Run `jupyter book start` to preview, or `jupyter book build --html` for a static build

A static version of the book will be generated in `_build/html/`.

### Publishing the book
A [github action](https://github.com/main-educational/2025/blob/main/.github/workflows/deploy.yml) has been setup to automatically re-build and publish the book every time a change is made to the content of the `main` branch.
Because this site is served from a subpath, the workflow sets `BASE_URL: '/2025'`.
