# Pose-Classification-Brainhack2020

This was WASD's attempt for the finals of the [DSTA BrainHack 2020](https://www.straitstimes.com/singapore/first-brainhack-event-incorporating-ai-and-cyber-security-elements-draws-1500-students)

Contributors: Daryl Lee, Alvin, Wei Xiong and Si Yu (me!)

## Objective
We were given images of 11 different poses and were supposed to train an image classification model to classify the various poses.
On the second day of the hackathon, we were given 4 more classes and limited time to adjust the model.
## Methodology
### Data Preprocessing
We used the typical image preprocessing techniques such as shearing, brightness, horizontal flipping, etc.
Something interesting that we used was Random Erasing, which was written about in this research paper. https://arxiv.org/abs/1708.04896.

### Model Training
We used transfer learning with multiple models that have been trained on Imagenet. We freezed all the layers and slowly unfreeze them to fine tune.
![Training](/Transfer_Learning.png)

### Ensemble
We trained an ensemble of models to squeeze those last few amounts of accuracy.
![Ensemble](/Ensemble.png)