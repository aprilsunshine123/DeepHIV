# DeepHIV
The codes for DeepHIV

Viral metagenomic sequencing data have become a main resource for discovering new viruses or diverged strains of known viral families.  As different strains may have different biological properties such as virulence and resistance to anti-viral drugs, fine-grained composition analysis should be applied to viral metagenomic data. In this work, we applied deep learning models for subtype-level viral read classification. Although deep learning-based models have had successful applications in sequence analysis such as predicting protein/RNA binding intensities and protein domain classifications, unique challenges still exist for applying deep learning models to fine-grained sequence classification. First, as metagenomic assembly is error-prone, we will conduct classification on reads directly. Compared to using longer or more complete contigs for training, using reads as the training and testing data poses a challenge for automatic feature learning. Second, the difference between the intra and inter sequence similarities is small for fine-grained classes such as HIV subtypes and thus can lead to mis-classification.  

We applied convolutional neural network (CNN) models to HIV subtype classification and compared the output with read mapping-based methods. The first set of experiments were conducted using simulated reads from available HIV subtypes' genomes. With known labels of all the simulated reads, we can perform careful comparison between CNN-based models and the read mapping strategy. The results showed that CNN-based model can achieve higher accuracy than read mapping when there are sufficient training genomes. We then applied our model to real human plasma datasets in order to test whether it can recognize HIV reads and conduct correct classification. The results showed that our model successfully rejected a majority of reads from other microbes while accurately classifying HIV reads into their originating subtypes.  

This study demonstrated that even with partial sequences as input, deep learning models can still successfully conduct fine-grained read classification with sufficient training data. The trained model, named DeepHIV, can be downloaded here.
