# Quick Start

Welcome to the Quick Start guide for the MetaKG Python package! This guide aims to help you get up and running with MetaKG as quickly as possible. By following the steps outlined below, you'll learn how to install MetaKG, perform basic queries, and start exploring the vast metabolite-centric knowledge graph.



## Step 1: Installation
Before you begin, ensure you have Python 3.6 or later installed on your system. You can install the MetaKG package using pip, Python's package manager. Open your terminal or command prompt and run the following command:

```python
pip install metakg
```

This command will download and install the MetaKG package along with its dependencies.



## Step 2: Importing MetaKG

Once installed, you can import the MetaKG package into your Python script or interactive environment (such as Jupyter Notebook) using the following Python code:

```python
from metakg import MetaKG
```



## Step 3: Basic Usage

The primary function of the MetaKG package is to provide access to the MetaKG knowledge graph. Here's a simple example to fetch and display information about a specific metabolite:

```
# Initialize the MetaKG object
metakg = MetaKG()

# Fetch information about a metabolite by its ID
metabolite_info = metakg.get_metabolite('hmdb_id:HMDB0000001')

# Display the information
print(metabolite_info)
```

This basic example demonstrates how to query the MetaKG for information about a metabolite using its unique identifier.

#### Conclusion

The Quick Start guide aims to provide a brief introduction to the MetaKG Python package, from installation to making your first query. For more detailed information about the package's capabilities, including advanced querying, biological analysis, and data manipulation features, refer to the subsequent documentation sections.

