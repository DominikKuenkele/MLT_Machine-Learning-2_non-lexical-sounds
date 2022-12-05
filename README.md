# Non-lexical sounds
> Part of the Master in Language Technology at the University of Gothenburg
>
> **Course:** Machine Learning 2 (LT2326)
>
> **Assignment:** Final project

## Running the code
All the code is included in the Jupyter Notebook and all the data is stored in the `data` folder. 
To run the model, all cells under `0 - Imports/Constants` need to be run first to get all imports and pretrained embeddings.

To analyze the data, all cells under `1 - Preparing Data` can be run. This is not necessary for training the model, since the training relies solely on the test and train splits, stored by the `split_data` in `.tsv` files. These files are already included in this repository.

The cells under `2 - Loading Data` will load the `.tsv` files into data loaders with a user defined collate function. The cells under `3 - Models` defines the different variation of the models. `4 - Training` will then use the train data loaders and train a specified model. The model can be exchanged for any of the defined (Careful! Model2 requires an additional `alpha` parameter to adapt the weighted addition). The code under `5 - Testing` will test and evaluate the model with the test data loader. With the function `generate_nls_sentence` in the last cell, it is then possible, to 'translate' a sentence into a sentence with NLS.

More details on the code can be found in the report.