# evolution-workshop-2026

Tool tutorials for the Imageomics workshop at **Evolution 2026**: **Designing for Discovery: Shaping Imageomics Tools for Biologists**.

**Date:** Saturday, June 20, 2026, 1:00–5:00 PM | **Location:** Cleveland, OH | [Program listing](https://www.xcdsystem.com/evolution/program/o5SCPR5/index.cfm)

All workshop content lives on a single page: [`docs/index.md`](docs/index.md). Each tool tutorial is a section on that page and generally links out to a Google Colab notebook that contributors add by hand.

## Contributing

Edit [`docs/index.md`](docs/index.md) directly. To add a tutorial notebook, paste your Google Colab URL into the corresponding tool section.

## Development

```bash
uv venv
source .venv/bin/activate
uv pip install -e .

```

Preview the site locally at `localhost:8000`:

```bash
zensical serve
```

## Acknowledgments

The Imageomics Institute is supported by the National Science Foundation under Award No. 2118240. Any opinions, findings and conclusions or recommendations expressed in this material are those of the author(s) and do not necessarily reflect the views of the National Science Foundation.
