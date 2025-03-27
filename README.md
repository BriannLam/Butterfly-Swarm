# Butterfly Swarm

## Description:

Butterfly Swarm is an Effect using TouchDesigner with multiple butterflies flying across the screen until you put your hand up to the camera. Then, the butterflies will flock towards your hand, forming a ring in the area where your hand is. The swarm will then proceed to follow your hand on the screen as you move your hand in the real world. When you close your hands, the butterflies will disperse. 

## Requirments: 

### [TouchDesigner](https://derivative.ca/download)  
TouchDesigner is the program in which the effect is run and edited. Implementation instructions will be at the end of the document. This file was made on the TouchDesigner v2023.12230 
### [MediaPipe](https://github.com/torinmb/mediapipe-touchdesigner)  
I used the MediaPipe made by Torin Blankensmith; the MediaPipe is the thing that captures the movements and actions of the hands so the butterflies can track them. This file was made on the MediaPipe v0.5.0.  
### Camera  
A camera is needed to capture the motion of the hands.  

## Implementation: 

### 1. Download:  
Download the Butterfly Swarm and the MediaPipe files and open them up. 
### 2. Importing MediaPipe: 
Copy the MediaPipe from the MediaPipe file (Cmd + C) and paste (Cmd + V) into the Butterfly Swarm file. Then, connect the MediaPipe Node to the hand-tracking node already in the TouchDesigner File. Disable all the detections from the MediaPipe aside from the Hand Tracking variable.  
### 3. Using OBS (optional):  
If you are using multiple filters or quickly switching the filer on and off, you can follow the instructions already in the TouchDesigner to connect with Open Broadcaster Software. 
### 4. Running the filter: 
To run the filter, press on the small image icon on the top left of the screen
![Screenshot 2025-03-27 at 4 42 31 PM](https://github.com/user-attachments/assets/d2b6b69a-4a75-4613-be55-003de0d3fc7b)


## Modification/Customization: 
### Changing Cameras 
Go to the MediaPipe and Swap the Webcam to the preferred camera. 
### Changing Sprites
Ensure you have all the frames that make up the image in a folder. Then go into geoaHand1 or GeoHand2. Find the MovieFilein Operators and drag your folder with all the frames. 
