Hurricane Predictor
=====================

**An application to predict hurricanes and help cities plan and prepare.**

### Brief Description

This application aims to predict hurricanes using **satellite imagery** and accordingly predict what course of action would be appropriate
according to the current status of the hurricane. It also aims to predict the **level of hazard** to the areas that are in the or surrounding the
areas of effect of the winds.

The satellite imagery would be processed to detect cloud formations. The application then checks the **optical flow** between adjacent images
to capture cloud motion. This then will be used to determine the areas that might get hit by the hurricane. Some of the various factors that might
have to be accounted for are **rotation**, **velocity**, etc.

Once the areas/regions that have been predicted as being in the hazard zones have been identified, a list of various measures that might have
to be taken will be shown. One example would be predicting the closest and safest regions for evacuating the people from the areas in the hurricane's
path.
