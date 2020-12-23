# All COVID / NORMAL models notebooks 

This repository gathers the notebooks dealing with the binary classification COVID / NORMAL (SAIN).

-----------

## Models

Notebooks are named according to the model used. The dataset used to train them is the one on the 'dataset' repository however you can use it with any dataset as long as it respects the following architecture :

1. In the root directory at the same level : the notebook and a directory Data/.
2. In the directory Data/ three directory : TRAIN, VALIDATION, TEST.
3. In each directory the file are distributed between two other folder : COVID and NORMAL.

You can use RGB or gray images with any size (all images are processed in 224 by 224).
The following extensions are supported : jpg, jpeg, png.

----------

## Comparisons

The notebook named 'allModelCompare.ipynb' is a notebook that loads and compares on the same code all the models used in this repository.

The notebook presents the results visually but if you want to restart the code you will have to load the models used or save models locally.

The models we used are all stored in the 'memory' repository in the FullModels folder.

If you want to use a different keras model you just have to register it in the following way: 

    model.save("path")
    tensorflow.keras.models.save(model,"path") # Alternative

Be careful not to use the keras format (hpf5). There may be some incompatibilities.


