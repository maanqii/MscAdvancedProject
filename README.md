# MscAdvancedProject
## YouTube video link:
https://youtu.be/43y8P3CNt4Y
## File Download:
Due to the large size of the UE (Unreal Engine) files, they cannot be directly uploaded to Github. Therefore, here is the link to the source files. Open it to download and view the original project:
## Project Progress Blog:
My progress blog records the entire project's planning and execution process in the form of logs, aiming to provide a detailed description of each stage of the project. Throughout this process, I received enthusiastic support and professional guidance from my mentor Phoenix Perry, and our weekly video communications became a crucial driving force for the project.

1. **7.21-8.4：Building the Game Framework**
I focused on Unreal Engine, conceptualizing and building a rough scene (blockout) through blueprints. This stage serves as the prototype of the overall game framework, allowing me to quickly and flexibly establish the basic structure of the game through visual scripting. Simultaneously, I designed the form of the entire scene, transforming thoughts into visual concepts through sketches. During this process, I referred to and watched learning videos related to UE5 to deepen my understanding of the engine. Creating characters using Metahuman was a key step during this period. Through exporting and binding skeletons, I could see the effects of the main characters in the scene. Although 3D sculpting of clothes was not complete, I started conceptualizing the storyline for the entire game, laying the foundation for subsequent blueprint creation.

2. **9.25-10.2：Creation of Main Character and Environment Building**
I focused on completing the creation of the main character and integrating it into the scene. Specifically, I completed the animation design for the character's clothes. At the same time, I built the overall environment, roughly completing the scene. During this period, I began using Blender to create some detailed objects to further enrich the game environment. The role of blueprints will be more prominent in this process. By constructing interaction blueprints, I can achieve more complex interactions between the main character and the environment, adding depth and interest to the game.

3. **10.7-10.21： Designing User Interface and Interaction Blueprints**
I dedicated myself to designing the user interface panel, building the blueprint for the main menu, and creating interaction pages for all interactive objects in the main scene. During this period, I expanded the use of blueprints to the UI and overall interaction design of the game, ensuring that players can interact smoothly and intuitively with the game world. Simultaneously, I ensured that all details of the scene were placed in appropriate positions, making the entire game world more realistic and engaging.

5. **10.21-10.28：Start Page and Scene Lighting Rendering**
 I will focus on the start page of the game and scene lighting rendering. At the same time, I will write the script for the entire game scene, adding more story elements to the game world. During this stage, I will also look for relevant textures, generate the required images through AI, and create elements such as tarot cards to enhance the visual appeal of the game. The application of blueprints will include the launch logic of the game, scene rendering, and the integration with AI-generated images and tarot cards, bringing a richer and more diverse experience to the entire game.

6. **10.28-11.11：Thesis Writing and End Game Production**
 I will allocate time to review literature and write the thesis, which is a relatively independent part of the project. It will mainly focus on completing all the content of the thesis while starting the production of the game ending. Based on the setting of portals, I need to design three different endings, requiring me to cleverly handle the branching and ending logic of the game in blueprints. At the same time, I will continue the work of AI image generation, providing high-quality visual materials for the ending scene of the game.

7. **11.11-11.18：Thesis Editing, BUG Fixes, and Video Editing**
I will focus on the later revision of the thesis and the addition of images, ensuring the integrity and professionalism of the thesis. At the same time, I will address any potential bugs in the game to ensure its stability. During this period, I will also edit videos, preparing for the final presentation of the project. The role of blueprints will involve the logic implementation of the game ending, bug fixes, and collaborative work with video editing.

This series of blueprint work will run throughout the project, from building scenes, character interactions, UI design, game launch logic, to the ending and final presentation. Blueprints will be a powerful tool for realizing my game design concepts. Through the clever application of blueprints, I hope to create a narrative game rich in story and interactivity, providing players with a deep and unforgettable experience.

## Brief Overview of Project Blueprints:

### Door/Drawer Interaction Blueprint:

1. **Rotating Door Orientation Check:**
   - Use a trigger to detect if the player is near the door.
   - Use blueprints to determine the player's orientation and identify the door's direction.
   - If the orientation meets the requirements, allow the player to interact.
     
<img width="1151" alt="61b0cb3b8a9c72a33b1fddbed87c909" src="https://github.com/maanqii/MscAdvancedProject/assets/119876408/14200dca-9a8f-45be-adbd-4283e44a6b09">

2. **Authenticity Check for the Key:**
   - Set up a trigger or interaction point to allow players to pick up the key.
   - Use blueprints to verify if the picked-up key is genuine.
   - If it is genuine, allow the door to open.
     
<img width="1149" alt="fecd67e8c60017086b915e535c75156" src="https://github.com/maanqii/MscAdvancedProject/assets/119876408/f7ef0c78-e644-4a97-bd4e-7fed91ac13c8">

3. **Locked State Check for Door Opening:**
   - Establish a state variable in the blueprint to indicate whether the door is in a locked state.
   - When the player interacts, check the door's locked state.
   - If the door is locked, maintain its current state and do not perform the opening operation.
     
