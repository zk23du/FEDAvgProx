# FedAvg
<h2> Text</h2>
<h3> Dataset = Agnews </h3>
<h3> Epochs = 100 </h3>
<h3> Clients = 5 </h3>

PGD performed better (FedProx), then DFW with FedProx and DFW FedAvg are almost same!!
<h4> ACCURACY</h4>

| Optimizer | 2 | 4 | 6 | 8 | 16 | --- |
| --- | --- | --- | --- | --- | --- | --- |
| SGD | 70.0573 | 70.7439 | 69.4774 | 69.5041 | 67.1977 | FedAvg |
| BCDFW | 71.8571 | 66.2378 | 64.6114 | 61.2518 | 54.4661 | FedAvg |
| DFW | 81.6589 | 79.4207 | 79.2451 | 75.9036 |  |  FedAvg|
| DFW-Prox | 85.4080 | 83.6526 | 81.5366 | 79.6966 | 70.1451 | FedProx |

<h4> LOSS</h4>

| Optimizer | 2 | 4 | 6 | 8 | 16 | --- |
| --- | --- | --- | --- | --- | --- | --- |
| DFW | 0.5434 | 0.5879 | 0.8076 | 1.4860 |  |  FedAvg|
| DFW-Prox | 0.4109 | 0.4699 | 0.5386 | 0.5904 |  0.8419 | FedProx |
