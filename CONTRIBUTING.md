# Contributing to Format Landscape

Thank you for your interest in contributing to the Format Landscape project! This guide will help you understand how to add or update content.

## Content Organization

The repository contains Quarto Markdown (`.qmd`) files that are automatically converted to HTML and published to GitHub Pages.

### Main Pages

- `index.qmd` - Landing page with overview and navigation
- `serialization-formats.qmd` - General overview of common serialization formats
- `*-physics.qmd` - Domain-specific pages for each physics area

### Supporting Files

- `_quarto.yml` - Quarto configuration (navigation, theme, settings)
- `styles.css` - Custom CSS styling
- `.github/workflows/publish.yml` - CI/CD automation
- `README.md` - Repository documentation

## How to Contribute

### Adding a New Format or Resource

1. **Identify the relevant page**: Determine which physics domain or the general serialization page is most appropriate

2. **Edit the `.qmd` file**: Add your content following the existing structure:
   - Use appropriate markdown headers (`##`, `###`)
   - Include links to official websites/repositories
   - Provide brief, clear descriptions
   - Mention key features and use cases

3. **Follow the existing format**:
   ```markdown
   ### Format Name
   - **Website**: [URL](URL)
   - **Description**: Brief description
   - **Use Cases**: Where it's used
   - **Key Features**: Notable characteristics
   ```

4. **Test your changes locally** (optional but recommended):
   ```bash
   quarto preview
   ```

5. **Submit a pull request**: Once you're satisfied with your changes

### Adding a New Physics Domain

If you need to add an entirely new physics domain:

1. **Create a new `.qmd` file**: e.g., `quantum-computing.qmd`

2. **Follow the template** from existing domain pages:
   - Front matter with title
   - Introduction section
   - Organized sections for different types of formats/tools
   - Related Resources section
   - External Links section

3. **Update `_quarto.yml`**: Add your new page to the navigation menu

4. **Update `index.qmd`**: Add a link to your new page

5. **Cross-reference**: Add links from related pages

## Content Guidelines

### Quality Standards

- **Accuracy**: Ensure all information is correct and up-to-date
- **Relevance**: Focus on formats and DSLs actually used in the physics community
- **Clarity**: Write clearly and concisely
- **Links**: Provide working links to official sources when possible
- **Neutral tone**: Maintain an objective, educational tone

### Markdown Style

- Use proper markdown headers (`#`, `##`, `###`)
- Use bullet points for lists
- Use **bold** for emphasis on key terms
- Use `code blocks` for technical terms
- Include links using `[text](URL)` format

### Structure

Each domain page should include:

1. **Introduction**: Brief overview of the domain and its data needs
2. **Main sections**: Organized by format type or use case
3. **Best Practices**: Guidelines for using formats in the domain
4. **Related Resources**: Links to other relevant pages
5. **External Links**: Links to organizations, standards bodies, etc.

## Quarto Markdown Features

You can use Quarto-specific features:

- **Code blocks** with syntax highlighting
- **Callout blocks** for notes/warnings
- **Cross-references** between pages
- **Tables** and **figures**

See [Quarto documentation](https://quarto.org/docs/authoring/markdown-basics.html) for more details.

## Local Development

### Prerequisites

1. Install Quarto: https://quarto.org/docs/get-started/

### Building Locally

```bash
# Preview (with live reload)
quarto preview

# Render to HTML
quarto render
```

The rendered site will be in the `_site` directory.

### Checking Your Changes

Before submitting a PR:

1. Preview your changes locally
2. Check that all links work
3. Verify cross-references to other pages
4. Ensure the navigation works correctly

## Automated Checks

When you submit a pull request:

- GitHub Actions will automatically build the site
- You can preview the build in the Actions tab
- Any build errors will be reported

## Questions?

If you have questions about contributing, please:

1. Check existing issues for similar questions
2. Open a new issue with your question
3. Tag it appropriately (e.g., `question`, `documentation`)

## License and Attribution

By contributing, you agree that your contributions will be part of the open educational resource that is Format Landscape.

Thank you for helping make scientific data formats more accessible!
