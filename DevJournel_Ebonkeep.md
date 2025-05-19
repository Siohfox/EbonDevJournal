# Game Project (Project Ebonkeep)

Project Number: Group Project

Ross Bates

SID: 1911666

# Major Sources

- Game URL: TBD
- Github: https://github.com/SenDev2001/ProjectEbonkeep
- Gameplay video: TBD

# Introduction
"The Battle of Ebonkeep" is a third person infiltration and boss fighting game where the player must infiltrate a castle known as Ebonkeep, find upgrades and assassinate guards
before reaching the castle keep and fighting a giant golem boss named "steve (tbd)", they must survive against and defeat the boss to claim victory and win the game.

Game features include:
- Stealth mechanic 
- Crossbow third person shooting and aiming
- Guards and NPC ai
- A huge boss fight with unique attacks
- Upgrades and power ups
- A large castle area to explore and admire
- High detail and cool effects

### Research

#### Identified resources

As a group, we decided on doing a third person infiltration game focusing on a cool boss fight similar to researched games Elden Ring, Dark Souls and Borderlands.
We decided this project would be focused for PC and Steam distribution and use, as it would portray the game the best. 

While I intended to try and make a fast paced game due to my experience with presenting games that had faster experiences generally did better in showcases, the team wanted to introduce a stealth mechanic to the gameplay which was also important to give some AI work to one of my other group team-mates, so I reluctantly agreed. While I still believe it might be better to have a fast rush and infiltrate game, it was okay to compromise and do a 50/50 on combat thrill and stealth game.

##### UE 5.4 Upsides:
For the engine, we agreed Unreal Engine 5.4 would work the best for us for three main reasons:
1. Fantastic visuals and working gameplay out-of-the-box to help speed up the game making process and create better visuals than most other engines at this time (2025)
2. UE 5.4 Is the most accessable engine, as it is installed on the workstations at the University we intend to work at, and have installed it on our home computers without errors, enabling
us to both work at home and away on this project.
3. Unreal's inbuilt animation tools and inbuilt AI programming makes making the core mechanics of the game faster and easier than it would be to create it from scratch on different engines. 

##### UE 5.4 Downsides:
The downsides to working in unreal include the unfortunate fact that a lot of the assets in Fab, Quixel and by the Unreal Engine developers are not free and easily accessable (anymore),
this means that most assets will have to be made by our small team, introducing a higher workload to compelte the project in a professional and reasonable time.

Another downside, is that installing a lot of the requirements for a C++ compatible Unreal project requires a lot of installed files, especially on windows computers, and as such, many problems
are caused in the initial installation and start up processes, with some people being unable to open the project for various reasons and the engine often complaining about needing to be rebuilt.


##### Other resources

For initial drafting, we made some quick sketches and found some reference images as to how it should look:

