# Installation

The MetaKG Python package is a useful tool for working with knowledge graphs and metadata. To get started with MetaKG in your Python environment, follow these step-by-step instructions to ensure a smooth installation process using either `pip` or `conda`.

## Prerequisites

Before installing MetaKG, you should have:

- Python 3.6 or newer
- `pip` (Python Package Installer) for `pip` installations
- Anaconda or Miniconda for `conda` installations

You can check your Python version by running:

```bash
python --version
```

If Python is not installed, download it from the official Python website and follow the installation instructions.

## Installation Steps

### Using pip

1. **Open your terminal or command prompt.**
2. **Ensure `pip`, `setuptools`, and `wheel` are up to date** to avoid installation issues:

```bash
python -m pip install --upgrade pip setuptools wheel
```

3. **Install MetaKG** by running:

```bash
pip install metakg
```

### Using conda

1. **Open your terminal or command prompt.**
2. **Install MetaKG** by running:

```bash
conda install -c conda-forge metakg
```

This command will install the MetaKG package from the Conda-Forge repository.

### Verify Installation

To check if MetaKG was installed correctly, import it in a Python shell:

```python
import metakg
print(metakg.__version__)
```

This command should display the installed version of the MetaKG package, indicating a successful installation.

### Troubleshooting

If you encounter any issues during the installation process, consider the following troubleshooting steps:

- Ensure you have a stable internet connection for downloading the package.
- Verify that your Python and pip versions meet the requirements.
- If you receive a permission error, try installing the package with elevated privileges using `sudo pip install metakg` or use a virtual environment.

### Conclusion

Following these steps should allow you to successfully install the MetaKG Python package. This package is your gateway to exploring and analyzing the rich dataset of metabolite-centric information within the MetaKG knowledge graph. For further assistance, refer to the package documentation or contact the support team.

### Next Steps

After successful installation, you're ready to explore MetaKG's features and capabilities. Refer to the following tutorials, examples, and API references.