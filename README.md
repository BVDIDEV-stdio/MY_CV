## Contact me:
Email: vergon3.42x@gmail.com \
Phone no.: +7 (961) 653-83-23  \
GitHub: [github.com/BVDIDEV-stdio](https://github.com/BVDIDEV-stdio) *//you ar here though* 

## General:
### Education:
- "Software Engineering"; HSE University (Nizhny Novgorod Campus); bachelor degree(2020-2024) - graduated
- "Design", Program track "System Game Design"; HSE University (HSE Art and Design School); master degree - enrol. 2024

### Skills:
| Category              | Skill/Tool | Skill Level        | Description/Application Areas                                                                                       |
|:----------------------:|:----------------:|:---------------|-------------------------------------------------------------------------------------------------------------------|
| Programming Languages  | Java             | Core         | Basic Syntax, primary Data Structures and Algorythms                                                         |
|                        | C#               | Intermediate   | Unity development, OOP, implementing code logic modules and linking them                                    |
|                        | Python           | Core           | Basic Syntax and Scripts                                                                             |
| Engines                | Unity            | Intermediate   | Programming (UI, Game Mechanics, Programming Interfaces), Animation, Scene Buildup, Prototyping, ShaderGraph and MAterials|
|                        | Unreal Engine    | Core           | Blueprint, Level Prototyping and Buildup, Animation and Rigging, Shaders and materials                                    |
| 3D Artist              | Blender          | Intermediate   | Hard Surface Modeling, Organic Modeling, UV Layout, Texturing, Shader Graphs, Skinned Meshes, Rigs, Animation, Mesh Cleanup and Optimization|
| Languages              | English          | C1             | Advanced                                                                                                            |
| Game Design            |                  | Core           | Difficluty Progression Curves, Balancing, Feature Design  |

## Work Experiencs
### HSE University (NN Campus):** Unity Programming Tutor: 2024-2025 

In the first semester of 2024-2025 academic year I taught practical classes for students (Faculty of Informatics, Mathematics and Computer Science). My responsibilities included:
- Syllabus Development
- Leading Practical Sessions
- Designing Lab Assignments Guidelines
- Lab Assignment Review and Grading (grades are recorded in students' project issues; you can access them via my contributions and activity log)\
In the second semester I advised students working on Unity projects as part of their term paper.

## Портфолио
### Thesis Paper and Graduation Project
As my graduation project I developed Unity game prototype to showcase the skills I acquired over four years of study. The prototype features a scene that includes:
- **Player character** capable of running, jumping, attacking and performing combo attacks, as well as shooting a projectile as a secondary attack;
- **Enemy character** that can patrol its surroundings or rapidly approach the player to attack; (enemy behaviour reminds that of Holow Knight basic enemies)
- healing mechanics and healing items logic
The project was designed with a focus to minimize component dependencies, ensuring modularity and scalability. The approach allows for easy improvements and reworking certain mechanics without overhauling the entire game code.


<div>
  <img src="/thesis_scheme_1.png" width="400" alt="на этой пикче общая схема логики игрового персонажа"/>
  <img src="/thesis_scheme_2.png" width="400" alt="тут схема противника"/>
  <img src="/thesis_scheme_3.png" width="400" alt="тут схема работы UI"/>
</div>
<p><em>Diagrams for: player character components and their interaction; Enemy AI logic and composition; UI logic</em></p>


<div>
  <img src="/thes_blender_skeletal_anim.png" width="400" alt="тут перс в блендере создаётся"/>
</div>
<p><em>Models and animations were made from scratch to cover basic visual requirements. Visual fidelity was not a priority, of course</em></p>


<div>
  <img src="/thes_animtree_combo.png" alt="пикча с анимациями для комбо"/>
</div>
<p><em>Anim state machine, providing combo-attacks on consecutive button clicks</em></p>

<div>
  <img src="/thes_anim_states.png" alt="ещё пикча с анимационным state machine"/>
</div>
<p><em>Anim state machine featuring player character logic in general</em></p>
<div>
  <img src="/thes_ui_1.png" width="400" alt="UI 1"/>
  <img src="/thes_ui_2.png" width="400" alt="UI 2"/>
</div>
<p><em>Examples for basic UI</em></p>

YouTube: https://youtu.be/yQFOX5VP178
Github: https://github.com/BVDIDEV-stdio/THESIS_WORK

### A small Snippet Project - Unreal Engine
https://youtu.be/MTQOhWPwzuw
The snippet project feature modular character system as well as an animation rig enhanced with leg IK so they align on slopes and uneven surfaces.
### 3D art
<div>
  <img src="/SHOTGUN_STYLIZED.png" width="500"/>
  <img src="/SHOTGUN_STYLIZED_2.png" width="500"/>
</div>
<p><em>Stylized futuristic shotgun practice, old work</em></p>

<div>
  <img src="/mp_styl.png" width="300"/>
  <img src="/mp_styl_2.png" width="300"/>
</div>
<p><em>Stylized MP5 practice, old one too</em></p>

<div>
  <img src="/port_arm.png" width="240"/>
  <img src="/port_char.png" width="240"/>
</div>
<div>
  <img src="/port_char2.png" width="240"/>
  <img src="/port_char3.png" width="240"/>
</div>
<div>
  <img src="/port_char4.png" width="240"/>
</div>
<p><em>Minimalistic character practice</em></p>

<div>
  <img src="/study_columns.png" width="300"/>
  <img src="/study_spike_n_arc.png" width="300"/>
</div>
<p><em>Some of the models created as part of a team project (top-down stealth action) for my master's program</em></p>

<div>
  <img src="/sawd_off1.png" width="300"/>
  <img src="/sawd_off2.png" width="300"/>
</div>
<p><em>Stylized sawed-off shotgun for a pet project of mine</em></p>

### Pet project
https://github.com/BVDIDEV-stdio/ITSADAMNJOKE-repo
So far the project (prototype stage) includes:
- WASD movement
- **Jumping**: can provide a regular jumping as well as double-jumping via maxAirJumps that can be increased (e. g. by getting an ability item)
- **Dash**: DOOM Eternal style: quickly dodge attacks and access hard-to-reach areas. Player's gravity is set to 0 while dashing to provide easy platforming. Dodges do exhaust and recharge so the player can not spam this ability. Max consecutive dodges quantity is adjustable, too
- **Inventory and Item**: in-game **Item** class entities store refs to Scriptable Objects defining items' very basic properties: title, description, weight and so on. Items are pickable via raycast from player's Camera.transform.forward. **Inventory** class works with a list of **ItemParams** objects carrying the exact values of **Item**s picked in the world (thus destroyed). Inventory has its standard item list logic implemented (addition/removal) as well as UnityEvents, which on invokation call various methods (e. g. Inventory UI update).
//Also inventory component is designed to be "written once, attached everywhere" so both Player and non-playable entities could use its functions.
- **UI:** The project includes a **UIWindow** class that serves as a base for any window-based UI. It is user-adjustable in "TES3 Morrowind"-way: players can drag its edges and the upper right corner to resize and reposition the window as needed. **UIWindow** contains no additional logic and acts solely as a content platform - each content element should implement its own logic. For example, the **InventoryMenu** class uses **UIWindow** methods to display buttons and a scrollbar yet the logic for these controls is handled entirely within InventoryMenu.

Additionally, the project features a placeholder pause menu implemented using a menu stack approach.

- **UI: HUD for item info**: this HUD piece displays a card containing the briefest item info (name, pic, type in rarity color style). While the card is displayed, the item is indicated by a rectangular frame that fits the pixel boundaries of the item mesh.
**WIP: Weapon class : Item, EquipSystem and Projectiles**: currently I am working on weapons Raycast/projectile spawn and also have got working EquipSystem allowing to equip weapons in either hand as well as to wield a weapon in both hands by "switching the grip mode". My goal was to implement the equip system similar to those found in Soulsborne games, because:
  1. This is an ***utterly*** entertaining challenge
  2. With careful game design and weapon balancing (including grip variations, bonuses, and penalties) this system will provide a solid foundation for players to experiment with different builds.
  3. I feel eager to **experiment firsthand** to discover the potential of this kind of system in *first-person shooters*.


[*russian language version*](READMErus.md)
