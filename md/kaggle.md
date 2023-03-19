# Data set - HW2

## Original Data set results

### Different models

| Models Name      | Sub Model | Test Order | Result on Kaggle |
| ---------------- | --------- | ---------- | ---------------- |
| Baseline         |           |            | 0.58             |
| efficientnet v1  | B6        | test 1     | 0.599            |
| efficientnet v1  | B6        | test 2     | 0.612            |
| efficientnet v2  | M         | test 1     | 0.616            |
| efficientnet v2  | L         | test 1     | 0.653            |
| efficientnet v2  | L         | test 2     | 0.703            |

## Final Configuration

### Variables

- Model: efficientnetv2 large
- Optimizer: Adam
- Learning rate: 3e-4
- Weight decay: 1e-5
- Scheduler: ReduceLROnPlateau
- Metric: Validation accuracy
- Mode: max
- Factor: 0.5
- Patience: 25
- Threshold: 1e-3
- Semi Supervising: True
- Semi Supervising Threshold: 0.65
- Pseudo Threshold: 0.90
- Breaking Threshold: 100

### Transformations

- RandomResizedCrop
- RandomVerticalFlip
- RandomHorizontalFlip
- RandomInvert
- ColorJitter
- RandomAffine
- RandAugment
