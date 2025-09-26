# Personal Website/Blog

This repository contains the source code for my personal website and blog, built using [Marmite](https://marmite.blog), a static site generator designed for developers.

This website is hosted on GitHub Pages and can be accessed at: [https://machadoah.github.io](https://machadoah.github.io)

## Development

To run the site locally, follow these steps:

1. Clone the repository:

    ```bash
    gh repo clone machadoah/machadoah.github.io
    cd machadoah.github.io
    ```

2. Install the dependencies:

    ```bash
    uv sync --no-dev
    ```

3. Start the development server:

    ```bash
    uv run task serve
    ```

4. Open your browser and navigate to `http://localhost:8000` to view the site.
