# AME520Fall2022 Final Project Written Description

## Project Title: 
* VR Integrated Character Animation Interactive System
## Design Goals: 
* To explore the application of neural perception theories such as embodied/disembodied cognition and enactivism in spatial phenomenology through computer graphics technology. The practice should use computer-generated visual information to have some effect on human cognition, such as optical illusions, and correct or adapt them in motion.
## Target Audience: 
* Anyone interested in the above field and curious about its impact on the development of complex interactive systems/video games.
## Project Background & Expectations：
* In my previous study and research, I have been able to use the shader nodes in Blender to make texture materials that can respond differently to light sources. In order to give the perceiver a different visual experience simultaneously about whether the object is a three-dimensional or two-dimensional digital representation by changing the direction of the light source in the environment under the condition of a given position and viewing angle.
![image load](https://github.com/XiangFan49/AME520Fall2022/raw/main/Assignment/Final%20Project/Previous%20Work%20Display.png =100x200px)
![image load](https://github.com/XiangFan49/AME520Fall2022/raw/main/Assignment/Final%20Project/Shader%20Node%20Display.png)
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

### Stage 3: Make an Animation for the Character (Blender & Optitrack)
* Skeleton rigging to make the bones to drive the mesh of the 3D model
* Generate data through motion capture.
* Bind motion capture data to skeleton for animation
### Stage Results：
![image load](https://github.com/XiangFan49/AME520Fall2022/raw/main/Assignment/Final%20Project/Stage%203%20Animation.png)

### Stage 4: Design Interaction Mechanism (Unity)
* Make animation controller
* Add controller to the character
* Import a simple scene
* Make a camera that can move with the character and adjust the viewing angle according to the mouse position
### Stage Results：
![image load](https://github.com/XiangFan49/AME520Fall2022/raw/main/Assignment/Final%20Project/Stage%204%20Design%20Interaction%20Mechanism.png)

## Design Gaps:
* At the beginning of the research and development of the project, it was considered to be designed as a real-time interactive system. However, in the actual attempt, it was found that the plug-in originally thought to transmit data from Motive to Unity in real time could not be used, so it had to be displayed with pre-recorded animation
* When doing texture baking, because it is not clear how the rendering system is composed in Unity, many material details are lost when imported from Blender to Unity
* Because the project went through a significant workflow shift halfway through development, there was no time to add collision volumes and fluid effects to the clothes, making the clothes in the animation appear like rigid bodies
* Also for the same reason as above there was no time to make the scene

## Project Future Outlook (In Order of Priority):
* Solve the problem of real-time motion capture data transmission. Possible reference solution: use VR equipment to complete motion capture and playback at the same time
* Create scenes that generate optical illusions
* Familiar with the use of shaders in Unity to optimize non-photorealistic rendering of models
* Add physical effect attributes to models and objects in the scene

Final vision for the future
