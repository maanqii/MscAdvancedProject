# MscAdvancedProject
## YouTube video link:
## File Download:
Due to the large size of the UE (Unreal Engine) files, they cannot be directly uploaded to Github. Therefore, here is the link to the source files. Open it to download and view the original project:

## Project Progress Blog:

My progress blog records the entire project's planning and execution process in the form of logs, aiming to provide a detailed description of each stage of the project. Throughout this process, I received enthusiastic support and professional guidance from my mentor Phoenix, and our weekly video communications became a crucial driving force for the project.

Firstly, from July 21 to August 4, I focused on Unreal Engine, conceptualizing and building a rough scene (blockout) through blueprints. This stage serves as the prototype of the overall game framework, allowing me to quickly and flexibly establish the basic structure of the game through visual scripting. Simultaneously, I designed the form of the entire scene, transforming thoughts into visual concepts through sketches. During this process, I referred to and watched learning videos related to UE5 to deepen my understanding of the engine. Creating characters using Metahuman was a key step during this period. Through exporting and binding skeletons, I could see the effects of the main characters in the scene. Although 3D sculpting of clothes was not complete, I started conceptualizing the storyline for the entire game, laying the foundation for subsequent blueprint creation.

From September 25 to October 2, I focused on completing the creation of the main character and integrating it into the scene. Specifically, I completed the animation design for the character's clothes. At the same time, I built the overall environment, roughly completing the scene. During this period, I began using Blender to create some detailed objects to further enrich the game environment. The role of blueprints will be more prominent in this process. By constructing interaction blueprints, I can achieve more complex interactions between the main character and the environment, adding depth and interest to the game.

Next, from October 7 to October 21, I dedicated myself to designing the user interface panel, building the blueprint for the main menu, and creating interaction pages for all interactive objects in the main scene. During this period, I expanded the use of blueprints to the UI and overall interaction design of the game, ensuring that players can interact smoothly and intuitively with the game world. Simultaneously, I ensured that all details of the scene were placed in appropriate positions, making the entire game world more realistic and engaging.

From October 21 to October 28, I will focus on the start page of the game and scene lighting rendering. At the same time, I will write the script for the entire game scene, adding more story elements to the game world. During this stage, I will also look for relevant textures, generate the required images through AI, and create elements such as tarot cards to enhance the visual appeal of the game. The application of blueprints will include the launch logic of the game, scene rendering, and the integration with AI-generated images and tarot cards, bringing a richer and more diverse experience to the entire game.

From October 28 to November 11, I will allocate time to review literature and write the thesis, which is a relatively independent part of the project. It will mainly focus on completing all the content of the thesis while starting the production of the game ending. Based on the setting of portals, I need to design three different endings, requiring me to cleverly handle the branching and ending logic of the game in blueprints. At the same time, I will continue the work of AI image generation, providing high-quality visual materials for the ending scene of the game.

In the final period, from November 11 to November 18, I will focus on the later revision of the thesis and the addition of images, ensuring the integrity and professionalism of the thesis. At the same time, I will address any potential bugs in the game to ensure its stability. During this period, I will also edit videos, preparing for the final presentation of the project. The role of blueprints will involve the logic implementation of the game ending, bug fixes, and collaborative work with video editing.

This series of blueprint work will run throughout the project, from building scenes, character interactions, UI design, game launch logic, to the ending and final presentation. Blueprints will be a powerful tool for realizing my game design concepts. Through the clever application of blueprints, I hope to create a narrative game rich in story and interactivity, providing players with a deep and unforgettable experience.

## Brief Overview of Project Blueprints:

### Door Interaction Blueprint:

1. **Rotating Door Orientation Check:**
   - Use a trigger to detect if the player is near the door.
   - Use blueprints to determine the player's orientation and identify the door's direction.
   - If the orientation meets the requirements, allow the player to interact.

2. **Authenticity Check for the Key:**
   - Set up a trigger or interaction point to allow players to pick up the key.
   - Use blueprints to verify if the picked-up key is genuine.
   - If it is genuine, allow the door to open.

3. **Locked State Check for Door Opening:**
   - Establish a state variable in the blueprint to indicate whether the door is in a locked state.
   - When the player interacts, check the door's locked state.
   - If the door is locked, maintain its current state and do not perform the opening operation.

4. **Door Sound Response:**
   - Add audio components in the blueprint.
   - Trigger corresponding sound effects when the door is opened or closed.
   - Consider using audio triggers to play sounds when specific events occur.

5. **Modeling Details:**
   - Use 3D modeling tools to divide the door into two parts, rotating only the central portion.
   - Ensure the door's collision volume matches the trigger for correct interaction events.
   - Avoid unnecessary complexity and keep the model clear and simple.

<img width="1149" alt="fecd67e8c60017086b915e535c75156" src="https://github.com/maanqii/MscAdvancedProject/assets/119876408/6c75f4dc-9ba2-4ddb-89d8-7204c5249631">
<img width="1151" alt="61b0cb3b8a9c72a33b1fddbed87c909" src="https://github.com/maanqii/MscAdvancedProject/assets/119876408/1f2c7877-3ca4-4695-9861-c5dd2bbd18fe">
