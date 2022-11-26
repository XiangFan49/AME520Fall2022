# AME520Fall2022 Final Project Written Description


## Project Title: 
* Irena in Wonderland
## Design Goals: 
* To explore the application of neural perception theories such as embodied/disembodied cognition and enactivism in spatial phenomenology through computer graphics technology. The practice should use computer-generated visual information to have some effect on human cognition, such as optical illusions, and correct or adapt them in motion.
## Target Audience: 
* Anyone interested in the above field and curious about its impact on the development of complex interactive systems/video games.
## Project Expectations：
* After experiencing the somatic lesson this semester, I have a deeper understanding of embodied cognition than I originally had while reading the literature. By following the guides, I was able to concentrate my focus on my body so that I could feel its structure from the movement. I hope to apply this understanding to my project, which before then, I only conceived at the stage of static perception from computer-generated images. So after experiencing the Optitrack optical motion capture system, I think I can build a real-time responsive interactive system to record users' actions while allowing them to observe their own movements from a third-person perspective through a digital avatar.
* Based on these considerations, the final project should be able to allow participants to observe the representations of their movements in real time through VR glasses and perform simple interactions in a digital scene. During this process, the optitrack motion capture suits on their bodies will transmit their motion data to Motive in real time and transfer it to Unity through this software. These data should then activate the skeleton of the 3D model in Unity to generate animation, while the rigged 3D model and the digital scene will be made in Blender.
## Workflow:
### Stage 1: Creating the 3D Model (Blender)
* Sculpt the geometry of the model
* Color the model with shader nodes
### Stage Results：
![image load](https://github.com/XiangFan49/AME520Fall2022/raw/main/Assignment/Final%20Project/Stage%201%203D%20Modeling.png)

### Stage 2: Import the Model into Unity (Blender & Unity)
* Make expandable UV maps for models
* Bake the model's shader nodes into textures
* Import the model into Unity in FBX mode and reconnect the model texture there
### Stage Results：
![image load](https://github.com/XiangFan49/AME520Fall2022/raw/main/Assignment/Final%20Project/Stage%202%20Import%20the%20model%20into%20Unity.png)

### Stage 3: Make an animation for the character (Blender & Optitrack)
* Skeleton rigging
* Generate data through motion capture.
* Bind motion capture data to skeleton for animation
### Stage Results：
![image load](https://github.com/XiangFan49/AME520Fall2022/raw/main/Assignment/Final%20Project/Stage%203%20Animation.png)

### Stage 4: Design Interaction Mechanism (Unity)
* Add controller to the character
* Make animation controller
* Import a simple scene
* Make a camera that can move with the character and adjust the viewing angle according to the mouse position
