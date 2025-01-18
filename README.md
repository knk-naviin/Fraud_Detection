# Path and Cost Based GNN Model

A PyTorch implementation for the paper below:  
**Path and Cost Based GNN Model for Imbalanced Learning for Mobile Social Network Fraud Detection**

## Running CSGNN

To run the code, you need to have at least Python 3.7 or later versions.  
1.Run `python data_process.py` to generate Sichuan and BUPT dataset in DGL;  
2.-Run `python main.py --config ./config/csgnn_sichuan.yml` to run CSGNN with default settings on Sihcuan dataset.
-Run `python main.py --config ./config/csgnn_bupt.yml` to run CSGNN with default settings on BUPT dataset.   

## Repo Structure
The repository is organized as follows:
- `data_process.py`: convert raw node features and adjacency matrix to DGL dataset;
- `main.py`:  training and testing CSGNN;
- `model.py`: CSGNN model implementations;
- `utils.py`: utility functions.  

# Model Train Results

Epoch 0, Train: Recall: 0.5373 AUC: 0.8650 Loss: 2.4003 | Val: Recall: 0.5343 AUC: 0.8712 Loss: 2.4068 

Epoch 1, Train: Recall: 0.8226 AUC: 0.8725 Loss: 1.9816 | Val: Recall: 0.8505 AUC: 0.8885 Loss: 1.9631 

Epoch 2, Train: Recall: 0.7970 AUC: 0.9092 Loss: 1.8193 | Val: Recall: 0.7950 AUC: 0.9088 Loss: 1.8153 

Epoch 3, Train: Recall: 0.8370 AUC: 0.9247 Loss: 1.6739 | Val: Recall: 0.8444 AUC: 0.9319 Loss: 1.6447 

Epoch 4, Train: Recall: 0.8452 AUC: 0.9167 Loss: 1.5860 | Val: Recall: 0.8629 AUC: 0.9260 Loss: 1.5397 

Epoch 5, Train: Recall: 0.8487 AUC: 0.9161 Loss: 1.5207 | Val: Recall: 0.8651 AUC: 0.9261 Loss: 1.4668 

Epoch 6, Train: Recall: 0.8496 AUC: 0.9230 Loss: 1.4595 | Val: Recall: 0.8642 AUC: 0.9330 Loss: 1.4086 

Epoch 7, Train: Recall: 0.8549 AUC: 0.9319 Loss: 1.4077 | Val: Recall: 0.8576 AUC: 0.9397 Loss: 1.3646 

Epoch 8, Train: Recall: 0.8586 AUC: 0.9366 Loss: 1.3677 | Val: Recall: 0.8561 AUC: 0.9421 Loss: 1.3272 

Epoch 9, Train: Recall: 0.8606 AUC: 0.9386 Loss: 1.3325 | Val: Recall: 0.8606 AUC: 0.9427 Loss: 1.2933 

Epoch 10, Train: Recall: 0.8676 AUC: 0.9407 Loss: 1.3003 | Val: Recall: 0.8530 AUC: 0.9439 Loss: 1.2688 

Epoch 11, Train: Recall: 0.8703 AUC: 0.9446 Loss: 1.2738 | Val: Recall: 0.8551 AUC: 0.9455 Loss: 1.2458 

Epoch 12, Train: Recall: 0.8679 AUC: 0.9469 Loss: 1.2529 | Val: Recall: 0.8514 AUC: 0.9463 Loss: 1.2303 

Epoch 13, Train: Recall: 0.8735 AUC: 0.9480 Loss: 1.2310 | Val: Recall: 0.8550 AUC: 0.9475 Loss: 1.2105 

Epoch 14, Train: Recall: 0.8746 AUC: 0.9475 Loss: 1.2116 | Val: Recall: 0.8590 AUC: 0.9483 Loss: 1.1943 

Test set results: 

Auc= 0.9543 G-mean= 0.8654 Recall= 0.8707