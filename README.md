# BIMS Website

Handbook and Technical Docs Repository for the IGRAC Hydrogeological Digitizing Project for Mozambique and Zimbabwe. Here is where we highlight the procedures, principles, and processes related to the work we carried out. Please review this content at [https://kartoza.github.io/IGRAC-ZimAndMozDigitizing](https://kartoza.github.io/IGRAC-ZimAndMozDigitizing) for more information.

## Building the Handbook as a PDF

### Check out the code

```bash
git clone git@github.com:kartoza/IGRAC-ZimAndMozDigitizing.git
```

### Install Dependencies

You need to install these packages:

```bash
pip install mkdocs-with-pdf
pip install mkdocs-material
pip install mdx_gh_links
pip install mkdocs-pdf-export-plugin
```

### Build the documentation

> Note that whenever you add new sections to nav in the mkdocs.yml
> (used for building the web version), you should apply those same
> edits to mkdocs-base.yml if you want those new sections to appear
> in the pdf too.

```bash
cd docs
./build-docs-pdf.sh
xdg-open TheDigitizingHandbook.pdf
```
