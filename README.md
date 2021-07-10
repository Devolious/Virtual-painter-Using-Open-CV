# Virtual-painter-Using-Open-CV
In the decade where everyone is locked in their home and online education is the only way out, my project brings in a cost effective and helpful solution for helping teachers in rural areas and from poor background who can't avail those costly typewriters and present on screen, I have devised a method which involves writing virtually infront of Webcam screen which will be displayed in output screen which can be screen shared and presented to students. My model will act as a virtual writing board for writting and conveying something to viewers.

Along with it can be useful in corporate meets also as one doesn't need anything to visualize a project and can draw using his own hands.It can be used as painting screen for children also which they can use for scribbling and this can be added as a feature in any meeting app which may bring a jovial atmosphere of drawing abstract figures around someone's face. These happiness and helpfulness is all I try to bring through this project.

I did a similar project related to it (Can be found in my repository) in which instead of hand-tracking I used a blue tip to draw but it had certain shortcomings like its quite hard to stop scribbling and cover the tip when not to scribble and was a bit messy too, this project is certainly an improvement over the previous project.

Coming to the **Technical aspect of Virtual Painter-cum-Writing Board**.

Here three paint brushes are available namely Pink,Blue,Green and eraser.The top UI of my model was designed in Canva.org and are accumulated in Headers folder.

**Process:-**
Firstly I overlayed the first image in headers over my screen and webcam was continuously captured.For Hand Detection Mediapipe module was used in my project, Mediapipe hand detection is based on finding 21 3D landmarks in our hands I drew all the landmarks on my screen and connected all the landmarks using lines now the lines on connection gave an impression of my hand. Multi-Hand landmark was used for at max 1 hand and all the landmark points were recorded and stored as its of utmost importance for us, also the distances were found between different landmarks and certain criteria was selected for observing whether fingers are up or not (based on distance of tips of fingers).

Detection Confidence was choosen around 0.65 and maxHands was set to 1 in our project case. If two fingers are up then we are in selection mode, then we observe in which portion of top the fingers lie so that that color is choosen and header image is changed in canvas too. For drawing and writing mode only index finger is up and when all fingers are up canvas is cleared. Finally after making some thresholding and binary operations we get our final canvas in which we can scribble and write easily and erase easily too.

**Scope of Improvement:-**
* It can be deployed in some application as a feature.

Thank you and as always ALL SUGGESTIONS ARE WELCOME !!
