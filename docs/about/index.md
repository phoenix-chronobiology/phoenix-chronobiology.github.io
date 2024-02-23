# ![Colophon](../images/colophon-2.png){: style="width: 80px; height:80px; vertical-align: middle;" } {{ page.title }}

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

```
mkdocs.yml    # The configuration file.
docs/
    index.md  # The documentation homepage.
    ...       # Other markdown pages, images and other files.
```

### Theme

[Material for MkDocs](https://squidfunk.github.io/mkdocs-material){: target="_blank" }

### Macros

See [macros info](macros-info.md)

## Typography

Material for MkDocs directly integrates with [Google Fonts](https://fonts.google.com/){: target="_blank" }. All fonts are taken from that collection.

Body text and titles are set in ![Cabin](../images/cabin.jpg){: alt="cabin" style="vertical-align: bottom; height: 32px;" }, a nonserif font. 

Code samples are set in ![Ubuntu Mono](../images/ubuntu-mono.jpg){: alt="Ubuntu Mono" style="vertical-align: bottom; height: 32px;" }, a nonserif, monospace font.

For clients who do not have these fonts, the style sheets specify some standard alternatives.

See also "[Privacy](#privacy)".

## Palette

The site provides both light and dark color schemes:

| Mode | Color Scheme |
| ---- | ------------ |
| Light | MkDocs default |
| Dark | MkDocs slate |

The primary color is set to <span style="color:#546d78; background-color: LightCyan; font-weight: bold;">blue-grey</span>.

The accent color is set to <span style="color:#4051b5; background-color: LightCyan; font-weight: bold;">indigo</span>.

## Graphics

![Phoenix Logo](../images/phoenix-mark-w-waves.png){: #phoenix-logo style="display:run-in; height:80px;"}
The Phoenix Project logo symbolizes the investigation of variation
in blood pressure. It is a composite of three images:

- The interior of a human heart and some of the blood vessels,
- An abstract electrocardiogram (ECG) tracing in red, and
- An abstract week-long systolic blood pressure cycle in blue.

The tracings are drawn along two different timescales.

![Colophon](../images/colophon-2.png){: #colophon-icon style="width:80px; height:80px; padding="100px"}
The Colophon icon is a colorized version of "Wax Seal Ampersand" by Rebecca Sicilia from [Noun Project](https://thenounproject.com/browse/icons/term/wax-seal-ampersand/){: target="_blank" title="Wax Seal Ampersand Icons"} (CC BY 3.0).

![favicon](../images/circadian-rhythms.png){: #favicon style="width:88px; height:80px;"}
The favicon is "circadian rhythms" by bsd studio from [Noun Project](https://thenounproject.com/browse/icons/term/circadian-rhythms/){: target="_blank" title="Circadian Rhythms"} (CC BY 3.0).

## Math Notation

Math statements are rendered with the [LaTex](https://en.wikibooks.org/wiki/LaTeX/Mathematics){: target="_blank" } typesetting language, using the [MathJax](https://squidfunk.github.io/mkdocs-material/reference/math/){: target="_blank" } library for displaying mathematical content in browsers. MathJax is incorporated into MkDocs using [arithmatex](https://facelessuser.github.io/pymdown-extensions/extensions/arithmatex/){: target="_blank" }, a Python Markdown extension.

## Privacy

The site uses the [privacy plugin built into Material for MkDocs](https://squidfunk.github.io/mkdocs-material/plugins/privacy/){: target="_blank" }. The plugin:

1. Scans the generated HTML for external assets, such as scripts, style sheets, images, and web fonts.
2. Downloads them.
3. Stores them in the site directory.
4. Replaces all references with links to the downloaded copies for self-hosting.

## License

!!! bug "DRAFT ONLY"
    License selection not finalized. The options being considered are:

    * <a property="dct:title" rel="cc:attributionURL" href="https://cadams4341.github.io/phoenix-biorhythm-platform/">Phoenix Biorhythm Platform</a> by <span property="cc:attributionName">Christopher Adams</span> is marked with <a href="http://creativecommons.org/publicdomain/zero/1.0?ref=chooser-v1" target="_blank" rel="license noopener noreferrer" style="display:inline-block;">CC0 1.0 Universal<img style="height:22px!important;margin-left:3px;vertical-align:text-bottom;" src="https://mirrors.creativecommons.org/presskit/icons/cc.svg?ref=chooser-v1"><img style="height:22px!important;margin-left:3px;vertical-align:text-bottom;" src="https://mirrors.creativecommons.org/presskit/icons/zero.svg?ref=chooser-v1"></a>
    * <a href="http://creativecommons.org/licenses/by/4.0/?ref=chooser-v1" target="_blank" rel="license noopener noreferrer" style="display:inline-block;">CC BY 4.0 (Attribution 4.0 International)<img style="height:22px!important;margin-left:3px;vertical-align:text-bottom;" src="https://mirrors.creativecommons.org/presskit/icons/cc.svg?ref=chooser-v1"><img style="height:22px!important;margin-left:3px;vertical-align:text-bottom;" src="https://mirrors.creativecommons.org/presskit/icons/by.svg?ref=chooser-v1"></a>

    The latter is the current placeholder (see page footer) because it is the more restrictive of the two.

<p xmlns:cc="http://creativecommons.org/ns#" xmlns:dct="http://purl.org/dc/terms/"><a property="dct:title" rel="cc:attributionURL" href="https://cadam4341.github.io/phoenix-biorhythm-platform">Phoenix Biorhythm Platform</a> by <span property="cc:attributionName">Christopher Adams</span> is licensed under <a href="http://creativecommons.org/licenses/by/4.0/?ref=chooser-v1" target="_blank" rel="license noopener noreferrer" style="display:inline-block;">Attribution 4.0 International<img style="height:22px!important;margin-left:3px;vertical-align:text-bottom;" src="https://mirrors.creativecommons.org/presskit/icons/cc.svg?ref=chooser-v1"><img style="height:22px!important;margin-left:3px;vertical-align:text-bottom;" src="https://mirrors.creativecommons.org/presskit/icons/by.svg?ref=chooser-v1"></a></p>