<img width="1145" alt="61105a647be7e68267ce2d258e71353" src="https://github.com/maanqii/MscAdvancedProject/assets/119876408/25cf51bb-17f6-4f3a-852a-0aa6197f056d">

4. **Door Sound Response:**
   - Add audio components in the blueprint.
   - Trigger corresponding sound effects when the door is opened or closed.
   - Consider using audio triggers to play sounds when specific events occur.
     
<img width="1145" alt="a11c39f062700a821d2bb247e8c92f3" src="https://github.com/maanqii/MscAdvancedProject/assets/119876408/ab2c95a0-5c45-4090-a749-f138dbf22379">

5. **Modeling Details:**
   - Use 3D modeling tools to divide the door into two parts, rotating only the central portion.
   - Ensure the door's collision volume matches the trigger for correct interaction events.
   - Avoid unnecessary complexity and keep the model clear and simple.

### Menu Interaction Blueprint Design:

1. **Trigger for Obtaining Items and Information:**
   - Use triggers or interaction points to detect if the player has acquired new items or information.
   - Use blueprints to determine the type of obtained items or information and add them to the menu.
     
<img width="1144" alt="b135547d2132befe7f0868116826ec5" src="https://github.com/maanqii/MscAdvancedProject/assets/119876408/44c84cd0-06e0-4d81-8a93-bc2ea9ccf04b">
<img width="1146" alt="fa205625634dace25b34c23843b88f1" src="https://github.com/maanqii/MscAdvancedProject/assets/119876408/d5665fc3-353d-4c85-b61d-17c9de93a553">

2. **Sound and Text Prompts:**
   - Add audio components in the blueprint to trigger corresponding sound effects based on the type of obtained items or information.
   - Create a notification box in the lower-left corner of the screen to display text prompts for the acquired information.

3. **Opening the Menu:**
   - Design a key trigger or interaction point to allow players to open the menu.
   - When the menu is opened, display the collected items and information for easy reference.
     
<img width="1148" alt="d5f073cab5062f55e18d551e6ad2266" src="https://github.com/maanqii/MscAdvancedProject/assets/119876408/792006d6-7532-40e3-90fc-a8829cb70d2a">

4. **Item Rotation Detection:**
   - Add rotation detection functionality to items in the menu, allowing players to examine items more closely.
   - Use blueprints to control the rotation behavior of items, enhancing interactivity.

5. **Handling Objects in the Backpack:**
   - Design a backpack system to store items collected by the player.
   - Use blueprints to allow players to discard items from the backpack, ensuring proper item handling.
     
<img width="1153" alt="5ddf5c3c891460e59821fe6c6a0cae2" src="https://github.com/maanqii/MscAdvancedProject/assets/119876408/8555e659-a891-4219-8b06-81ea99e52254">
<img width="1148" alt="74ef68a31ce3cde01e5cb0f0f535c7f" src="https://github.com/maanqii/MscAdvancedProject/assets/119876408/0e989c30-f11e-478c-82e5-a7acc0abbf38">    
<img width="1148" alt="170af82659b820c7bda9230040b80da" src="https://github.com/maanqii/MscAdvancedProject/assets/119876408/515c3183-1353-4622-97e7-09a347ffd128">

6. **Save Functionality:**
   - Add a save button in the main menu, allowing players to manually save their progress.
   - Design save logic using blueprints to preserve the current game state.

7. **Association between Items and Catalogs:**
   - Establish associations between items and catalogs in the menu.
   - When a player clicks on an item, the menu automatically navigates to the corresponding catalog.
     
<img width="1148" alt="fcf85aa012a755a4c075feb68cc2d6c" src="https://github.com/maanqii/MscAdvancedProject/assets/119876408/57fbbdf1-8d14-45b2-8fe4-a2b1b0651d1d">

8. **Secondary Verification and Physics Engine for Keys:**
   - Implement secondary verification for keys through blueprints, ensuring that only genuine keys can be used.
   - Retain the physics engine for keys to make their behavior more realistic in the game.
   
<img width="1149" alt="f72831b7affb6ed06f31af97cd01334" src="https://github.com/maanqii/MscAdvancedProject/assets/119876408/3d081271-8883-49ea-a335-38e2e1532c2d">
<img width="1151" alt="bf6673078673f6a8b08ddb59148b44f" src="https://github.com/maanqii/MscAdvancedProject/assets/119876408/cfd882b2-a861-48bb-b82c-32d4a9933efe">

9. **Check Time and Loop:**
   - Set a time interval and loop mechanism to check the authenticity status of keys.
   - If a genuine key is detected, allow its use.

10. **Visibility Handling for Uncollected Items:**
    - In the main scene, use blueprints to ensure the visibility of uncollected items.
    - Ensure that uncollected items exist in the scene but do not impact the player's gaming experience.
      
<img width="1148" alt="e18110318f1637423b8f3adc3382b7f" src="https://github.com/maanqii/MscAdvancedProject/assets/119876408/80e4597e-6850-411d-b4de-19649b5fea9c">

