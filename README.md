# MS-DIAL Knowledge Base

Comprehensive documentation and knowledge base for MS-DIAL (Mass Spectrometry - Data Independent AnaLysis).

## About

This repository contains a comprehensive knowledge base for MS-DIAL, a free software for processing mass spectrometry data in metabolomics, lipidomics, and proteomics research.

## Documentation

The knowledge base is built using [Quarto](https://quarto.org/) and includes:

- **Getting Started Guide**: Quick introduction to MS-DIAL
- **Installation Instructions**: Step-by-step setup guide  
- **User Guide**: Comprehensive documentation covering:
  - Data processing workflows
  - Metabolomics analysis
  - Lipidomics workflows
- **Tutorials**: Hands-on examples and walkthroughs
- **FAQ**: Frequently asked questions
- **About**: Project information and citations

## Building the Documentation

### Prerequisites

- [Quarto](https://quarto.org/docs/get-started/) (version 1.3 or later)

### Build Instructions

```bash
# Preview the documentation locally
quarto preview .

# Build static HTML
quarto render .

# The generated documentation will be in the docs/ directory
```

### Publishing

To publish to GitHub Pages:

```bash
quarto publish gh-pages
```

## Contributing

Contributions are welcome! Please feel free to:

- Report issues or bugs
- Suggest improvements to documentation
- Submit pull requests with corrections or additions
- Share your workflows and tutorials

## Resources

- **Official MS-DIAL Website**: [http://prime.psc.riken.jp/compms/msdial/main.html](http://prime.psc.riken.jp/compms/msdial/main.html)
- **MS-DIAL GitHub**: [systemsomicslab/MsdialWorkbench](https://github.com/systemsomicslab/MsdialWorkbench)
- **YouTube Channel**: [@msdialproject](https://www.youtube.com/@msdialproject)
- **Twitter**: [@msdial_project](https://twitter.com/msdial_project)

## Citations

If you use MS-DIAL in your research, please cite:

> Tsugawa H., et al. (2015) MS-DIAL: data-independent MS/MS deconvolution for comprehensive metabolome analysis. *Nature Methods*, 12(6), 523-526.

> Tsugawa H., et al. (2020) A lipidome atlas in MS-DIAL 4. *Nature Biotechnology*, 38(10), 1159-1163.

## License

This documentation is released under CC0 1.0 Universal (Public Domain). See [LICENSE](LICENSE) for details.