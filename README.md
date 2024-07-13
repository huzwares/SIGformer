# jupyter SIGformer 

SIGformer in Jupyter. This repository is a fork of the official Python repository, converted into Jupyter Notebook format to enable interactive coding, documentation, and visualization in an integrated environment.

## Getting Started

To use this code in Google Colab, please follow these steps:

1. **Copy this Notebook in Google Colab**


2. **Enable GPU**: For better performance, it is recommended to run this notebook on a GPU. You can enable the GPU by going to `Runtime` > `Change runtime type` > `Hardware accelerator` and selecting `GPU`. T4 or other GPUs are recommended for optimal performance.


3. **Copy Data Files**: Copy the files from the `/data/` folder to your Google Drive. This will make it easier to access them from within the Colab environment.


4. **Mount Google Drive**: In the second cell of the notebook, mount your Google Drive by running:

```python
from google.colab import drive
drive.mount('/content/drive')
```


5. **Uncomment the First Cell**: The first cell in the notebook contains commands to install the necessary dependencies. To run the code smoothly, you must uncomment this cell and execute it. 
Here is what the first cell looks like:
```python
# !pip install torchsparsegradutils torch_geometric
```


6. **Run the First Cell**: After uncommenting the cell, run it to install the required packages. This may take a few minutes.


7. **Configure Data Paths**: In the third cell (the configuration cell), change the "_train_file", "_valid_file", and "_test_file" variables to point to the paths of the copied data files in your Google Drive. For example:
```python
_train_file = '/content/drive/My Drive/path_to_your_data/train_file.csv'
_valid_file = '/content/drive/My Drive/path_to_your_data/valid_file.csv'
_test_file = '/content/drive/My Drive/path_to_your_data/test_file.csv'
```