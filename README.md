Cyclone Predictor
=====================

*"If you know the enemy and know yourself, you need not fear the result of a hundred battles."*

Every year cyclones cause significant damages to property and human life. But with the development of modern systems shall we still be at the mercy of the environment? We hope our application will help predict the motion of such Cyclones before they hit land and thus can create a difference to the world.

### Brief Description

This application aims to predict cyclone using **satellite imagery** and accordingly predict what course of action would be appropriate
according to the current status of the cyclone. It also aims to predict the **level of hazard** to the areas that are in the or surrounding the
areas of effect of the winds.

The satellite imagery would be processed to detect cloud formations. The application then checks the **optical flow** between adjacent images
to capture cloud motion. This then will be used to determine the areas that might get hit by the cyclone. Some of the various factors that might have to be accounted for are **rotation**, **velocity**, etc

Once the areas/regions which lie in the path of the cyclone are identified the government can be informed and the will undertake the necessary precautions and preemtive measures can be deployed. This in itself will reduce the loss of human life and prevent huge damages to property and life.

### Base Idea

Decompose the image sequence into a set of frames. Use each pair of succesive frames and compare the optical flow. Then smooth and decompose the optical flow. Use the properties of the flow field to identify the vertex cores which could comprise the storm cells. The visual information obtained from the image and optical flow can be used to build the descriptor of each extracted vortex core.

### Implementation Features

- Training data
   - This would entail the retrieval of satellite weather images.
   - Will be accomplished using Python library(s) like SatPy which can retrieve satellite images.
   - Using this library we can not only obtain the satelite data but also resample the data.
   - The library already provides the necessary atmospheric corrections and visual enhancements.


- Classification
  - Train a random forest by using the training data.
  - The Random forest is an ensemble learning algorithm that makes predictions by combining the results of multiple individual decision trees trained from random subsets of the training data.


- Storm Feature Extraction
   - Using formations information to determine/predict cloud motion by taking into account various other factors (rotation, divergence, velocity, & coriolis effect)
   - This can be accomplished using the optical flow technique, applied between adjacent images.
   - We can then use the flow field is used to identify local vortex regions, which are the potential storm systems.
   - We also need to keep in mind the relative rotation of the satelite and certain smoothening must be applied.


- Application of Predictions
   - Use the obtained predictions to check areas that will likely be affected.
   - Cross-verifing the path of the predicted cloud formation with pre-loaded maps.
   - Alert the respective organisations the path and impact of the Cyclone.

### Technologies used

1. Python
2. Azure
