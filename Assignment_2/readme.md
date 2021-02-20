# Homework Assignment 2 for CMPE258

Screenshot along the way are included. Notes for specific items of note below

## Hello AI Platform (Unified)
Pretty much followed the instructions. I did run into some issues when selecting too low of a compute resource so one of the endpoints did not deploy properly, and I can't remove it. This also won't allow me to delete the model. Will need to figure out how to remove the whole project once this homework is submitted.

I did notice the image classification is the most expensive to run, followed by the video classification.

## AutoML Vision Edge
I tried to follow the instructions from codelab, but Firebase no longer supports training with AutoML directly and instead asks you to go to the console.
*AutoML Vision Edge model training is now only available in the Google Cloud console.*

I was able to use the AI Platform Console to train the edge model and then download the .tflite file. ~3MB. It was not as straightforward as the tutorial made it seem, as I ran into a lot of permission issues and had to adjust the IAM settings.

## Time Series Forecasting
Followed the tutorials, screenshots included in the time series forecasting folder. I did run into issues with the 2nd and 3rd notebook provided, I'm guessing some of the default options have changed since the writing of the tutorial. In the 2nd notebook I had to make sure that the ConvergenceWarning package from sklearn is imported.

In the 3rd notebook, the region for the model needed to be explicitly set to 'global', otherwise it sits there waiting on the prompt.

## Overall Impression
Overall, this is a very good overview of the AutoML platform. Seems like cost would run up pretty quick if used in a production environment.
