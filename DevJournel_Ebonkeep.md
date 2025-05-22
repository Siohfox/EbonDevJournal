# Game Project (Project Ebonkeep)

Project Number: Group Project

Ross Bates

SID: 1911666

# Major Sources

- Game URL: TBD
- Github: https://github.com/SenDev2001/ProjectEbonkeep
- Gameplay video: TBD

# Project Outline
"The Battle of Ebonkeep" is an immersive third-person action game centered around stealth-based infiltration and intense boss combat. Players take on the role of a skilled assassin tasked with breaching the heavily fortified castle of Ebonkeep—a towering medieval fortress shrouded in darkness and mystery. As they journey deeper into its labyrinthine halls, players must navigate tight corridors, avoid detection, silently eliminate guards, and collect powerful upgrades scattered throughout the environment.

The ultimate goal is to reach the heart of the castle—the Keep—where a formidable final challenge awaits: a colossal, ancient golem known only as "The Fallen One." This massive boss creature serves as the final test of the player's skill, strategy, and resourcefulness. Victory is only achieved by surviving and defeating this fearsome enemy, marking the end of the infiltration and the completion of the mission.

Game features include:
- Stealth mechanic 
- Crossbow third person shooting and aiming
- Guards and NPC AI
- A huge boss fight with unique attacks
- Upgrades and power ups
- A large castle area to explore and admire
- High detail and cool effects

The project aims to deliver a compelling and memorable third-person experience that combines the thrill of sneaking through enemy territory with the intensity of a massive boss showdown. At its core, The Battle of Ebonkeep is about the tension, planning, and reward of a successful infiltration culminating in a climactic, high-stakes duel against a powerful foe.

My objective is to design and implement the boss enemy’s artificial intelligence within Unreal Engine 5, utilizing the engine's Behavior Tree and Blackboard systems to create a robust and dynamic AI. This system will allow the boss to perform a variety of autonomous actions, such as adapting to player behavior, executing complex attack patterns, transitioning between different combat phases, and reacting to environmental changes in real-time. The goal is to craft a challenging and engaging encounter that feels intelligent and responsive, enhancing the overall gameplay experience during the climactic boss battle.

My secondary objective is to help achieve a working and functioning game, including player movement, effects and 


### Research

#### Identified resources

As a group, we decided on doing a third person infiltration game focusing on a cool boss fight similar to researched games (Elden Ring, 2022), Dark Souls III (Dark Souls III, 2016) and Borderlands 3 (Borderlands 3 Game, 2019).
We decided this project would be focused for PC and Steam distribution and use, as it would portray the game the best. 

While I intended to try and make a fast paced game due to my experience with presenting games that had faster experiences generally did better in showcases, the team wanted to introduce a stealth mechanic to the gameplay which was also important to give some AI work to one of my other group team-mates, so I reluctantly agreed. While I still believe it might be better to have a fast rush and infiltrate game, it was okay to compromise and do a 50/50 on combat thrill and stealth game.

##### UE 5.4 Upsides:
For the engine, we agreed Unreal Engine 5.4 would work the best for us for three main reasons:
1. Fantastic visuals and working gameplay out-of-the-box to help speed up the game making process and create better visuals than most other engines at this time (2025)
2. UE 5.4 Is the most accessable engine, as it is installed on the workstations at the University we intend to work at, and have installed it on our home computers without errors, enabling
us to both work at home and away on this project.
3. Unreal's inbuilt animation tools and inbuilt AI programming makes making the core mechanics of the game faster and easier than it would be to create it from scratch on different engines.
(TechCrunch, Coldewey, 2022)

##### UE 5.4 Downsides:
The downsides to working in unreal include the unfortunate fact that a lot of the assets in Fab, Quixel and by the Unreal Engine developers are not free and easily accessable (anymore),
this means that most assets will have to be made by our small team, introducing a higher workload to compelte the project in a professional and reasonable time.

Another downside, is that installing a lot of the requirements for a C++ compatible Unreal project requires a lot of installed files, especially on windows computers, and as such, many problems
are caused in the initial installation and start up processes, with some people being unable to open the project for various reasons and the engine often complaining about needing to be rebuilt.
(Why Is Unreal Engine 5 Criticized, and Is It Really That Bad?, s.d.)

##### Other resources

For initial drafting, we made some quick sketches and found some reference images as to how it should look:

