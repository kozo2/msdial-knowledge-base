# MS-DIAL Knowledge Base - Documentation Guide

## Overview

This knowledge base provides comprehensive documentation for MS-DIAL (Mass Spectrometry - Data Independent AnaLysis), covering installation, usage, workflows, and best practices.

## Documentation Structure

### Main Pages

1. **[index.qmd](index.qmd)** - Home page and welcome
   - Overview of MS-DIAL
   - Key features
   - Quick links to resources

2. **[getting-started.qmd](getting-started.qmd)** - Introduction for new users
   - Prerequisites
   - Supported data types
   - Quick start workflow
   - Common questions

3. **[installation.qmd](installation.qmd)** - Installation guide
   - System requirements
   - Windows installation
   - Linux (Docker) installation
   - Database setup
   - Troubleshooting

4. **[tutorials.qmd](tutorials.qmd)** - Hands-on tutorials
   - Basic LC-MS metabolomics
   - GC-MS with retention index
   - LC-MS/MS lipidomics
   - DIA/SWATH processing
   - Ion mobility MS
   - Multi-batch processing

5. **[faq.qmd](faq.qmd)** - Frequently asked questions
   - General questions
   - Installation and setup
   - Data import and formats
   - Data processing
   - Compound identification
   - Troubleshooting

6. **[about.qmd](about.qmd)** - Project information
   - Development team
   - Version history
   - Publications
   - Resources and contact

### User Guide

Located in the `user-guide/` directory:

1. **[overview.qmd](user-guide/overview.qmd)** - User guide overview
   - Guide organization
   - Common workflows
   - Key concepts
   - Parameter settings

2. **[data-processing.qmd](user-guide/data-processing.qmd)** - Complete workflow
   - Project creation
   - Peak detection
   - Identification
   - Alignment
   - Data export
   - Quality control

3. **[metabolomics.qmd](user-guide/metabolomics.qmd)** - Metabolomics workflows
   - LC-MS metabolomics
   - GC-MS metabolomics
   - Database selection
   - Identification strategies
   - Advanced topics

4. **[lipidomics.qmd](user-guide/lipidomics.qmd)** - Lipidomics workflows
   - Lipid class support
   - Project setup
   - Lipid annotation
   - Acyl chain determination
   - Quality control

## Building the Documentation

### Prerequisites

- Quarto 1.4 or later
- Optional: R or Python for code examples

### Local Preview

```bash
quarto preview .
```

This will start a local server (usually at http://localhost:4200) where you can preview the documentation.

### Build Static Site

```bash
quarto render .
```

This generates HTML files in the `docs/` directory.

### Publish to GitHub Pages

The repository includes a GitHub Actions workflow (`.github/workflows/quarto-publish.yml`) that automatically builds and deploys the documentation to GitHub Pages when changes are pushed to the main branch.

## Content Guidelines

### Writing Style

- Use clear, concise language
- Include practical examples
- Add screenshots where helpful
- Use callout boxes for important notes
- Follow existing formatting conventions

### Code Examples

- Use syntax highlighting
- Keep examples simple and focused
- Include expected output
- Explain parameters

### Callout Boxes

Quarto supports several callout types:

```markdown
::: {.callout-note}
## Title
Content
:::
```

Types: `note`, `tip`, `warning`, `caution`, `important`

### Cross-References

Link to other pages:

```markdown
See the [Installation Guide](installation.qmd) for details.
```

Link to sections:

```markdown
See [Peak Detection](user-guide/data-processing.qmd#peak-detection).
```

## File Organization

```
.
├── .github/
│   └── workflows/
│       └── quarto-publish.yml   # GitHub Actions workflow
├── user-guide/                  # User guide section
│   ├── overview.qmd
│   ├── data-processing.qmd
│   ├── metabolomics.qmd
│   └── lipidomics.qmd
├── _quarto.yml                  # Quarto configuration
├── index.qmd                    # Home page
├── getting-started.qmd          # Getting started guide
├── installation.qmd             # Installation guide
├── tutorials.qmd                # Tutorials
├── faq.qmd                      # FAQ
├── about.qmd                    # About page
├── styles.css                   # Custom CSS
├── README.md                    # Repository README
└── CONTRIBUTING.md              # This file
```

## Contributing

### Adding New Content

1. Create a new `.qmd` file in the appropriate directory
2. Add YAML front matter with title
3. Write content using Markdown
4. Add the file to `_quarto.yml` navigation if needed
5. Build and test locally
6. Submit a pull request

### Updating Existing Content

1. Edit the relevant `.qmd` file
2. Test changes locally with `quarto preview`
3. Ensure no broken links
4. Submit a pull request

### Adding Images

1. Create an `images/` directory
2. Save images with descriptive names
3. Reference in Markdown: `![Description](images/filename.png)`
4. Optimize image sizes for web

### Adding Videos

Embed YouTube videos:

```markdown
{{< video https://www.youtube.com/watch?v=VIDEO_ID >}}
```

## Maintenance

### Regular Updates

- Update version numbers when MS-DIAL releases new versions
- Add new features as they are released
- Update troubleshooting section based on user feedback
- Keep citations and links current

### Quality Checks

- Test all links regularly
- Verify code examples work
- Check for outdated information
- Ensure consistent formatting

## Getting Help

- **Quarto Documentation**: https://quarto.org/docs/
- **Markdown Guide**: https://www.markdownguide.org/
- **MS-DIAL Website**: http://prime.psc.riken.jp/compms/msdial/main.html

## License

This documentation is released under CC0 1.0 Universal (Public Domain).
