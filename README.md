# 2023--FCNN

# Code from the article, "Characterization and optimization of 5’ untranslated region containing poly-adenine tracts in *Kluyveromyces marxianus* using machine-learning model"

## introduction
You can find the code used in our article about construction of Full Connected Neural Network (FCNN) model using a mini-library from *Kluyveromyces marxianus* and  how to perform prediction of the model and SHapley Additive exPlanation (SHAP) sensitivity analysis of features.

## Note

Firstly, each Python file, along with its corresponding calculated data file(s), should be placed in separate folders. The packages tensorflow v 2.14.0 and shap v 0.41.0 should be installed correctly.
  
To construct the FCNN model, you will need the following files: "construction and train for FCNN.py" and "all.txt". The "all.txt" file contains a table that includes the feature values and relative GFP abundance of all samples, excluding the header (the feature names).
  
For prediction, you will need the following files: "prediction through model.py", "model.h5" (the selected file that contains the saved weights), and "input.txt". The "input.txt" file contains a table of new 5' UTR sequences' feature values, where the feature rank remains consistent with the previous data.
  
For sensitivity analysis, the following files are required: "SHAP_sensitivity_analysis.py", "model.h5", and "input.txt". The "input.txt" file contains a feature value table with a header (where the feature names are listed as the first row) from the training set. The header will facilitate the plot of SHAP sensitivity analysis.

## Code
[FCNN model](https://github.com/CODdown/2023--FCNN/tree/main/Code/construction%20and%20train%20for%20FCNN.py): Python code used to construct and train the FCNN model  
[prediciton](https://github.com/CODdown/2023--FCNN/tree/main/Code/prediction%20through%20model.py): Python code used to predict the GFP abundacne of new sequence with new calculated feature values using selected and saved model  
[sensitivity analysis](https://github.com/CODdown/2023--FCNN/tree/main/Code/SHAP%20sensitivity%20analysis.py): Python code used to perform the SHAP sensitivity analysis of features of train set  
