---
title: About the Site
---

## Host

The Phoenix Projects operate as a study group of the [Twin Cities Section of the Institute of Electrical and Electronics Engineers](http://www.tc-ieee.org){: target="_blank" }.

The Phoenix Biorhythm site is hosted on GitHub Pages.

## Static Site Generator

**MkDocs** is a static site generator that's geared towards building project documentation. Documentation source files are written primarily in [Markdown](https://www.markdownguide.org){: target="_blank" }, and configured with a single YAML configuration file

This site uses Markdown, HTML and cascading style sheets.

For full documentation, visit [mkdocs.org](https://www.mkdocs.org){: target="_blank" }.

### MkDocs Commands

* `mkdocs new [dir-name]` - Create a new project.
* `mkdocs serve` - Start the live-reloading docs server.
* `mkdocs build` - Build the documentation site.
* `mkdocs -h` - Print help message and exit.

### Project layout

``` yaml
mkdocs.yml              # The configuration file
docs/
    index.md            # The documentation homepage
    about/
        index.md
        images/         # subproject-specific images
        ...
    abpm/               # ambulatory blood pressure monitor subproject
        index.md
        images/         # subproject-specific images
       ...
    algorithms/         # biorhythm analysis algorithms subproject
        index.md
        images/         # subproject-specific images
        ...
    biorhythm-platform/ # biorhythm analysis platform subproject
        index.md
        images/         # subproject-specific images
        architecture/
            index.md
            ...
        privacy-security/
            index.md
            ...
        requirements/
            index.md
            ...
    glossary/
        index.md
        images/         # glossary-specific images
    images/             # program-general images, icons and clip art     
    javascripts/
    snippets/
    stylesheets/
    ...                 # Other markdown pages and other files
```

The project is linked to two subprojects:

* blog
* library

### Theme

[Material for MkDocs](https://squidfunk.github.io/mkdocs-material){: target="_blank" }

### Macros

See [macros info](macros-info.md)

## Typography

Material for MkDocs directly integrates with [Google Fonts](https://fonts.google.com/){: target="_blank" }. All fonts are taken from that collection.

Body text and titles are set in ![Cabin](images/cabin.jpg){: alt="cabin" style="vertical-align: bottom; height: 32px;" }, a nonserif font. 

Code samples are set in ![Ubuntu Mono](images/ubuntu-mono.jpg){: alt="Ubuntu Mono" style="vertical-align: bottom; height: 32px;" }, a nonserif, monospace font.

For clients who do not have these fonts, the style sheets specify some standard alternatives.

See also "[Privacy](#privacy)".

## Palette

The site provides both light and dark color schemes:

| Mode | Color Scheme |
| ---- | ------------ |
| Light | MkDocs default |
| Dark | MkDocs slate |

The primary color is set to <span style="color:#546d78; font-weight: bold;">blue-grey (#546d78)</span>.

The accent color is set to <span style="color:#4051b5; font-weight: bold;">indigo (#4051b5)</span>.

## Graphics

| Image&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; | Explanation | Source |
| ------ | ----------- | ------ |
|![Phoenix Mark](../images/phoenix-mark.png){: id="phoenix-mark" style="height:80px;"} | The **Phoenix Projects mark** symbolizes the investigation of variation in blood pressure. | The Phoenix is a composite of the following three images. |
| ![Human Heart Cutaway](../images/coeur_01.png){: style="height:80px;"} | The interior of a human heart and some of the blood vessels | SERVIER MEDICAL ART, a service to medicine provided by Les Laboratoires Servier [www.servier.com](https://www.servier.com/){: target="_blank" }. Image retrieved from [https://smart.servier.com/wp-content/uploads/2016/10/coeur_01.png](https://smart.servier.com/wp-content/uploads/2016/10/coeur_01.png){: target="_blank" }.<br><br>Servier Medical Art is licensed under [CC BY 4.0 <img style="height:18px!important;margin-left:3px;vertical-align:text-bottom;" src="https://mirrors.creativecommons.org/presskit/icons/cc.svg?ref=chooser-v1"><img style="height:18px!important;margin-left:3px;vertical-align:text-bottom;" src="https://mirrors.creativecommons.org/presskit/icons/by.svg?ref=chooser-v1">](https://creativecommons.org/licenses/by/4.0/){: target="_blank" } |
| ![Magnifying Glass](../images/deelight-Magnifying-Glass.svg){: style="height:80px;"} | Magnifying glass | ["Magnifying Glass", by deelight](https://openclipart.org/detail/2202/magnifying-glass){: target="_blank" }, on [OPENCLIPART.org](https://openclipart.org){: target="_blank" }.<br><br>![Public Domain](../images/publicdomain.svg){: style="height: 20px;" } |
| ![Pulse Curve BP-ECG Timing](../images/pulse-curve-bp-ecg-timing-static.svg){: style="height:60px;"} | An abstract: <ol><li>electrocardiogram (ECG) tracing in <span style="color:#33cc33; font-weight: bold;">lime green (#33cc33)</span></li><li>An abstract atrial blood pressure cycle in <span style="color:#cc3333; font-weight: bold;">persian red (#cc3333)</span></li></ol>The tracings are drawn along the same timescale. | Derived from the image titled "Timing of arterial pulse and the ECG", in ["Normal arterial line waveforms", **Deranged Physiology**: A free online resource for Intensive Care Medicine](https://www.derangedphysiology.com/main/sites/default/files/sites/default/files/CICM%20Primary/G%20Cardiovascular%20system/arterial%20line%20timing%20with%20ECG.JPG){: target="_blank" }, by [Alex Yartsev](https://derangedphysiology.com/main/contact){: target="_blank" }.<br><br>The derivation removed all but the waveforms and converted the result to SVG. |
| | The **Phoenix Logo** incorporates the [Phoenix Mark](#phoenix-mark). | ![Phoenix Logo](../images/phoenix-logo.png){: style="width: 214px; height:80px;"}  |
| ![favicon](../images/circadian-rhythms.png){: style="width: 66px; height:60px;"} | | The **favicon** is "circadian rhythms" by bsd studio from [Noun Project](https://thenounproject.com/browse/icons/term/circadian-rhythms/){: target="_blank" title="Circadian Rhythms"} (CC BY 3.0).<br><br>The same image is used for the **apple-touch-icon**. |

The [hero image](../images/hero-heart.svg){: target="_blank" } on the site's home page is the Phoenix Projects mark with CCS animation added to the waveforms.

## Math Notation

Math statements are rendered with the [LaTex](https://en.wikibooks.org/wiki/LaTeX/Mathematics){: target="_blank" } typesetting language, using the [MathJax](https://squidfunk.github.io/mkdocs-material/reference/math/){: target="_blank" } library for displaying mathematical content in browsers. MathJax is incorporated into MkDocs using [arithmatex](https://facelessuser.github.io/pymdown-extensions/extensions/arithmatex/){: target="_blank" }, a Python Markdown extension.

## Library

The ***[Library](https://phoenix-chronobiology.github.io/library/)*** is built as a subsite, separate from this main site. This was done primarily so that the [blog plug-in built into Material for MkDocs](https://squidfunk.github.io/mkdocs-material/plugins/blog/){: target="_blank" } could be applied to both the **Library** and the **[Blog](#blog)** components. The Blog plug-in uses Markdown front-matter to automatically create:

1. *Archive* pages that each list a subset of assets for a time interval.
1. *Category* pages that each list a subset of assets for each category.

Every item in the library has an article, written in Markdown, that serves as library index card. The card includes:

1. The work's title.
1. The work's authors.
1. An abstract or excerpt of the work.
1. The date of distribution or publication.
1. The categories to which the projects assign the work.
1. A citation to the work.
1. URLs to the digital files comprising the asset. The work may consist of some combination of papers, slides, spreadsheets, or graphics.

The URLs usually point into this site's source GitHub repository. However, a card may contain a link into:

* A GitHub repository of an individual project contributor;
* [The GitHub repository for **Hyde**](https://github.com/phoenix-chronobiology/hyde){: target="_blank" }, the archive of The Phoenix Chronobiology Projects' legacy site; or
* The home site of the project sponsor, the University of Minnesota's [Halberg Chronobiology Center, `https://halbergchronobiologycenter.umn.edu)`](https://halbergchronobiologycenter.umn.edu){: target="_blank" }.

This ability to reference sources outside the site is influenced by the activation of the [Privacy plug-in](#privacy).

!!! bug "IDEA"
    1. The project must decide whether to allow the assignment of a given asset to multiple categories rather than to just one.
    1. The project must decide whether to govern the list of categories to avoid redundant or misunderstood keywords.
    1. The ***Library*** could automatically create "Author" pages that list the assets produced by each author. However, just as for the Blog, the project must still resolve details about author privacy.
    1. The summary pages (*Archive*, *Category*) are similar to those implemented by [Academic Pages](https://github.com/academicpages/academicpages.github.io){: target="_blank" }. Because Academic Pages uses [Jekyll](https://jekyllrb.com/){: target="_blank" } rather than [MkDocs](https://www.mkdocs.org){: target="_blank" } for static site generation, the templates for Academic Pages would need converting from [Liquid](https://jekyllrb.com/docs/liquid/){: target="_blank" } to [Jinja](https://palletsprojects.com/projects/jinja/){: target="_blank" }. (The grammar and environments of Liquid and Jinja are similar, so the conversion would be straightforward.)

## Blog

The ***[Blog](https://phoenix-chronobiology.github.io/blog/)***, like the ***[Library](#library)***, is built as a subsite, separate from this main site.

The Blog subsite uses the [blog plug-in built into Material for MkDocs](https://squidfunk.github.io/mkdocs-material/plugins/blog/){: target="_blank" }.

Each blog entry is written in Markdown.

The Blog plug-in uses Markdown front-matter to automatically create:

1. *Archive* pages that each list a subset of assets for a time interval.
1. *Category* pages that each list a subset of assets for each category.

!!! example
    ``` markdown

    ---
    date:
      created: 2024-04-24
      updated: 2024-10-15
    categories:
      - Meeting Minutes
    ---

    # Welcome 2024!

    Lorem ipsum dolor sit amet, consectetur adipiscing elit, sed do eiusmod
    tempor incididunt ut labore et dolore magna aliqua.
    ```

!!! bug "IDEA"
    The plug-in can automatically create "Author" pages that list of the subset of posts by each author. However, the project must still resolve details about attribution to, and mediation of, authors.

For a fully developed blog on which this blog is modeled, see the [Material for MkDocs Blog](https://squidfunk.github.io/mkdocs-material/blog/){: target="_blank" }

## Privacy

The site uses the [privacy plugin built into Material for MkDocs](https://squidfunk.github.io/mkdocs-material/plugins/privacy/){: target="_blank" }. The plugin:

1. Scans the generated HTML for external assets, such as scripts, style sheets, images, and web fonts.
2. Downloads them.
3. Stores them in the site directory.
4. Replaces all references with links to the downloaded copies for self-hosting.

## License

!!! tip
    The following site, provided by GitHub, is recommended for picking an open source license.
    
    [https://choosealicense.com](https://choosealicense.com){: target="_blank" }.

<p xmlns:cc="http://creativecommons.org/ns#" ><a rel="cc:attributionURL" href="https://cadams4341.github.io/phoenix-biorhythm-platform/">This work</a> is licensed under <a href="http://creativecommons.org/licenses/by/4.0/?ref=chooser-v1" target="_blank" rel="license noopener noreferrer" style="display:inline-block;">Creative Commons Attribution 4.0 International Public License<img style="height:22px!important;margin-left:3px;vertical-align:text-bottom;" src="https://mirrors.creativecommons.org/presskit/icons/cc.svg?ref=chooser-v1"><img style="height:22px!important;margin-left:3px;vertical-align:text-bottom;" src="https://mirrors.creativecommons.org/presskit/icons/by.svg?ref=chooser-v1"></a>.</p>

This license is intended for documentation and media only. It is not intended for any software or hardware described on this site.
