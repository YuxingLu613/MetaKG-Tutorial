# Meta2Vec Embedding

Meta2Vec, as part of the MetaKG ecosystem, is an innovative tool designed to allocate embeddings for metabolites within the MetaKG knowledge graph. This tool applies the principles of representation learning to the field of metabolomics, aiming to capture the complex relationships and characteristics of metabolites in a form that can be easily utilized for computational analysis and machine learning applications.

## Getting Started with Meta2Vec

We have developed a seperate Python package for `meta2vec` for instant use without building MetaKG.

`meta2vec` is a Python package for metabolite embedding, which allows for the representation of metabolites in a vector space.

`meta2vec` package contains three modules:

* `distance`: provides functions for calculating the similarity distance between two metabolites using their embeddings.
* `utils`: provides helper functions for working with HMDB (Human Metabolome Database) dataset.
* `visualize`: provides functions for visualizing the embeddings using UMAP.

An example.ipynb is provides.

## Installation

`meta2vec` package can be installed via `pip`:

```bash
pip install meta2vec
```

## Usage

Here is a brief overview of how to use `meta2vec` package:

### Load Pre-trained Embeddings

```python
from meta2vec import from_pretrained

# Load the TransE pre-trained embeddings
hmdb_embeddings = from_pretrained(model_type="TransE", embedding_dir="embedding")
```

The above code loads the pre-trained HMDB embeddings from the `embedding` directory. If the embeddings are not already present in the directory, the function will download them from the GitHub repository.

### Calculate Distance between Two Metabolites

```python
from meta2vec import hmdb_id_cosine_distance, hmdb_id_euclidean_distance

# Calculate the cosine distance between two HMDB IDs
cosine_distance = hmdb_id_cosine_distance(hmdb_embeddings, "HMDB0000001", "HMDB0000002")

# Calculate the Euclidean distance between two HMDB IDs
euclidean_distance = hmdb_id_euclidean_distance(hmdb_embeddings, "HMDB0000001", "HMDB0000002")
```

### Find Most Similar Metabolites

```python
from meta2vec import most_similar

# Find the most similar HMDB IDs to a given HMDB ID
similar_compounds = most_similar(hmdb_embeddings, "HMDB0000001")
```

### Visualize Embeddings

```
from meta2vec import visualize_umap

# Visualize the embeddings using UMAP
visualize_umap(hmdb_embeddings)
```
