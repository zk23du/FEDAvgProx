# FedAvg
<h2> Text</h2>
<h3> Dataset = Agnews </h3>
<h3> Epochs = 100 </h3>
<h3> Clients = 5 </h3>

PGD performed better (FedProx), then DFW with FedProx and DFW FedAvg are almost same!!
<h4> ACCURACY</h4>
<h5> Batch Size = 10</h5>

| Optimizer | 2 | 4 | 6 | 8 | 16 | --- |
| --- | --- | --- | --- | --- | --- | --- |
| SGD | 70.0573 | 70.7439 | 69.4774 | 69.5041 | 67.1977 | FedAvg |
| BCDFW | 71.8571 | 66.2378 | 64.6114 | 61.2518 | 54.4661 | FedAvg |
| DFW | 81.6589 | 79.4207 | 79.2451 | 75.9036 | 72.8033 |  FedAvg|
| DFW-Prox | 85.4080 | 83.6526 | 81.5366 | 79.6966 | 70.1451 | FedProx |

<h4> LOSS</h4>

| Optimizer | 2 | 4 | 6 | 8 | 16 | --- |
| --- | --- | --- | --- | --- | --- | --- |
| DFW | 0.5434 | 0.5879 | 0.8076 | 0.8860 | 0.9833 |  FedAvg|
| DFW-Prox | 0.4109 | 0.4699 | 0.5386 | 0.5904 |  0.8419 | FedProx |

<h5> Batch Size = 32</h5>

| Optimizer | 2 | 4 | 6 | 8 | 16 | --- | --- |
| --- | --- | --- | --- | --- | --- | --- | --- |
| DFW | 81.1730 | 76.3926 |  |  |  |  FedAvg| TextCNN |
| DFW-Prox | 89.1978 | 88.7245 | 88.2323 | 88.0035 | 86.7621 | FedProx | TextCNN |
| DFW | 88.6743 | 87.2261 |  |  |  |  FedAvg| fastText |
| DFW-Prox | 88.7151 | 88.4957 | 88.0818 | 87.4487 | 85.1478 | FedProx | fastText |

<h4> LOSS</h4>

| Optimizer | 2 | 4 | 6 | 8 | 16 | --- | --- |
| --- | --- | --- | --- | --- | --- | --- | --- |
| DFW | 0.5162 | 0.6751 |  |  |  | FedAvg | TextCNN |
| DFW-Prox | 0.2003 | 0.2524 | 0.2846 | 0.3038 |  0.3599 | FedProx | TextCNN |
| DFW | 0.3847 | 0.4526 |  |  |  | FedAvg | fastText |
| DFW-Prox | 0.2262 | 0.2767 | 0.3110 | 0.3371 |  0.4126 | FedProx | fastText |

<h2> Image </h2>
<h3> Dataset = Cifar10 </h3>
<h3> Epochs = 300 </h3>
<h3> Clients = 5 </h3>
Optimizers: DFW, PerturbedGradientDescent (specifically for FedProx)

PGD performed better (FedProx), then DFW with FedProx and DFW FedAvg are almost same!!
<h4> ACCURACY</h4>

| Optimizer | 2 | 4 | 6 | 8 | 16 | --- |
| --- | --- | --- | --- | --- | --- | --- |
| SGD | 70.0573 | 70.7439 | 69.4774 | 69.5041 | 67.1977 | FedAvg |
| BCDFW | 71.8571 | 66.2378 | 64.6114 | 61.2518 | 54.4661 | FedAvg |
| DFW | 80.0069 | 78.6828 | 78.1630 | 77.9363 | 77.5963 |  FedAvg|
| DFW | 79.7160 | 78.6162 | 78.6495 | 78.6695 | 78.8961 | FedProx |
| PGD | 82.6956 | 82.1157 | 81.50 | 81 | 79.7560 | FedProx |

<h4> LOSS</h4>

| Optimizer | 2 | 4 | 6 | 8 | 16 | --- |
| --- | --- | --- | --- | --- | --- | --- |
| SGD | 0.4813 | 0.6934 | 0.9535 | 0.6434 | 0.8552 | FedAvg  |
| BCDFW | 0.9481 | 0.9484 | 0.9879 | 1.0980 | 1.2994 | FedAvg  |
| DFW | 0.0945 | 0.1713 | 0.1977 | 0.2131 | 0.2879 | FedAvg  |
| DFW | 0.1136 | 0.1769 | 0.1730 | 0.2230 | 0.2983 | FedProx |
| PGD | 0.0145 | 0.0134 | 0.0799 | 0.0761 | 0.3226 | FedProx |
