# Multiple Object Detection and Kangaroo Detection Web Apps 


In this project, our team developped two object detection web apps hosted on different platforms. 

## Part I : Multiple Object Detection Web App

This Flask app loads a pre-trained Tensorflow.js model using the ImageNet dataset. It can take in two forms of image inputs: static images or via webcam and outputs predictions. 

**Installation in the cloud**

An image is built and stored in Amazon ECR. From there, the application is easily  deployed  in App Runner.

**Installation locally**

if Docker is installed, the following commands can be run:
```properties
docker build -t flask-object-detect-app:latest
```
After the build completes, you can run the container:

docker run -d -p 5000:5000 object-detect


## Part II : Kangaroo Detection Web app using Transfer Learning

What if we wanted to detect specific objects? Like Kangaroo...? In this case, we retrain/validate the model on all kangaroo images and save this new model. This time, the application can only detect kangaroo like pictures(webcam or pictures).

The app is hosted on Glitch and can be accessed here(*add*). All you need to do is click on the preview button


## Cloud Architecture

![new](https://user-images.githubusercontent.com/47464258/164947189-8655c683-3252-4c80-8a00-dcfc42ad2a61.png)

## Credits
This project was inspired by
- https://codelabs.developers.google.com/tensorflowjs-transfer-learning-teachable-machine#8
- https://codelabs.developers.google.com/codelabs/tensorflowjs-object-detection
- https://towardsdatascience.com/custom-real-time-object-detection-in-the-browser-using-tensorflow-js-5ca90538eace
