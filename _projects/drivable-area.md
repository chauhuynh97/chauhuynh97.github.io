---
title: "Drivable Area Detection"
excerpt: "This project applied a simplified U-Net architecture to perform drivable areas detection. This architecture provides a solid way to classify each pixel as belonging to a drivable surface or not. After implementing, training, and testing with the Berkeley Deep Drive dataset, the CNN model was able to predict drivable area by an accuracy of 81%. For comparison, a baseline classification algorithm was implemented using logistic regression. The accuracy of the baseline algorithm is 56%. The model was able to increase the accuracy by around 30%."
permalink: /drivable-area
collection: projects
---


Image segmentation is a critical part of autonomous vehicle perception algorithms. In this paper, we present a Convolution Network architecture to detect drivable surface area on images taken from the dashboard of vehicles. The convolution network developed in this project is heavily influenced by U-Net, the state of the art in medical image segmentation, which relies mainly on augmented data rather than a large dataset to train the network. We show that this medical image segmentation technique is quite practical for drivable area detection for autonomous vehicles. We trained and tested the network on images and labels from the Berkeley Deep Drive (BDD) dataset and achieved outstanding results on clear, daytime images of roads and satisfactory results on nighttime and crowded images. The network is fast and can keep up with the bandwidth of on-demand drivable area detection for autonomous driving applications. 

![U-Net architecture](https://chauhuynh97.github.io/images/U-Net-architecture.png)

![Daytime example of input image, label image, and predicted output image](https://chauhuynh97.github.io/images/drivable-area-daytime-prediction.png)

![Nighttime example of input image, label image, and predicted output image](https://chauhuynh97.github.io/images/drivable-area-nighttime-prediction.png)

