# Tenki
End-to-end image classification model using AWS SageMaker's built-in algorithm that classifies different weather conditions.

## Key Features
- No pre-trained models
- SageMaker GPU training (ml.g4dn.xlarge) on ~1500 images
- Handled data issues: corrupt images, S3 quota requests
- Achieved **88.9% validation accuracy** from scratch
- Batch transform for test set predictions
- Kaggle submission: 0.515 public score

## Tech Stack
- Amazon SageMaker (training, transform)
- Amazon S3 (data storage)
- MXNet built-in image-classification algorithm
- Python, boto3, pandas, numpy

## Results
- Best validation accuracy: **88.89%** (Epoch 14)
- Leaderboard position: 6/9 (public)

Some issues i faced and resolved.
- SageMaker quota troubleshooting (Service Quotas request)
- Data cleaning (deleted corrupt .jpg files)
- LST file format for built-in algo
