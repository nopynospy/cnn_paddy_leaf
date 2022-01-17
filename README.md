# CNN Paddy Leaf Disease Classification

Does transfer learning improve paddy leaves disease classification?
This is a classification task with four classes, which are brown spot, hispa, leaf blast and healthy.

The dataset is found at https://www.kaggle.com/minhhuy2810/rice-diseases-image-dataset

Senan et al. (2020) used a convolutional model on the dataset at 70:30 and 50:50 train-test ratio and achieved 90% and 96% test accuracy. On the other hand, Trinh (2021) used DenseNet169 and obtained 80% validation accuracy at 80:20 train-test ratio.

Benchmark 1: https://www.researchgate.net/profile/Muhammad-Aamir-5/publication/343420028_An_Efficient_Convolutional_Neural_Network_for_Paddy_Leaf_Disease_and_Pest_Classification/links/5f5e11bb299bf1d43cffe6f2/An-Efficient-Convolutional-Neural-Network-for-Paddy-Leaf-Disease-and-Pest-Classification.pdf

Benchmark 2: https://www.kaggle.com/huyquoctrinh/transfer-learning-with-data-augmentation-densenet/notebook

# Conclusion

At train-test split ratio of 70:30, the best model is the convolutional model suggested by Senan et al. (2020) with the addition of a dropout layer. Although the train and validation accuracies were 73%, due to class imbalance, the auc revealed that the actual validation auc was only 59%.