<img src="https://cdnb.artstation.com/p/assets/images/images/030/310/069/large/tobias-quintella-15-tobias-quintella-01.jpg?1600216345" alt="Ref Image Here" width="1000"/>
Figure 1`: A reference image we will loosely base the castle design around (Quintella, T. (no date) Tobias Quintella, Medieval castle design concept. Available at: https://tbquintella.artstation.com/ (Accessed: 16 February 2025). )

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
I used some videos on how to start creating games with Unreal Engine 5.4 such as Unreal Sensei's beginner tutorial (How to Create a Game in Unreal Engine 5 - UE5 Beginner Tutorial, 2023). Generally I found, most tutorials for Unreal Engine 5.* applied to almost all version of Unreal Engine 5, which was particularly useful. I also found that since Unreal 5 is a fairly recent development to Unreal, there was a lot of new and up to date learning material that applied to early development of the engine, which meant information I found about Unreal 5 was almost always up-to-date and realistic, making the learning experience surprisingly easy and pleasant. This did mean, however, that not a lot of material existed yet, so the stuff that did exist was fairly limited. In figure B below, I used this video to learn the basics of Unreal Engine 5 itself and create my first games using the engine. 

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

##### Software Failures

Throughout working as a team in the project, I experienced many issues with the softwares. Notably, we were held back by github not being able to store much in terms of objects. Since Unreal engine has very large files often, this was a problem for us. We set the project up as LFS, only to learn that it has a "Bandwidth" of 1Gb. This practically meant, with the way we first set it up, that only one person could download the project and make changes once before we hit the monthly quota.
This was undoubtably frustrating, and took us at least 2 weeks to get properly working before any of us could properly engage in the project.
So in other words:
Problem: LFS needed, github has a small amount
Solution: We had someone who was paying for the LFS set it up, and found a solution of dividing the project into Statics and Dynamics to help save space on both sides. This solution was not flawless, but it allowed the project to finally work on github, and satisfied the 3 months of work we needed to do.

Another issue we had was that Unreal 5.4 had many issues with loading C++ projects on various devices. It was difficult to figure out what exactly it wanted, and it kept saying "Cannot build source files, try rebuilding manually". In the end, we found a page (Unreal Engine 5: How To Recover Files "Could not compile. Try rebuilding from source manually.")


##### Creating the shooting
As the person in charge of creating the character with shooting mechanics, i decided to use a line trace to trace where the player would shoot.

In figure F and G, I used a raycast, or a Line trace as it's referred to in Unreal, to trace from the camera to the crosshair. I did this so the player could shoot at the crosshair, and it seemed like the simplest way for me, who has never programmed a shooting mechanic before. After seeing it the ray hit something or not, I would trace another line from the crossbow to the hit point of the crosshair linetrace. This resulted in a crossover point where the two lines meet, and would allow the bullets to come from the crossbow the player held, instead of the center of the screen.

![Initial Image](https://raw.githubusercontent.com/Siohfox/EbonDevJournal/refs/heads/main/Images/shooting1.png)
Figure F: A third person view of a shot made, showing the line trace from the crosshair to the hit point

![Initial Image](https://raw.githubusercontent.com/Siohfox/EbonDevJournal/refs/heads/main/Images/shooting2.png)
Figure G: An alternate view, to see the line trace from both the weapon and the camera, to decide which point the crossbow should shoot towards

##### Adding arrow stab

Since we're using a crossbow as our main form of attack, I decided to implement a feature where the arrows appear to stick into walls and targets.

![Initial Image](https://raw.githubusercontent.com/Siohfox/EbonDevJournal/refs/heads/main/Images/arrow_stab.png)
Figure H: An image showing arrows sticking into the wall after implementation.

I used animations from the Animation Starter Pack (Fab, s.d.), to create the animation blueprint for the character, allowing for a third person moving shooter.

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

![Initial Image](https://raw.githubusercontent.com/Siohfox/EbonDevJournal/refs/heads/main/Images/tree.jpg)
Figure I: A figure of the behaviour tree in Unreal used by the main Boss

A short video here demonstrates the unpolished initial concept boss fight, showcasing the AI working and some simple mechanics, using a placeholder boss.
[Watch the Boss fight video](https://github.com/Siohfox/EbonDevJournal/blob/main/Images/Firstbossfight%20TreeNoAudio.mp4)

#### Niagara VFX

As part of our group project, I took on the task of creating visual effects using Unreal Engine's Niagara system to enhance the game's feel. Being new to Niagara, I began by enabling the plugin in Unreal Engine 5.4 and exploring the basic interface. I found the official documentation particularly helpful, especially the Quick Start guide, which walked me through creating simple effects like smoke and sparks.

I ended up using niagara for a few parts of the project, namely the boss slam effects, arena particle effects, and a test fire particle which was not implemented in the end demo.

##### Shockwave
Using tutorials from SoftTofuVFX (UE5 Particle ShockWave Tutorial, 2023), I was able to create an awesome shockwave particle effect for the boss' slam attack.

![ShockwaveFx here](https://raw.githubusercontent.com/Siohfox/EbonDevJournal/refs/heads/main/Images/ShockwaveFX.jpg)
Figure J: A Niagara shockwave particle that I implemented following the method used by SoftTofuVFX (UE5 Particle ShockWave Tutorial, 2023)

An early example of the boss using the shockwave is below:
[Watch the Boss Shockwave Niagara video](https://github.com/Siohfox/EbonDevJournal/blob/main/Images/BossShockwaveNiagara.mp4)

##### Meteors

One of the bosses attacks involved hurling meteors from the sky. To make them more meteor like, i used references from UnrealCG's tutorial on Youtube (Create Stunning Fire Effects in Unreal Engine 5 with Niagara, 2023) to help create a static mesh wrap around for the meteors, making them look like they're on fire. Adding to that, I added some red particles to make it look like the meteors are flaming.

![FX here](https://raw.githubusercontent.com/Siohfox/EbonDevJournal/refs/heads/main/Images/MeteorNiagaraFX.gif)

Figure K: The final look of a meteor in the game made by myself, used by one of the bosses attacks when it is enraged (under half health)

##### Arena Ambience

For the arena, I felt it needed some ambience, so I added some basic fog particles employing some of Unreal's default Volumetric fog upon Niagara FX particles, which covered the whole arena. This created a look of fogginess to the arena, giving it some depth. Additionally, since the boss is vaguely firey, I added some hanging particles which look a bit like embers, to further enhance the look of the arena, which can be shown in the figures below.

![FX here](https://raw.githubusercontent.com/Siohfox/EbonDevJournal/refs/heads/main/Images/BeforeFogFX.png)
Figure L: An example of what the arena looked like before the particles

![FX here](https://raw.githubusercontent.com/Siohfox/EbonDevJournal/refs/heads/main/Images/AfterFogFX.png)
Figure M: An example of what the arena looked like after the particles


## Critical Reflection

### What did or did not work well and why?

Embarking on the development of Project Ebonkeep presented a series of challenges and learning opportunities. Transitioning from Unity to Unreal Engine 5.4 was initially difficult, especially given my limited experience with Unreal's architecture. However, the engine's robust documentation and community tutorials facilitated a smoother adaptation process.

One of the standout successes was the implementation of the AI Behavior Tree system. Leveraging Unreal's Behavior Trees allowed for modular and scalable AI behaviors, which were instrumental in creating dynamic enemy interactions. The use of Selectors and Sequences enabled the design of complex decision-making processes for NPCs, enhancing gameplay depth (Epic Games, 2025a).

Integrating the AI Perception system further enriched the AI's responsiveness. By configuring senses such as sight and hearing, NPCs could react more naturally to the player's actions, creating a more immersive experience (Epic Games, 2025b).

However, not all aspects proceeded smoothly. The initial setup of the AI systems was time-consuming, with challenges arising from understanding the intricacies of Behavior Trees and Perception components. Debugging AI behaviors required a lot of attention, as minor misconfigurations could lead to erratic NPC actions. Additionally, while the visual scripting through Blueprints was powerful, it occasionally became complex to manage, especially when dealing with extensive AI logic.

A very important reflection was that the movement system used was very janky, and is not something i'd recommend. We made the character move a bit like a Fortnite third person shooter character, and it just feels bad to use. If I had more time, i would love to introduce a proper movement system to the game.

I also want to critise my time management, and effort for the development journal. I was unable to include all of the parts I put into the project, as much of it was small tweaks and particle effects. 

### What would you do differently next time?

Reflecting on the development process, I can already find areas to improve. Firstly, time planning and casualty planning could have been much better, we found a lot of group changes happened which stunted the development of the project. In the future, i should be prepared for this and get work done faster to compensate. Early-stage prototypes could help identify potential pitfalls in AI behavior and system integration, allowing for timely adjustments.

I would love to use a better movement system, and allocate more time into the character, even if it wasn't my main goal.

## Bibliography

FromSoftware, Bandai Namco Entertainment (2016) Dark Souls III.

Gearbox Software, 2k (2019) Borderlands 3.

FromSoftware, Bandai Namco Entertainment (2022) Elden Ring.

Coldewey, D. (2022) Why should you care about Epic’s Unreal Engine 5? At: https://techcrunch.com/2022/04/11/what-is-epic-games-unreal-5/ (Accessed: 14 Feb 2025).

Why Is Unreal Engine 5 Criticized, and Is It Really That Bad? (s.d.) At: https://vgtimes.com/articles/121246-why-is-unreal-engine-5-criticized-and-is-it-really-that-bad.html (Accessed: 14 Feb 2025).

How to Create a Game in Unreal Engine 5 - UE5 Beginner Tutorial (2023) At: https://www.youtube.com/watch?v=1XjgLKrb4_M (Accessed: 15 Jan 2025).

Epic Games (2025a) Unreal Engine Behavior Tree Node Reference: Composites. Available at: [https://dev.epicgames.com/documentation/en-us/unreal-engine/unreal-engine-behavior-tree-node-reference-composites](https://dev.epicgames.com/documentation/en-us/unreal-engine/unreal-engine-behavior-tree-node-reference-composites) (Accessed: 24 Jan 2025).

Epic Games (2025b) Behavior Tree in Unreal Engine - Overview. Available at: [https://dev.epicgames.com/documentation/en-us/unreal-engine/behavior-tree-in-unreal-engine---overview](https://dev.epicgames.com/documentation/en-us/unreal-engine/behavior-tree-in-unreal-engine---overview) (Accessed: 25 Jan 2025).

Epic Games (2025c) Behavior Trees in Unreal Engine. Available at: [https://dev.epicgames.com/documentation/en-us/unreal-engine/behavior-trees-in-unreal-engine](https://dev.epicgames.com/documentation/en-us/unreal-engine/behavior-trees-in-unreal-engine) (Accessed: 30 Jan 2025).

Wadstein, M. (2016) WTF Is? AI: Simple Parallel Node in Unreal Engine 4 (UE4). Available at: [https://www.youtube.com/watch?v=idejwkR4Vcc](https://www.youtube.com/watch?v=idejwkR4Vcc) (Accessed: 4 Feb 2025).

Creating visual effects in Niagara: [https://dev.epicgames.com/documentation/en-us/unreal-engine/creating-visual-effects-in-niagara-for-unreal-engine](https://dev.epicgames.com/documentation/en-us/unreal-engine/creating-visual-effects-in-niagara-for-unreal-engine) (Accessed: 19 Feb 2025).

Pitchfork Academy (Youtube) How To Make A Third Person Shooter - Unreal Engine 5 Tutorial: [https://www.youtube.com/watch?v=-IM5IE_XiLI](https://www.youtube.com/watch?v=-IM5IE_XiLI) (Accessed: 6 Feb 2025).

Unreal Engine 5: How To Recover Files "Could not compile. Try rebuilding from source manually.":  https://dev.epicgames.com/community/learning/tutorials/RedB/unreal-engine-5-how-to-recover-files-could-not-compile-try-rebuilding-from-source-manually (Accessed: 20 Jan 2025).

Unreal Engine 5 - Official Valley of the Ancient Tech Showcase (IGN): [https://www.youtube.com/watch?v=SeY-ousiCPg](https://www.youtube.com/watch?v=SeY-ousiCPg)  (Accessed: 10 March 2025).

Create Stunning Fire Effects in Unreal Engine 5 with Niagara (UnrealCG): [https://www.youtube.com/watch?v=SeY-ousiCPg](https://www.youtube.com/watch?v=oaaBxBMUGvQ)  (Accessed: 12 March 2025).

Boss shockwave: Magical Shockwave in Unreal Engine Niagara | in 12 minutes (Motion Dreams Youtube): https://www.youtube.com/watch?v=ZAKTxE4VZ1U (Accessed:  20 Feb 2025).

Cool meteor landing particle effect: Ue5 Decal Material Tutorial | Magic circle | Downloadfiles (RainRainFX Youtube): [https://www.youtube.com/watch?v=wsKODsPr3CQ](https://www.youtube.com/watch?v=wsKODsPr3CQ) (Accessed:  29 Jan 2025).

UE5 Particle ShockWave Tutorial, SoftTofuVFX, Youtube (2023) At: [https://www.youtube.com/watch?v=3AJBfDuUEXc](https://www.youtube.com/watch?v=3AJBfDuUEXc) (Accessed:  19 Feb 2025).

Fab (s.d.) At: https://www.fab.com/listings/98ff449d-79db-4f54-9303-75486c4fb9d9 (Accessed:  1 Mar 2025).


## Declared Assets

Meteor hit noise: https://freesound.org/people/SuperSouper/sounds/684987/ (Accessed: 26 Feb 2025)
Impact circle: https://clipground.com/images/magic-circle-clipart-12.png (Accessed: 22 Feb 2025)
Crossbow shot sfx: https://freesound.org/people/Lunevix/sounds/246015/ (Accessed: 25 Feb 2025)
Crossbow model by wolkoed: https://sketchfab.com/3d-models/crossbow-29266724221344da8c37367f90959b81#download (Accessed: 12 Feb 2025)
Rocks and meteors (Rock Pack Vol 01 by Vampawn): https://www.fab.com/listings/f66023d1-7951-4c62-8ad5-121b4b0df349 (Accessed: 3 March 2025)

The following assets were assisted or edited by GPT 4o:
Development Journal
