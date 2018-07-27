# camera_model
Built a CNN model to identify the camera (out of 10 models) with which an image was shot.

My best submission got me a Leaderboard score of 0.9728, with a final Leader board rank of 33 out of 582 (top 6%).
As a result of this, I was awarded a silver medal for this competition.

| File Name | Description | Kaggle LB score (accuracy score) |
|--|--|--|
| 01_image_size_selection.ipynb | Analysed the train image sizes | - |
| 01_train_validation_split.ipynb | Contains all data processing like getting external data, cropping |   -  |
| 03_ResnetV2_unalt.ipynb | Trained all the layers of ResNet-50 model initialised with imagenet weights. Trained with only unaltered images | 0.9539 |
| 03_ResnetV2_image_aug.ipynb | Trained all the layers of ResNet-50 model initialised with 03_ResnetV2_unalt weights. Trained with manipulated images | 0.9539 |
| 03_ResnetV2_image_aug_multiprocessing.ipynb | Same version as 03_ResnetV2_image_aug, but trained with multiprocessing | - |
| 03_ResnetV2_unalt_multiprocessing.ipynb | Same version as 03_ResnetV2_unalt, but trained with multiprocessing | - |
| 04_CACNN_unalt.ipynb | Implemented content-adaptive CNN from this [paper](https://arxiv.org/pdf/1703.04856.pdf), and trianed on unaltered images | - |
| 04_CACNN_image_aug.ipynb | 04_CACNN_unalt implementation, but trained on manipulated images | - |
| 05_MobileNet_unalt.ipynb | Trained all the layers of MobileNet model initialised with imagenet weights. Trained with only unaltered images | 0.9639 |
| 05_MobileNet_image_aug.ipynb | Trained all the layers of MobileNet model initialised with 05_MobileNet_unalt weights. Trained with manipulated images | 0.9639 |
| 06_DenseNet_unalt.ipynb | Trained all the layers of DenseNet201 model initialised with imagenet weights. Trained with only unaltered images | 0.9722 |
| 06_DenseNet_image_aug.ipynb | Trained all the layers of DenseNet201 model initialised with imagenet weights. Trained with manipulated images | 0.9722 |
| 07_Ensemble_ml.ipynb | Ensembled all the above models using normal mean, logistic, random forest, xgboost | 0.9739(mean) |
| 07_Ensemble_ml_logistic.ipynb |  Ensembled all the above models with seperate logistic regression model for each class | 0.9728 |
