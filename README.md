# The Phoenix Chronobiology Projects

## Overview

**The Phoenix Chronobiology Projects**:

* Work with the [University of Minnesota's Halberg Chronobiology Center](https://halbergchronobiologycenter.umn.edu).
* Operate as a study group of the [Twin Cities Section of the Institute of Electrical and Electronics Engineers](http://www.tc-ieee.org).

The goals of the Projects are to develop:

1. An ambulatory blood pressure monitor that is inexpensive, unobtrusive, easy to use, and collects a week of blood pressure measurements.
1. A platform for biorythm analysis.

The Halberg Chronobiology Center wants the monitor and analytic framework for long term use on massive scale for:

1. Assessing cardiovascular health, detecting pre-disease early, and optimizing treatment schedules, in order to reduce the number of people who die of preventable heart attacks and strokes.
1. Understanding, for health surveillance and maintenance, how blood pressure and heart rate vary in response to stimuli in everyday life.

## This repository

This repository hosts the Projects' home page, which is published on GitHub Pages.

### Static site generator

**MkDocs** is a static site generator that is geared toward building project documentation. Source files are written primarily in [Markdown](https://www.markdownguide.org), and configured with a single YAML configuration file

This site uses Markdown, HTML and cascading style sheets.

For full documentation, visit [mkdocs.org](https://www.mkdocs.org).

### Commands

* `mkdocs new [dir-name]` - Create a new project.
* `mkdocs serve` - Start the live-reloading docs server.
* `mkdocs build` - Build the documentation site.
* `mkdocs -h` - Print help message and exit.

### Project layout

```
mkdocs.yml              # The configuration file
docs/
    index.md            # The documentation homepage
    about/
        index.md
        ...
    abpm/               # ambulatory blood pressure monitor project
        index.md
        ...
    biorhythm-platform/ # biorhythm analysis platform project
        index.md
        architecture/
            index.md
            ...
        requirements/
            index.md
            ...
    images/
    javascripts/
    privacy-security/
        index.md
        ...
    snippets/
    stylesheets/
    glossary.md
    ...                 # Other markdown pages and other files
```

The ***Library*** and ***Blog*** components are built as external subsites.

### Theme

[Material for MkDocs](https://squidfunk.github.io/mkdocs-material)

## Building the site

### Production build

The site is built and deployed via [GitHub Actions](https://docs.github.com/en/actions).

The actions are triggered by a `git push` to the `main` branch.

> The repository currently places minimal constraints on change. Anyone with write access may directly `push` content from a local repository to the GitHub repository. Expect more robust change management as the number of contributors grows. 

### Local build

1. Set up `git`

    See <a href="https://git-scm.com/downloads" target="_blank">https://git-scm.com/downloads</a>

1. Checkout repository

    ```
    git clone https://github.com/phoenix-chronobiology/phoenix-biorhythm-platform.git
    ```

1. Set up Node.js runtime

    > Production environment includes _Node version 20.x_

    See <a href="https://nodejs.org/en" target="_blank">https://nodejs.org/en</a>

1. Set up Node.js dependencies

    ```
    npm clean-install
    ```

1. Set up Python runtime

    > Production environment includes _Python version 3.x_

    See <a href="https://www.python.org/" target="_blank">https://www.python.org/</a>


1. Install Python dependencies

    ```
    pip install mkdocs
    pip install mkdocs-material
    pip install mkdocs-macros-plugin
    pip install mkdocs-git-revision-date-localized-plugin
    pip install mkdocs-link-marker
    pip install mkdocs-exclude
    ```

1. Build documentation

    ```
    mkdocs build --clean
    mkdocs --version
    ```

1. Start MkDocs server

    > See `mkdocs serve -h` for port options
    >
    > Default is port `8000`

    ```
    mkdocs serve
    ```

1. Open local site

    > Use port specified with `mkdocs serve` command

    Open <a href="http://127.0.0.1:8000/" target="_blank">http://127.0.0.1:8000/</a>
