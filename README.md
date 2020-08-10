# Licence-Plate-Detection-and-Recognition-System

Licence Plate Detection System is an Automatic License Plate Recognition of vehicles (mainly 4 wheelers) using SVC Classifier.
With increasing number of vehicles on roads, it is getting difficult to manually enforce laws and traffic rules for smooth traffic flow. Toll-booths are constructed on freeways and parking structures, where the car has to stop to pay the toll or parking fees. Also, Traffic Management systems are installed on freeways to check for vehicles moving at speeds not permitted by law. All these processes have a scope of improvement. In the center of all these systems lies a vehicle. In order to automate these processes and make them more effective, a system is required to easily identify a vehicle.

## PROPOSED SOLUTION:

The obvious answer to the above problem is by using the vehicle’s number plate. Vehicles in each country have a unique license number, which is written on its license plate. This number distinguishes one vehicle from the other, which is useful especially when both are of same make and model. An automated system can be implemented to identify the license plate of a vehicle and extract the characters from the region containing a license plate. The license plate number can be used to retrieve more information about the vehicle and its owner, which can be used for further processing. Such an automated system should be small in size, and portable.

### IDEA:

LPR sometimes called ALPR (Automatic License Plate Recognition) has 3 major stages.

#### *License Plate Detection:*

This is the first and probably the most important stage of the system. It is at this stage that the position of the license plate is determined. The input at this stage is an image of the vehicle and the output is the license plate. In this stage, the position of the rectangular number plate in the input image is detected. Then the detected number plate is extracted out from the image, to serve as the input to the next stage i.e., Character Segmentation stage. The approach used in this work for License Plate detection is based on Otsu BInarization and Connected Component Analysis (CCA).

#### *Character Segmentation:*

It’s at this stage the characters on the license plate are mapped out and segmented into individual images. Character segmentation is the procedure of extracting the characters and numbers from the license plate image. Diverse aspects make the character segmentation task complicated, like image noise, plate frame, space mark, plate’s rotation and light variance. A number of procedures have been proposed for character segmentation to overcome these problems. After removing the plate borders in the previous step, this step starts with removing the noise from the plate. The approach used in this work for character segmentation is based on Adaptive thresholding, morphological processing and contour tracing.

#### *Character Recognition:* 

This is where we wrap things up. The characters earlier segmented are identified here. We’ll be using machine learning for this. After the segmentation of elements (characters and numbers), the final module in the license plate recognition process is character recognition. It’s at this stage we introduce the concept of machine learning. Although there are many techniques present and applied for character recognition like statistical, syntactic and neural networks in this research, character recognition is performed by using feature extraction. We’ll be taking the path of supervised learning because we already have an idea of how As, Bs and all the letters look like. Supervised learning can be divided into two categories; classification and regression. Character recognition belongs to the classification category. 

To execute this phase, we need to get a training data set, choose a supervised learning classifier, train a model, test the model and see how accurate it is, then use the model for prediction.

There are several classifiers we can use with each of them having its advantages and disadvantages. We’ll use SVC (support vector classifiers) for this task. I chose to use SVC because it gave me the best performance. However, this does not necessarily mean that SVC is the best classifier.

## PRESENTATION:
https://drive.google.com/file/d/17kCSqDIrjCDMSeeqQHhJLUNRKCt5gR2Y/view?usp=sharing
