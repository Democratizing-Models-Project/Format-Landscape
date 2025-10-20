# Format-Landscape

This repository gathers links and resources on **serialization formats** and **domain-specific languages (DSLs)** used in various physics domains.

## About

Format Landscape is a collection of Markdown documents that provides an organized overview of data formats, file formats, and domain-specific languages used across different areas of physics research:

- **Lattice Physics** - Lattice QCD and related simulations
- **Hadron Physics** - Hadron structure and interactions
- **Nuclear Physics** - Nuclear structure and reactions
- **Astrophysics** - Astronomical observations and cosmology
- **Laser Physics** - Laser-plasma interactions and ultrafast phenomena
- **Particle Physics** - High-energy particle physics experiments
- **Neutrino Physics** - Neutrino experiments and simulations

## Website

The website is automatically built from the Markdown source files using [Quarto](https://quarto.org/) and deployed to GitHub Pages.

Visit the live site at: **https://democratizing-models-project.github.io/Format-Landscape/**

## Local Development

To build and preview the site locally:

1. Install Quarto: https://quarto.org/docs/get-started/
2. Clone this repository
3. Run `quarto preview` in the repository root
4. Open your browser to the provided local URL

To render the site:
```bash
quarto render
```

The output will be in the `_site` directory.

## Contributing

Contributions are welcome! To add information about a format or correct existing content:

1. Fork this repository
2. Edit the relevant `.qmd` files
3. Submit a pull request

## Structure

- `index.qmd` - Main landing page
- `serialization-formats.qmd` - Overview of common serialization formats
- `*-physics.qmd` - Domain-specific pages for each physics area
- `_quarto.yml` - Quarto configuration
- `.github/workflows/publish.yml` - CI/CD workflow for automatic deployment

## License

This is an open educational resource. Content is provided as-is for the benefit of the scientific community.

## Part of

This project is part of the **Democratizing Models Project**, aimed at making scientific software and data more accessible and interoperable.
