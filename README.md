<p align="center">
  <img alt="NSIDC logo" src="https://nsidc.org/themes/custom/nsidc/logo.svg" width="150" />
</p>


# revealjs_presentation_template

revealjs_presentation_template contains templates for NSIDC Revealjs presentations.


## Level of Support

* This repository is not actively supported by NSIDC but we welcome issue submissions and
  pull requests in order to foster community contribution.

See the [LICENSE](LICENSE) for details on permissions and warranties. Please contact
nsidc@nsidc.org for more information.


## Requirements

`quarto`


## Installation

I think the best current approach is to fork this repository for each presentation you create,
then clone the forked repo.

An `environment.yml` is included.  If you are just creating a presentation with no embedded
or executable code, and have `quarto` installed under your user, then you probably do not
need to create an environment.  If you do not have quarto installed, or if you want to create
a separate environment, then you can use `mamba` or `conda` to create an environment.

```
mamba env create -f environment.yml
```

```
conda env create -f environment.yml
```


## Usage

The recommended workflow for creating a presentation is to run `quarto preview`.  This
produces a "live rendering" of the presentation in a web browser tab.  Changes made to
the presentation markdown document are automatically rendered in the "preview".

```
quarto preview name_of_document.qmd
```

When you are ready to publish run

```
quarto render name_of_document.qmd
```

For Revealjs presentations, running `quarto render` generates a `_site` folder that contains
a html file.  The `embed-resources` parameter is set to `True` in the presentation markdown
files so that all resources to create a presentation are in one file that can be shared.

See the [quarto docs](https://quarto.org/docs/tools/text-editors.html) for more information.

A small number of slide layout examples are included in the markdown slides.  For more
information, see the [quarto guide to Revealjs presentations](https://quarto.org/docs/presentations/revealjs/) for information about creating slides.


## Troubleshooting

Read the quarto docs for more information.


## Credit

This content was developed by the National Snow and Ice Data Center with funding from
multiple sources.
