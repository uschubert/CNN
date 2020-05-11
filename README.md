# CNN Jet Tagger
In this project we are building jet tagging models, which distinguish between signal and background events.
The main input is the pt-distribution in the detector of the jet, which is represented as a heat map. This heat map is fed to a convolutional
neural network. In addition we are giving the neural network a selection of different expert variables, whose impact on the model prediction we 
want to explore. We judge the impact of these expert variables, through permutation invariance and different LRP algorithms.
## Notebooks
There are three notebooks in this directory. First [CNN_Data_preprocess](CNN_Data_preprocess.ipynb) balances, standardizes and splits the data into test and training set. Furthmore we alos plot the histograms for all features.
Second the [CNN_fit_model](CNN_fit_model.ipynb) fits a CNN model with all expert variables and several models each with one expert variable.
Third [CNN_Analyze](CNN_Analyze.ipynb) analyzes the impact of the different expert variables with permutation invariance and the
LRP algorithm implemented in [innvestigate](https://github.com/albermax/innvestigate).
