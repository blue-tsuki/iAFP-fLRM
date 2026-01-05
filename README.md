# iAFP-fLRM
This repository contains code for "iAFP-fLRM:Accurate Identification of AntifungalPeptides via Hybrid Deep Learning Architecture and Multi-Modal Feature Fusion".
# 1 Description
iAFP-fLRM is a hybrid deep learning framework for AFP prediction.The model integrates BLOSUM62-based evolutionary features, token and positional embeddings, and a Transformer encoder, followed by an LSTM-ResMLP classification module to capture both global contextual and local sequential dependencies.
# 2 Running

*   **`dataset/`**: Contains the required datasets.  
*   **`model/`**: Stores pre-trained models ready for inference.  
*   **`util/`**: Utility modules.  
    - `data_loader.py`: Handles data loading and preprocessing.  

In addition, the main scripts and files are as follows:

*   **`model.py`**: Defines the iAFP-fLRM model architecture.  
*   **`train.py`**: Defines the Model Training Process.
*   **`main`**: Can be run directly to train the model.

# 3 Predict
To predict AFP sequences, prepare the target sequences and set the input file path in `predict.py`. The script will then output the Predicted_Label,True_Label,Confidence and Correct.
