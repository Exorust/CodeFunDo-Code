Cyclone Predictor
=====================

**An application to predict cyclone and help cities plan and prepare.**

### Brief Description

This application aims to predict cyclone using **satellite imagery** and accordingly predict what course of action would be appropriate
according to the current status of the cyclone. It also aims to predict the **level of hazard** to the areas that are in the or surrounding the
areas of effect of the winds.

The satellite imagery would be processed to detect cloud formations. The application then checks the **optical flow** between adjacent images
to capture cloud motion. This then will be used to determine the areas that might get hit by the cyclone. Some of the various factors that might have to be accounted for are **rotation**, **velocity**, etc.

Once the areas/regions that have been predicted as being in the hazard zones have been identified, a list of various measures that might have
to be taken will be shown. One example would be predicting the closest and safest regions for evacuating the people from the areas in the cyclone's path.

### Implementation Steps

1. Retrieval of satellite weather images.
   - This will be accomplished using Python library(s) like SatPy which can retrieve satellite images.
2. Processing of weather images to detect cloud formations.
   - This will use image processing algorithms using neural network structures.
3. Finding patterns in cloud formations.
4. Using formations information to determine/predict cloud motion by taking into account various other factors(rotation, velocity, etc.)
   - This can be accomplished using the optical flow technique, applied between adjacent images.
5. Using the predictions to check areas that will likely be affected.
   - Cross-verifing the path of the predicted cloud formation with pre-loaded maps.

### Technologies used

1. Python
2. Azure
