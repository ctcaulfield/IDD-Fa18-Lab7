# Video Doorbell, Lab 7

*A lab report by Christopher Caulfield*

### In This Report

1. Upload a video of your version of the camera lab to your lab Github repository
1. As usual, update your class Hub repository to add your [forked IDD-Fa18-Lab7](/FAR-Lab/IDD-Fa18-Lab7) repository.
1. Answer the questions in-line below on your README.md.

## Part A. HelloYou from the Raspberry Pi

**a. Link to a video of your HelloYou sketch running.**
https://youtu.be/CNPdow5xZWg

## Part B. Web Camera

**a. Compare `helloYou/server.js` and `IDD-Fa18-Lab7/pictureServer.js`. What elements had to be added or changed to enable the web camera? (Hint: It might be good to know that there is a UNIX command called `diff` that compares files.)**
The main change in the additional takePicture function which allows the user to take a picture. Within the function is a call to the npm NodeWebcam which takes the picture. On the html side, there is a new line of code for displaying the image. 

**b. Include a video of your working video doorbell**
https://youtu.be/JwGueAVJjwc

## Part C. Make it your own

**a. Find, install, and try out a node-based library and try to incorporate into your lab. Document your successes and failures (totally okay!) for your writeup. This will help others in class figure out cool new tools and capabilities.**

I decided to use the Google Vision NPM package - https://www.npmjs.com/package/@google-cloud/vision.

When you hit the doorbell button the image is snapped via camera and sent to Google Vision. It then returns back a JSON of the data. In my case I wanted to know how many people were in the picture.

If there is one person in the photo - you are welcome to come inside! If there are 2 or greater - you cannot enter. If there is nobody - I basically joke and say "nice try!".

Failures: I had no failures because I am a Google Cloud Platform Wizard. 

**b. Upload a video of your working modified project**
https://youtu.be/Sv09ljI76L8
