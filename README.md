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
Clone the Butterfly Swarm and the MediaPipe repositories. Follow this [link](https://www.youtube.com/watch?v=Cx4Ellaj6kk&t=644s) to download MediaPipe.
### 2. Importing MediaPipe: 
Copy the "MediaPipe" node from the MediaPipe file (Cmd + C) and paste (Cmd + V) into the Butterfly Swarm file. Then, connect the "MediaPipe" Node to the "hand-tracking" node already in the TouchDesigner File. Disable all the detections from the MediaPipe aside from the Hand Tracking variable. 

### 3.Installing the Background: 
Take the "Background.jpeg" file and drag it directly into Touch Designer. Replace the "BACKGROUND_HERE" node with the background file. Attach the background file to the bottom of the "over1" node. If you want to use your background, this is where you would replace the background. 

### 4. Installing the Butterfly: 
Go into "geohand1" and look for the "moviefilein2" node. Drag the "butterfly2" file into the file section of the node. Do the same for "geohand2"; drag the second file into the "moviefilein2" node. If you have your own sprite you would like to use, you can place the sprite frames here. 
![screenshot(touchdesigner)](https://github.com/user-attachments/assets/f26be11f-83d9-4b0c-a384-de3f5a81b80e)

### 3. Using OBS (optional):  
If you are using multiple filters or quickly switching the filer on and off, you can follow the instructions already in the TouchDesigner to connect with Open Broadcaster Software. 
### 4. Running the filter: 
To run the filter, press the small image icon on the top left of the screen.
![Screenshot 2025-03-27 at 4 42 31 PM](https://github.com/user-attachments/assets/d2b6b69a-4a75-4613-be55-003de0d3fc7b)
