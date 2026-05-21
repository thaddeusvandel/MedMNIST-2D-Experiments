# MedMNIST 2D Experiments

Replication of 2D ResNet-50 (224) experiments on all 12 MedMNIST2D datasets as part of a pre-warm-up exercise for AI research in medical imaging.

## Datasets
Trained and evaluated on all 12 MedMNIST2D datasets from the 
[MedMNIST v2 benchmark](https://medmnist.com/), including PathMNIST, 
ChestMNIST, DermaMNIST, and 9 others.

## Model
- Architecture: ResNet-50 (224)
- Each dataset trained 5 times
- Metrics: AUC and Accuracy

## Results
| Dataset        | AUC (mean ± std) | ACC (mean ± std) |
|----------------|------------------|------------------|
| ChestMNIST     |0.7199 ± 0.0051   |0.9296 ± 0.0006   |
| PathMNIST      |0.9789 ± 0.0030   |0.8829 ± 0.0030   |
| TissueMNIST    |0.9312 ± 0.0010   |0.6861 ± 0.0027   |
| BloodMNIST     |0.9971 ± 0.0002   |0.9546 ± 0.0022   |
| BreastMNIST    |0.8634 ± 0.0057   |0.8279 ± 0.0046   |
| DermaMNIST     |0.9097 ± 0.0030   |0.7269 ± 0.0045   |
| PneumoniaMNIST |0.9651 ± 0.0007   |0.8895 ± 0.0079   |
| RetinaMNIST    |0.6963 ± 0.0226   |0.5060 ± 0.0241   |
| OrganAMNIST    |0.9983 ± 0.0001   |0.9454 ± 0.0018   |
| OrganCMNIST    |0.9937 ± 0.0002   |0.9180 ± 0.0023   |
| OrganSMNIST    |0.9776 ± 0.0007   |0.7951 ± 0.0018   |
| OCTSMNIST      |0.9612 ± 0.0016   |0.7742 ± 0.0064   |


## Setup
```bash
pip install -r requirements.txt
python train.py --dataset chestmnist
```

## References
- MedMNIST v2: https://doi.org/10.1038/s41597-022-01721-8
- Original experiments: https://github.com/MedMNIST/experiments