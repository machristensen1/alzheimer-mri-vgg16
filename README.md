For this project, we will task a CNN to classify MRI scans of brains in various stages of dimensia.

https://huggingface.co/datasets/Falah/Alzheimer_MRI

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

This dataset is highly imbalanced. This can lead to poor model performance which, in the healthcare realm, could potentially lead to poor patient outcomes. Being able to detect dimension as early as possible can allow of We will attempt to resolve the imbalanced dataset through the following:

* Data augmentation
* Pre-training/transfer learning

For data augmentation, we will be augmenting our dataset through random cropping, zooming, rotation, and noise. For transfer learning, we will be taking advantage of the VGG19 Neural Network that is commonly used in other image classification algorithms.

https://www.tensorflow.org/tutorials/structured_data/imbalanced_data
