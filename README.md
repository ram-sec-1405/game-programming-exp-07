# game-programming-exp-07

## NAME:RAMPRASATH
## REG NO:212223220086
## AIM:
To implement an AI character in Unreal Engine that roams randomly within a defined area using
Behavior Trees and Navigation Mesh.
## PROCEDURE:
1. Navigation Setup
Add a NavMeshBoundsVolume to your level and scale it to cover the roamable area.
Ensure navigation is built (press P to visualize the navmesh).
2. Create AI Character
Create a new Character or Pawn Blueprint (e.g., BP_AICharacter ).
Add an AIController Blueprint (e.g., BP_AIController ) and assign it to your AI character.
3. Set Up Behavior Tree
Create a Behavior Tree (e.g., BT_RandomRoam ) and a corresponding Blackboard .
Add a Blackboard Key (e.g., TargetLocation ) of type Vector.
4. Implement Roaming Logic
In the Behavior Tree, use the following structure:
Root ➝ Selector
Sequence
Find Random Location (custom task to set TargetLocation )
Move To node (uses TargetLocation )
Create a custom BTTask Blueprint for finding a random location
using UNavigationSystemV1::GetRandomPointInNavigableRadius .
5. Place and Test
Place your AI character in the level.
Assign the AI Controller and Behavior Tree.
Play the scene and observe the AI roaming randomly.
AI Random Roam - Unreal Engine

## Output:
![image](https://github.com/user-attachments/assets/dbe69142-8809-43bf-82a9-97f8431767ec)
![image](https://github.com/user-attachments/assets/9f82af00-1875-4523-977d-2efad19faa21)
![image](https://github.com/user-attachments/assets/08a9a185-1d09-4a02-b02f-efe4d4bc053c)
![image](https://github.com/user-attachments/assets/7baa5be3-ce1d-45fd-946c-1ac9b086bcdc)
![image](https://github.com/user-attachments/assets/ad9532af-d757-41ac-ab39-b7996d34c83a)





## Result:
The AI character successfully roams within the defined NavMesh area, choosing random
destinations at intervals using the Behavior Tree logic.