### Letter Blueprint:

1. **Automatic Translation of Letters:**
   - Add automatic translation functionality to the blueprint, allowing the text on the letter to be automatically translated into the language used by the player.
   - Utilize the built-in translation services of the engine or implement custom translation logic.
     
<img width="1150" alt="ba3541b0a3d7a13868e0e248a5a5ffc" src="https://github.com/maanqii/MscAdvancedProject/assets/119876408/a14449b7-1dd8-4b35-973b-43af19175077">

2. **Handling After Reading:**
   - Design an interaction mechanism for reading the content of the letter.
   - Add a "read" state to the blueprint to facilitate subsequent processing.
     
<img width="1148" alt="7b2ab102a81f4ea5fd2122725774fc1" src="https://github.com/maanqii/MscAdvancedProject/assets/119876408/48ec3e47-1036-4ad3-8805-9253c9c7af02">

3. **Automatic Logging of Information into a Journal:**
   - Set up a journal directory in the blueprint, ensuring that letters that have been read are automatically recorded in the journal list.
   - Update the journal directory to allow players to view the content of letters they have read at any time.
     
   <img width="1150" alt="73acef15fc070a5d983972d1bf623ba" src="https://github.com/maanqii/MscAdvancedProject/assets/119876408/1f501bad-ba61-4cbf-b403-2c4583af5cb4">

### Player Blueprint Design:

1. **First-Person Exploration:**
   - Set the camera perspective to first-person, allowing players to explore the game world through their own viewpoint.

2. **Detailed Clothing:**
   - Add detailed clothing to the blueprint, allowing players to see their own attire in the game.
   - Utilize techniques such as skeletal animation to ensure that clothing naturally follows the player's movements when looking up or down.

3. **Enhanced Player Presence:**
   - Use animation blueprints and skeletal animations to achieve smooth transitions when the player looks up, looks down, etc., enhancing the player's presence and immersion.

<img width="887" alt="b21a40cc4acf6f4204488710f498676" src="https://github.com/maanqii/MscAdvancedProject/assets/119876408/67be06d1-cce9-4de4-92f5-975d1fa1264d">

4. **Blueprint-Based Controls:**
   - All protagonist actions, including jumping, sprinting, normal walking, etc., are designed based on blueprints.
   - Use blueprint scripts to handle player input and trigger corresponding actions.

<img width="1154" alt="d09561157e26dcf47d57efa607f82c6" src="https://github.com/maanqii/MscAdvancedProject/assets/119876408/18fead7e-3090-4169-b7d8-c57f1daad927">

5. **Action Coordination:**
   - Coordinate with appropriate action animations to ensure that the player's movements in the game appear natural, smooth, and adhere to real-world physics.

6. **Jumping and Sprinting:**
   - Design the logic for jumping and sprinting in the blueprint, ensuring that these actions trigger correctly in the game and have appropriate animation effects.

<img width="1154" alt="d07acb65723c7ddd3f62e1e6ff91563" src="https://github.com/maanqii/MscAdvancedProject/assets/119876408/717ac575-a587-4faf-8e37-8e10fa7d9d65">

7. **Normal Walking and Mouse-Movement-Based Camera Follow:**
   - Design the logic for normal walking, allowing players to control character movement via the keyboard.
   - Handle mouse movement in the blueprint, enabling the camera to follow the mouse's movement, providing a more freely controlled experience.

### Bottle Blueprint:

1. **Interaction with Regular Bottles:**
   - Use triggers to detect if the player interacts with the bottle.
   - In the blueprint, design an enlargement effect for the bottle for closer inspection.

<img width="1155" alt="37c146c8177debe8cde3686bba6305d" src="https://github.com/maanqii/MscAdvancedProject/assets/119876408/d1146dea-23f8-4e08-b92a-64401806409b">

2. **Bottle with Bottom Text Prompt:**
   - In the blueprint, add functionality for a bottom text prompt, ensuring that bottles with hidden text display the text when interacted with.

3. **Rolling Bottles to Discover Hidden Information:**
   - Design an interaction mechanism for rolling bottles, allowing players to freely roll them.
   - In the blueprint, determine the bottle's state; when the player discovers hidden information, trigger the corresponding effect.

<img width="1148" alt="df6a17294e8f1f76080df8a43400499" src="https://github.com/maanqii/MscAdvancedProject/assets/119876408/9abe5033-186d-49f8-b63b-cbbbbade6937">
<img width="1149" alt="543d69ee70d1ca474dee8e7eb21a62c" src="https://github.com/maanqii/MscAdvancedProject/assets/119876408/0c543afe-2660-45ea-9ba8-26258f1f8221">


4. **Disappearance of Hidden Information and Journal Directory Update:**
   - In the blueprint, set the display state for hidden information, making it disappear when discovered.
   - Update the journal directory, adding new information so that players can track the information they have found.

<img width="1151" alt="b70c4687407a1cf598710070e69a371" src="https://github.com/maanqii/MscAdvancedProject/assets/119876408/6cf142c0-2382-4664-b52c-002060020730">
