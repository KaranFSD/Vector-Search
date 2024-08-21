# Vector Search Demo Notebook

This notebook demonstrates how to perform vector-based text search using the `sentence_transformers` library. It showcases encoding text data into vectors, storing these embeddings, and querying them to find the most semantically similar text entries to a given query.

## Prerequisites

Before running this notebook, ensure you have the following Python libraries installed:

- `sentence_transformers`
- `pandas`

You can install the required libraries using pip:


## Setup

1. Clone this repository or download the notebook and data file (`Text.csv`) to your local machine.
2. Open the notebook in Jupyter Lab or another compatible IDE.
3. Ensure you have a CSV file named `Text.csv` containing a column labeled `text` with the text entries you wish to encode and search through.

## How It Works

1. The notebook starts by loading a pre-trained model from the `sentence_transformers` library.
2. It reads text data from a CSV file into a pandas DataFrame.
3. Text entries are encoded into high-dimensional vectors using the model.
4. These embeddings are saved to a file (`embeddings.pkl`) for future use.
5. A query is defined, and its embedding is computed.
6. Cosine similarity is used to compare the query embedding against all stored embeddings to find the most similar text entry.
7. The result is displayed, showing the most semantically similar text entry to the query.

## Usage

- Modify the `query` variable in the notebook to change the search term.
- Run all cells in sequence to execute the demo.
- Observe the output to see the most similar text entry to your query.

## Saving and Loading Embeddings

The notebook demonstrates saving computed embeddings to a file (`embeddings.pkl`) and reloading them for future queries. This approach is efficient for large datasets, as it avoids re-computing embeddings every time you want to perform a search.

## Contributing

Contributions, improvements, and bug fixes are welcome! Please feel free to submit pull requests or open issues for discussion.