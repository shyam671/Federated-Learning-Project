# Federated-Learning-Project

## Centralized training

| Model       | Normalization Layer | Number of Parameters | Accuracy / Link   |
| ----------- | ------------------- | -------------------- | ----------------- |
| ResNet-50   |        BN           |         23528522     |       86.91       |
| ResNet-50   |        GN           |         23528522     |       87.48       |

![Drag Racing](Plots/pt-1n.png)

## Fed-Avg training

### IID Distribution 

| Model       | Normalization Layer | Accuracy / Link   |
| ----------- | ------------------- | ----------------- |
| ResNet-50   |        BN           |       81.14       |
| ResNet-50   |        GN           |       78.60       |

![Drag Racing](Plots/pt-2_iid.png)

### Non-IID Distribution 

| Model       | Normalization Layer | Accuracy / Link   |
| ----------- | ------------------- | ----------------- |
| ResNet-50   |        BN           |       34.55       |
| ResNet-50   |        GN           |       51.01       |

## MOON (Model-Contrastive Federated Learning)
Parameters: Number of client:4, Network: Resnet-18, Communication Rounds: 20, Client Epochs: 5, Dataset: CIFAR-10

| Method      | Accuracy @Beta=0.5  |  Accuracy @Beta=0.1  |     Model Link    |
| ----------- | ------------------- | -------------------- | ----------------- |
| FedAvg      |        89.03        |        66.15         |                   |
| FedProx     |        88.66        |        72.47         |                   |
| MOON        |        90.00        |        68.31         |                   |

![Drag Racing](Plots/pt-5.png)
