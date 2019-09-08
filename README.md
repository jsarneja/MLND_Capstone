# Machine Learning Nanodegree Capstone Project
### Capstone Topic - Spooky story author classification
The [dataset](https://www.kaggle.com/c/spooky-author-identification/data) is procured from a past kaggle competition. The data contains textual excerpts from spooky stories and our task is to map textual excerpts to their respective (three) authors.

### General instructions
1. I executed the project on a Windows machine on an anaconda environment so all instructions below are for Windows
2. The input dataset is already in the `Dataset` folder of the github repo
3. The full jupyter notebook takes ~3.5 hours to run on a high powered machine with GPU. Please ensure a GPU machine before executing this code (specifically for running the neural net model scripts)
4. Two cells take most amount of time to run. These are cells in section 8.2.4 (Hyperparameter tuning) and section 8.3.2 (Stacking of same base learner trained on multiple features). Appropriate notes have been listed on top of each of these cells warning that they take ~1 hour each to run
5. Dummy files named `keep.txt` have been saved in some folders in order to make the folders visible to git. Please ignore these files

### Steps to run this project
1. Clone this github repository using the following command. This will clone the files and the folders
    ```
    git clone https://github.com/jsarneja/MLND_Capstone.git
    ```

2. Download the [Glove word embeddings](http://nlp.stanford.edu/data/glove.42B.300d.zip) (file size ~2GB), place it in the `pre-trained word embeddings` folder and unzip its contents to extract the underlying txt file

3. For running the FastText model in the project, *fasttext* python package is used. For installing this package on windows, Visual Studio C++ build tools should be installed beforehand from [here](https://visualstudio.microsoft.com/thank-you-downloading-visual-studio/?sku=BuildTools&rel=16). During installation, remember to select the C++ tools option (file size ~4GB) in order to complete the necessary requirement for installing the *fasttext* package in python. Skip this part if memory is an issue and you don't need to run the FastText part of the code. In such a case, please remove *fasttext* package from the *requirements.txt* file mentioned below

4. Navigate to the repo and run the following command to download the requirements (works for Windows):
    ```
    pip install -r requirements.txt
    ```
5. To open the jupyter notebook, navigate to the repo and type the following command and in the browser, select the file `Capstone_project.ipynb`:
    ```
    jupyter notebook
    ```
