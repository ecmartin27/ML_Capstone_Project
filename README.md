This repository contains a jupiter notebook, which builds a convolutional neural network (CNN) to analyze microscopy images from https://idr.openmicroscopy.org/webclient/?show=screen-1251. These images contain tumor cells treated with a variety of chemotherapy compounds. The model is trained on both control and treated cells to analyze the toxicity of each compound.

After the CNN model is trained, its learned toxicity features are connected to a label corresponding to the compound that each group of cells was treated with. RDkit was used to find structural features of each compound, such as carbon percentage or chirality. This is then fed into a feed-forward neural network to correlate the toxicity features with features of each compound. After training this model, it is used to predict the relative toxicity of a chemotherapy compound, given its structural features.
