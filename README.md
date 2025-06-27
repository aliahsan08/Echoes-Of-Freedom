README.md for Echoes of Freedom

Project Title:
Echoes of Freedom

Group Members 

1.Wasiq Amir 

2.Zayna Qasim 

3.Ali Ahsan 

4.Fatima Nisar

Project Description:

"Echoes of Freedom" is a text-based adventure game set in a captivating fantasy world. 
Players take on the role of a rebellious prisoner who escapes captivity to overthrow a tyrant ruler. 
Combining exploration, turn-based combat, and narrative-driven progression, this game offers players a thrilling experience filled with strategic challenges and meaningful decisions.

Features

Immersive Storytelling:
Engaging cutscenes and narrative choices that shape the player’s journey.
Deeply integrated lore with unique characters and encounters.

Strategic Combat:
Turn-based battles with options like attack, defend, recharge, and heal.
Dynamic boss fights with custom audio themes.

Exploration:
Navigate through intricate maps for each level.
Solve puzzles, interact with NPCs, and uncover secrets.

Level System:
Five levels, each with its own unique map, enemies, and challenges.
Gradual difficulty progression.

Player Progression:
Level-up mechanics with stat improvements.
XP gain based on performance and decisions.

Inventory Management:
Collect, use, and manage items like keys, potions, and special artifacts.

Audio and Visuals:
Dynamic background music and sound effects.
SFML-based fullscreen graphics for title and premise screens.


Technical Architecture

Core Components:

Character Management:
Character struct for player, enemies, and bosses with attributes like HP, SP, ATK, XP, and level.

Level Management:
Each level is represented by a 2D string array (mapX).
A global pointer array (maps) dynamically switches between levels.

Combat System:
Turn-based combat loop with enemy AI and randomized actions.

Inventory System:
2D array for item storage with fields for name, quantity, and description.

Audio Integration:
Background music and boss-specific soundtracks loaded using SFML.
Voice-over segments enhance storytelling.

Flowchart Overview:
Title Screen → Premise → Level Exploration → Battle or Interaction → Boss Fight → Cutscene → Next Level

Deploying and Running Echoes of Freedom

Download the Zip File:
Download the provided Echoes_of_Freedom.zip file and extract it to your desired directory.

Opening the .exe:
Open the executable file (.exe) and play the game. All the necessary components and libraries have already been integrated

Playing the Game:
Ensure your system volume is turned up for an immersive experience.
Follow the on-screen instructions to navigate the game.



Detailed Documentation

1. Game Initialization

Title Screen:
showTitleScreen(sf::Sound& titleSound): Displays the title screen with animations and audio.

Premise:
premise(sf::Sound& premiseSound): Narrates the backstory with synchronized typewriter text.

2. Levels
   
Structure:
Maps are stored as 2D string arrays, with obstacles (*), paths ( ), and interactive elements.

Progression:
Levels (level0 to level4) introduce new mechanics, puzzles, and story elements.

Key Functions:
levelX(): Handles gameplay logic for each level, including door interactions, puzzles, and battles.

3. Combat System
   
Mechanics:
Turn-based combat where players and enemies alternate actions.
Includes counter-attacks, vulnerabilities, and logical enemy behavior.

Key Functions:
battle(): Main combat loop.
attack(), defend(), recharge(), heal(): Define specific actions.
levelUpSystem(): Manages player leveling and stat improvements.

4. Inventory Management
   
Structure:
2D array (inventory) with fields for item name, quantity, and description.

Key Functions:
addItem(), removeItem(): Modify inventory based on events.
displayInventory(): Displays all collected items.

5. Boss Fights
    
Integration:
Each level concludes with a unique boss battle.
Bosses have distinct stats and custom soundtracks.

Key Functions:
bossBattle(): Manages boss encounters with level-specific logic.

6. Audio Integration

SFML Implementation:
Background music and event-specific audio enhance immersion.

Initialization:
initializeAudio(): Loads all required audio files.

7. Narrative Integration

Cutscenes:
Story-driven events with player choices affecting outcomes.

Key Functions:
cutscenes(): Displays cutscene text and handles player decisions.

Level-Specific Highlights

Level 0:
Escape from the prison by solving puzzles and fighting guards.
Collect a key and unlock the first door.

Level 1:
Introduces interactive portals and narrative-driven puzzles.

Level 2:
Encounter ghouls and discover the "Ghoul's Medal."
Choose whether to engage or help certain NPCs.

Level 3:
Solve a riddle using clues found in battles.

Level 4:
Face the King’s elite guard and decide your ultimate fate.