<img src="https://cdnb.artstation.com/p/assets/images/images/030/310/069/large/tobias-quintella-15-tobias-quintella-01.jpg?1600216345" alt="Ref Image Here" width="1000"/>
Figure A: A reference image we will loosely base the castle design around (Quintella, T. (no date) Tobias Quintella, Medieval castle design concept. Available at: https://tbquintella.artstation.com/ (Accessed: 16 February 2025). )

##### Resource Gathering

The clear resources I need to identify and research were for my part of the group project are:

Major focus:
- Unreal's Behaviour Tree system and other AI related tools in Unreal Engine 5.4
- Unreal Engine 5 blueprinting
- Animation blueprints
- Any sort of existing boss fight creation
- Boss fights from other games, especially related games

Minor focus:
- Third person character control and design
- Niagara particles and FX
- Widget blueprints and UI

Since I have a lot to do to make the game function properly, I need to quickly research how to use Unreal Engine in general, as I am brand new to the software, and previously mostly used
Unity as my main engine for games programming.
This means I would need to learn the entirety of Unreal's basic UI, programming including possibly c++ classes (of which i have prior experience), and the various tools such as blackboards, behaviour trees, Widget UI, Animation blueprints, and possibly creating my own animations. 

### Sources

#### Unreal Basics
I used some videos on how to start creating games with Unreal Engine 5.4. Generally I found, most tutorials for Unreal Engine 5.* applied to almost all version of Unreal Engine 5, which was particularly useful. I also found that since Unreal 5 is a fairly recent development to Unreal, there was a lot of new and up to date learning material that applied to early development of the engine, which meant information I found about Unreal 5 was almost always up-to-date and realistic, making the learning experience surprisingly easy and pleasant. This did mean, however, that not a lot of material existed yet, so the stuff that did exist was fairly limited. In figure B below, I used this video to learn the basics of Unreal Engine 5 itself and create my first games using the engine. 

[![A video](https://img.youtube.com/vi/1XjgLKrb4_M/0.jpg)](https://www.youtube.com/watch?v=1XjgLKrb4_M)
Figure B: A video on the basics of creating a game in Unreal by Unreal Sensei, a Youtuber who creates guides for Unreal Engine. ((2023) YouTube. Available at: https://www.youtube.com/watch?v=1XjgLKrb4_M (Accessed: 01 January 2025). 

#### Creating a Boss Fight in Unreal Engine

After grasping the fundamentals of Unreal Engine 5, I delved into designing a boss fight to enhance my understanding of AI behavior and combat mechanics. I discovered a comprehensive tutorial series by Gorka Games that provided a step-by-step guide on crafting a boss encounter using Behavior Trees, AI Controllers, and Blueprint scripting. The series began with implementing the core AI logic and progressively introduced visual effects through Niagara and audio enhancements via MetaSounds, of which I chose to ignore and do in my own way.

This structured approach made the learning process both manageable and engaging. The tutorial also offered free project files and utilized Marketplace assets like the Ancient Golem, however I chose to use a basic model from mixamo for testing and animating, allowing me to focus on gameplay mechanics without the need to create assets from scratch. The clarity and pacing of the tutorials were particularly beneficial, especially when navigating complex systems like AI decision-making and environmental triggers.

[![A video](https://img.youtube.com/vi/z96BRmR7zXQ/0.jpg)](https://www.youtube.com/watch?v=z96BRmR7zXQ)
Figure C: A tutorial on creating a boss fight in Unreal Engine 5 by Gorka Games, covering AI behavior, visual effects, and sound design. ((2024) YouTube. Available at: https://www.youtube.com/watch?v=z96BRmR7zXQ (Accessed: 09 January 2025).

#### Third person shooter character

Although my job was to create a boss ai, it fell on me to create a third person character controller for the game, as no one else was able to do it, so I took it upon myself in order to have a complete and working game. I found a comprehensive tutorial by MizzoFrizzo (Figure D) that guided me through creating a third-person shooter using Blueprints. The tutorial covered essential aspects such as character movement, aiming, shooting mechanics, and animation blending. The step-by-step approach made complex concepts accessible, and the use of Blueprints allowed for visual scripting, which was particularly helpful for grasping the underlying logic without delving into C++ code. This hands-on experience significantly enhanced my ability to implement responsive and engaging player controls in a third-person perspective. While this was useful, I do not believe this will be the final design of the character movement, as it is a bit clanky and rough.

[![A video](https://img.youtube.com/vi/-IM5IE_XiLI/0.jpg)](https://www.youtube.com/watch?v=-IM5IE_XiLI)
Figure D: A tutorial on creating a third-person shooter character in Unreal Engine 5 by MizzoFrizzo, focusing on Blueprints-based implementation. ((2024) YouTube. Available at: https://www.youtube.com/watch?v=-IM5IE_XiLI (Accessed: 16 January 2025).

#### Comprehensive AI

After establishing a solid foundation in Unreal Engine 5, I sought to deepen my understanding of advanced AI systems, particularly focusing on the engine's built-in perception capabilities such as sight and hearing. I discovered a detailed tutorial by Ryan Laley that delves into the AI Perception system, illustrating how to implement sight and hearing senses within AI characters. The tutorial provides a step-by-step guide on configuring AI to detect players through visual and auditory stimuli, utilizing Behavior Trees and Blueprints to create responsive and dynamic AI behavior. This resource was instrumental in enhancing my comprehension of AI perception mechanics, enabling me to develop more immersive and intelligent AI interactions in my projects.

[![A video](https://img.youtube.com/vi/OytuX_swh8M/0.jpg)](https://www.youtube.com/watch?v=OytuX_swh8M)
Figure E: A tutorial on implementing AI perception using sight and hearing in Unreal Engine 5 by Ryan Laley, focusing on Behavior Trees and Blueprints. ((2022) YouTube. Available at: https://www.youtube.com/watch?v=OytuX_swh8M (Accessed: 08 May 2025).

#### Other Similar Games (infiltration Boss Fighting)

In developing Ebonkeep, a third-person infiltration and boss-fighting game set within a formidable castle, we drew inspiration from several titles renowned for their intricate level design, stealth mechanics, and challenging boss encounters. These games not only influenced the thematic and gameplay elements of Ebonkeep but also provided valuable insights into creating a compelling player experience.

Styx: Shards of Darkness, a stealth game developed by Cyanide Studio and published by Focus Home Interactive. Released on March 14, 2017, the game emphasizes infiltration, vertical navigation, and the use of stealth abilities to overcome enemies within complex environments . The game's setting within a fortress and encounters with formidable adversaries align closely with the stealth and boss-fighting aspects envisioned for Ebonkeep.

Assassin’s Creed Shadows: This installment revitalizes the franchise's stealth mechanics, emphasizing strategic infiltration and assassination within expansive, guarded castles. Players navigate complex environments, utilizing tools and allies to execute precise attacks, reminiscent of the calculated approach I envision for Ebonkeep's infiltration sequences.

Elden Ring
FromSoftware's Elden Ring offers an expansive open world filled with formidable enemies and intricate lore. The game's emphasis on exploration, environmental storytelling, and challenging boss battles inspired Ebonkeep's design of its vast castle environment and the climactic golem boss encounter. The seamless integration of exploration and combat in Elden Ring serves as a benchmark for creating an engaging player journey.

Dark Souls
The Dark Souls series is renowned for its interconnected world design and punishing yet rewarding combat system. Its approach to level design, where areas are intricately linked and exploration is encouraged, influenced Ebonkeep's castle layout, promoting a sense of discovery and strategic navigation. The deliberate combat mechanics in Dark Souls also informed the design of enemy encounters in Ebonkeep.

By analyzing these titles, I was able to identify key elements that contribute to engaging combat experiences. Incorporating aspects such as strategic infiltration, diverse combat mechanics, and immersive world-building has been instrumental in shaping the gameplay and narrative of Ebonkeep, ensuring it offers a rich and captivating experience for players.

## Implementation

### Design

#### Gameplay Loop

The core gameplay loop of Ebonkeep revolves around a mixture of stealth, exploration, and high-stakes combat. The loop is designed to gradually increase in intensity as the player progresses through the castle grounds.

1. Infiltration Phase – Players begin outside the castle and must avoid detection by patrolling guards, using stealth and cover to sneak through courtyards and halls. They can eliminate enemies silently or avoid them entirely.

2. Exploration and Upgrades – As players navigate the environment, they are encouraged to explore alternate paths and hidden rooms to discover upgrades such as increased crossbow damage, speed boosts, or health regeneration items.

3. Combat Encounters – As the difficulty ramps up, players engage in more frequent combat situations where stealth is no longer a viable option. The player must use their upgraded abilities to defeat tougher enemies.

4. Boss Fight – The final stage of the loop culminates in a challenging boss fight against a massive golem named Steve (name still TBD). This battle tests all of the player’s skills, from dodging and timing to weapon use and spatial awareness.

5. Victory and Reflection – Upon defeating the boss, the game ends with a short cinematic and victory screen, rewarding players for their journey and effort.

This loop creates a satisfying balance of tension and release, gradually increasing stakes while giving players opportunities to prepare and adapt.

#### Code and Blueprint Naming Conventions and Design

To maintain clarity and consistency across the development team, we adopted conventions based on Allar's UE5 Style Guide. This helped ensure that all Blueprints, variables, and assets were readable and easily traceable by any team member.

Key naming standards included:

- BP_ prefix for all Blueprints (e.g., BP_Guard, BP_BossGolem)

- FX_ for Niagara systems (FX_Explosion, FX_Smoke)

- UI_ for interface elements (UI_HealthBar, UI_MainMenu)

- SM_ / SK_ for static and skeletal meshes (e.g., SM_CastleWall, SK_Golem)

- CamelCase for variables (PlayerHealth, AttackCooldown)

- VerbNoun format for functions (UpdateHealthBar, TriggerAlarm)

Using these conventions improved readability, eased debugging, and made it easier for new team members to understand and work with the project files.
ref: https://github.com/Allar/ue5-style-guide

#### Creating game

##### Initial implementation
Initially, we started with a basic third-person template provided by Unreal Engine 5.4. The goal was to rapidly prototype the core mechanics: player movement, crossbow shooting, and basic enemy detection.

We incrementally built in features such as:

1. A simple stealth system using trigger volumes and AI sight perception

2. Guard AI patrol paths using spline-based movement

3. Crossbow weapon functionality using line traces and damage values

4. Placeholder power-ups to represent future upgrade mechanics

The early versions were very unfinished, but served as a strong testbed to iterate on gameplay mechanics and gauge how sneaking around and combat would mesh.
Feedback

After internal testing and feedback from peers and mentors, we received several useful critiques:

- Stealth Mechanics were too simplistic. Guards didn’t have dynamic responses and behaved predictably, making it too easy to bypass them.

- Player Movement felt stiff and lacked polish, especially when transitioning between aiming and movement.

- Visual Feedback was unclear — hits didn’t feel impactful, and it was hard to read enemy behaviors.

Based on this, we prioritized improving AI responsiveness, added visual effects for shooting and stealth detection, and refined the animation transitions for smoother controls. The feedback loop was vital in shaping a more cohesive and engaging experience.

##### Creating the shooting
As the person in charge of creating the character with shooting mechanics, i decided to use a line trace to trace where the player would shoot.

In figure F and G, I used a raycast, or a Line trace as it's referred to in Unreal, to trace from the camera to the crosshair. I did this so the player could shoot at the crosshair, and it seemed like the simplest way for me, who has never programmed a shooting mechanic before. After seeing it the ray hit something or not, I would trace another line from the crossbow to the hit point of the crosshair linetrace. This resulted in a crossover point where the two lines meet, and would allow the bullets to come from the crossbow the player held, instead of the center of the screen.

![Initial Image](https://raw.githubusercontent.com/Siohfox/EbonDevJournal/refs/heads/main/Images/shooting1.png?token=GHSAT0AAAAAADEFH2XWDNUACYWD2T6JLALW2BLR32A)
Figure F: A third person view of a shot made, showing the line trace from the crosshair to the hit point

![Initial Image](https://raw.githubusercontent.com/Siohfox/EbonDevJournal/refs/heads/main/Images/shooting2.png?token=GHSAT0AAAAAADEFH2XX3RATILR7RJZCPDX62BLS6TA)
Figure G: An alternate view, to see the line trace from both the weapon and the camera, to decide which point the crossbow should shoot towards

##### Adding arrow stab

Since we're using a crossbow as our main form of attack, I decided to implement a feature where the arrows appear to stick into walls and targets.

![Initial Image](https://raw.githubusercontent.com/Siohfox/EbonDevJournal/refs/heads/main/Images/arrow_stab.png?token=GHSAT0AAAAAADEFH2XWVLAQ3M32W4RF25J62BLT5PQ)
Figure H: An image showing arrows sticking into the wall after implementation.


##### Feedback

After internal testing and feedback from peers and mentors, we received useful critiques:

Feedback 1:
"The aiming for the crossbow sights was bad and didn't improve much"
- anonymous tester
Response:
We attempted to adjust it so you could aim down the sight more and made it easier to move. It still doesn't feel perfect.

Feedback 2:
"There's not much feedback for being hit or hitting an enemy"
- anonymous tester
Response:
We intend to implement a flashing red enemy mechanic, or introduce a stagger animation, but we likely do not have enough time.

Feedback 3:
"The movement feels unfun"
- anonymous tester
Response:
We need to add better movement, if we have time.

Feedback 4:
"The crosshair and UI looks bad and covers the screen"
- anonymous tester
Response:
We updated the crosshair to look visually better, and created some borders for the UI elements such as the health bars, adding a name for the boss too.




#### AI design

Creating the boss AI was a complex but rewarding part, and was my main part. The boss, later named as The Fallen One, was designed to feel like a powerful and intimidating presence within the castle keep. Initially designed to be 12 times the player height, we ended up sticking to that and keeping it large and intimidating.



I used a blackboard and behaviour tree to simulate the AI behaviour of the boss.
To create the boss I used 3 separate classes:
1. I used a normal blueprint **"BP_Boss"** to include the boss model, health, and other important mechanics.
2. I used an AI class, a blueprint class derived from an AI actor built into unreal, and named it **BP_AI_Boss**. Since BP_Boss was a child of the character class, it allowed me to add an AI Controller class such as this one under the pawn dropdown in the details panel. This is what would "Control" the boss.
3. The final part was the **Blackboard** and **Behaviour Tree**, which I named, which i've bundled into one for clarity's sake. The blackboard was created as BB_Boss, and contained important stats, such as a linked health amount with the BP_Boss, and some other useful booleans that the blackboard could track such as testing whether it was dead, if the blackboard itself is enabled, and if it is seeing any target- however for this game sight was not necessary as it is implied the boss can always see the player. The BT_Boss behaviour tree was used to decide what action the boss should take next by checking the blackboard and using what Unreal calls "Sequences"

##### Research into Unreal's Behaviour Tree system 

As I embarked on developing AI for our game, Ebonkeep, I delved into Unreal Engine's Behaviour Tree system to structure complex decision-making processes for non-player characters (NPCs). This system allows for modular and hierarchical AI behavior design, which was essential for implementing both stealthy guards and the dynamic boss character.

In my exploration, I focused on understanding the core components of Behaviour Trees: Selectors, Sequences, and Simple Parallel nodes.

1. Selectors: These nodes evaluate their child nodes from left to right and execute the first one that succeeds. If a child node fails, the Selector moves on to the next. This structure is ideal for fallback behaviors. For instance, if a guard loses sight of the player, the AI can switch from a chase behavior to a search routine (Epic Games, 2025a).

2. Sequences: Sequence nodes execute their child nodes in order, proceeding only if each child succeeds. If any child fails, the entire sequence fails. This is useful for chaining dependent actions, such as a boss character preparing an attack, executing it, and then returning to an idle state (Epic Games, 2025a).

3. Simple Parallel: This node allows for concurrent execution of a main task and a background task. For example, while a boss character charges a powerful attack (main task), it can simultaneously track the player's position (background task). This structure is particularly useful for creating more lifelike and responsive AI behaviors (Epic Games, 2025b).

To deepen my understanding, I consulted Unreal Engine's official documentation, which provided comprehensive guides and examples on implementing these nodes effectively (Epic Games, 2025c). Additionally, I found video tutorials, such as the one by Mathew Wadstein on Simple Parallel nodes, to be helpful in these concepts, although the tutorial was in Unreal 4 back in 2016 9 years ago from now, it was still helpful and translatable to modern systems that Unreal still uses. (Wadstein, 2016).

Through this research, I was able to construct AI behaviors that are both modular and scalable, enhancing the gameplay experience by providing challenging and intelligent adversaries.

![Initial Image](https://raw.githubusercontent.com/Siohfox/EbonDevJournal/refs/heads/main/Images/tree.jpg?token=GHSAT0AAAAAADEFH2XXJ4VOMRT5G5BULBOY2BLQ3HA)

## Critical Reflection

### What did or did not work well and why?

Words

### What would you do differently next time?

Words

## Bibliography

Epic Games (2025a) Unreal Engine Behavior Tree Node Reference: Composites. Available at: [https://dev.epicgames.com/documentation/en-us/unreal-engine/unreal-engine-behavior-tree-node-reference-composites](https://dev.epicgames.com/documentation/en-us/unreal-engine/unreal-engine-behavior-tree-node-reference-composites) (Accessed: 24 Jan 2025).

Epic Games (2025b) Behavior Tree in Unreal Engine - Overview. Available at: [https://dev.epicgames.com/documentation/en-us/unreal-engine/behavior-tree-in-unreal-engine---overview](https://dev.epicgames.com/documentation/en-us/unreal-engine/behavior-tree-in-unreal-engine---overview) (Accessed: 25 Jan 2025).

Epic Games (2025c) Behavior Trees in Unreal Engine. Available at: [https://dev.epicgames.com/documentation/en-us/unreal-engine/behavior-trees-in-unreal-engine](https://dev.epicgames.com/documentation/en-us/unreal-engine/behavior-trees-in-unreal-engine) (Accessed: 30 Jan 2025).

Wadstein, M. (2016) WTF Is? AI: Simple Parallel Node in Unreal Engine 4 (UE4). Available at: [https://www.youtube.com/watch?v=idejwkR4Vcc](https://www.youtube.com/watch?v=idejwkR4Vcc) (Accessed: 4 Feb 2025).

## Declared Assets

Assets here

The following assets were modified with the use of GPT 4o:

