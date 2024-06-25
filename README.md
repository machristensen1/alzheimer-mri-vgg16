The dataset we'll be using (`Falah/Alzheimer_MRI`). There are four labels:

    '0': Mild_Demented
    '1': Moderate_Demented
    '2': Non_Demented
    '3': Very_Mild_Demented

From: https://www.dementiacarecentral.com/aboutdementia/facts/stages/ 

* Very Mild:
    * Forgets names
    * Misplaces familiar objects
    * Symptoms not evident to loved ones or doctors
* Mild:
    * Increased forgetfulness
    * Slight difficulty concentrating
    * Decreased work performance
    * Gets lost more frequently
    * Difficulty finding right words
    * Loved ones begin to notice
* Moderate:
    * Difficulty concentrating
    * Forgets recent events
    * Cannot manage finances
    * Cannot travel alone to new places
    * Difficulty completing tasks
    * In denial about symptoms
    * Socialization problems: Withdraw from friends or family
    * Physician can detect cognitive problems

This dataset is highly imbalanced. This can lead to poor model performance potentially leading to poor patient outcomes. We will attempt to resolve the imbalanced dataset through the following:

* Data augmentation
* Pre-training/transfer learning

For data augmentation, we will be augmenting our dataset through random cropping, zooming, rotation, and noise. We will also be taking advantage of the VGG16 Neural Network commonly used in other image classification tasks. The VGG16 model will be pre-trained on the ImageNet dataset.

Further resources on imbalanced data:


https://www.tensorflow.org/tutorials/structured_data/imbalanced_data
