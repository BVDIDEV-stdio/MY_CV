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
/
/
/

## Контакты:
Email: vergon3.42x@gmail.com \
Phone no.: +7 (961) 653-83-23  \
GitHub: [github.com/BVDIDEV-stdio](https://github.com/BVDIDEV-stdio) *//но Вы и так здесь* 

## Общая информация:
### Образование:
- "Программная инженерия"; НИУ ВШЭ (Нижегородский филиал); бакалавриат - окончено (2020-2024)
- "Дизайн", профиль "Системный гейм-дизайн"; НИУ ВШЭ (Школа Дизайна НИУ ВШЭ); магистратура - учусь (enrol. 2024)

### Навыки:
| Категория              | Навык/Инструмент | Уровень        | Описание/Области применения                                                                                                      |
|:----------------------:|:----------------:|:---------------|----------------------------------------------------------------------------------------------------------------------------------|
| Языки программирования | Java             | Базовый        | Основы синтаксиса, базовые алгоритмы и структуры данных                                                                          |
|                        | C#               | Intermediate   | Разработка на Unity, ООП, написание интерфейсов и логики                                                                         |
|                        | Python           | Базовый        | Основы синтаксиса, простые скрипты                                                                                               |
| Движки                 | Unity            | Intermediate   | Программирование (интерфейсы, логика), анимация, сборка сцен, прототипирование, ShaderGraph, материалы                           |
|                        | Unreal Engine    | Базовый        | Blueprint, сборка уровней и прототипов, анимация/риггинг, шейдеры                                                                |
| 3D-моделинг            | Blender          | Intermediate   | Hard surface и organic моделинг, UV-развёртки, текстурирование, Shader-графы, skinned-меши, риггинг, анимация, оптимизация мешей |
| Иностранные языки      | Английский       | C1             | Advanced                                                                                                                         |

## Опыт работы
### НИУ ВШЭ НН:** преподаватель (Unity-программирование): 2024-2025 

В первом семестре 2024-2025 уч. года вёл практические занятия для студентов (*НИУ ВШЭ НН; факультет КНТ; 2 курс*). В мои обязанности входило:
- Составление плана курса
- Ведение практических семинаров
- Составление требований для лабораторных работ
- Проверка лабораторных работ (в районе декабря у меня в активити есть контрибы - надеюсь, их видно - там в Issues проектов выставлены оценки за лабы)\
Во втором семестре я консультировал тех студентов, у которых курсовые работы подразумевали выполнение Unity-проектов.

## Портфолио
### Дипломная работа - Unity-проект
В качестве ВКР я решил сделать прототип игры на Unity, в котором я мог бы продемонстрировать навыки, полученные за 4 года обучения. Этот прототип представляет из себя сцену, в которой есть:
- персонаж игрока, который может бегать, прыгать, атаковать с проведением комбо, а также "кастовать файрбол" в качестве secondary-атаки;
- персонаж противника с простой логикой, способный патрулировать местность или бегать к игроку, чтобы атаковать; (похож по поведению на обычного противника из Holow Knight)
- логика лечения посредством хилящих предметов в игровом мире
Проект создавался с упором на уменьшение взаимозависимости компонентов, модульность и облегчение масштабирования в будущем, дабы в него было достаточно просто вносить улучшения и перерабатывать механики, не "перелопачивая" весь остальной код игры.


<div>
  <img src="/thesis_scheme_1.png" width="400" alt="на этой пикче общая схема логики игрового персонажа"/>
  <img src="/thesis_scheme_2.png" width="400" alt="тут схема противника"/>
  <img src="/thesis_scheme_3.png" width="400" alt="тут схема работы UI"/>
</div>
<p><em>Схема работы логики персонажа и взаимодействия компонентов, из которых он состоит; схема логики противника; схема работы UI</em></p>


<div>
  <img src="/thes_blender_skeletal_anim.png" width="400" alt="тут перс в блендере создаётся"/>
</div>
<p><em>Модели и анимации были сделаны с нуля. Они не претендуют на визуальную изящность, т. к. диплом был сфокусирован на качестве кода</em></p>


<div>
  <img src="/thes_animtree_combo.png" alt="пикча с анимациями для комбо"/>
</div>
<p><em>Анимационный state machine, реализующий комбо-атаки при быстрых нажатиях кнопки атаки</em></p>

<div>
  <img src="/thes_anim_states.png" alt="ещё пикча с анимационным state machine"/>
</div>
<p><em>Анимационный state machine с логикой перехода анимаций у персонажа</em></p>
<div>
  <img src="/thes_ui_1.png" width="400" alt="UI 1"/>
  <img src="/thes_ui_2.png" width="400" alt="UI 2"/>
</div>
<p><em>Простой юай</em></p>

YouTube: https://youtu.be/yQFOX5VP178
Github: https://github.com/BVDIDEV-stdio/THESIS_WORK

### Небольшой тренировочный проект - Unreal Engine
https://youtu.be/MTQOhWPwzuw
Этот миниатюрный сниппет-проект включает в себя систему модульных персонажей, а также анимационный риг с инверсной кинематикой ног для "align-а" с наклонными и неровными поверхностями.
### Моделинг
<div>
  <img src="/SHOTGUN_STYLIZED.png" width="500"/>
  <img src="/SHOTGUN_STYLIZED_2.png" width="500"/>
</div>
<p><em>Стилизованный футуристический дробовик, старая работа</em></p>

<div>
  <img src="/mp_styl.png" width="300"/>
  <img src="/mp_styl_2.png" width="300"/>
</div>
<p><em>Стилизованный MP5, тоже старая работа</em></p>

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
<p><em>Минималистичный персонаж, модель для тренировки</em></p>

<div>
  <img src="/study_columns.png" width="300"/>
  <img src="/study_spike_n_arc.png" width="300"/>
</div>
<p><em>Некоторые из моделей, сделанных в командном проекте для магистратуры</em></p>

<div>
  <img src="/sawd_off1.png" width="300"/>
  <img src="/sawd_off2.png" width="300"/>
</div>
<p><em>Стилизованный дробовик-"обрез" для пет-проекта</em></p>

### Пет-проект
https://github.com/BVDIDEV-stdio/ITSADAMNJOKE-repo
В данном пет-проекте пока что есть:
- Возможность двигаться на WASD
- **Прыжок**: он устроен так, что в логике прыжка есть переменная maxAirJumps - при её увеличении у игрока будет возможность делать прыжок в воздухе (или несколько, если переменная > 1). Таким образом можно реализовать достаточно простой "подбор абилки", которая даст игроку способность к дабл-джампу.
- **Рывок (Dash)**: вспомните DOOM Eternal: там можно при помощи рывков уворачиваться от разного рода атак. Так и здесь - рывки позволяют короткое время двигаться с большой скоростью, расходуются и перезаряжаются, дабы ими нельзя было спамить. Во время рывка игрок всегда движется только горизонтально - скорость и ускорение свободного падения в этот момент у него нулевые. Также можно (как и в случае с прыжками) настраивать максимальное число рывков подряд: опять же, вспомните DOOM Eternal - там такое число равно двум, и по израсходовании такого числа рывков игрок ждёт кулдауна хотя бы одного из них.
- **Предметы и инвентарь**: для внутриигровых предметов есть класс Item и некоторые ScriptableObject-ы, на основе которых у предметов определяются самые базовые характеристики: название, описание, вес в инвентаре, редкость и т. д. Предметы при инициализации получают guid для их однозначной идентификации (может быть необходимо, когда, например, в инвентаре есть два почти идентичных предмета, но с разной редкостью). Предметы можно подбирать (механика подбора зиждется на Raycast-е от камеры игрока). Inventory хранит в себе список ItemParams-сущностей на основе "подобранных" Item-сущностей и располагает набором методов для изменения информации об этом списке (всё стандартно - добавление/удаление). Также эти методы Invok-ают UnityEvent-ы, на которые подписаны методы UI для инвентаря.
//Сам инвентарь сделан так, чтобы добавить его как компонент можно было не только к игроку, но и, например, к врагу.
- **UI**: для окон пользовательского интерфейса есть класс UIWindow - это окно, которое можно перетаскивать по экрану и расширять/уменьшать (почти так же, как в TES 3: Morrowind). UIWindow больше не содержит логики, и её нужно добавлять через контент в самом окне. Так, например, InventoryUI представляет из себя UIWindow, на котором базируются кнопки, скроллбар и карточки, за логику которых отвечает уже InventoryMenu.cs.
Также есть кодовая основа для меню паузы, переключение между которыми будет осуществляться посредством меню-стека
- **UI: HUD с информацией о предметах**: эта часть HUD-а при наведении камеры на предмет выводит на экран карточку с информацией о предмете с его названием, типом и редкостью. Сам предмет в это время обрамляется прямоугольником, охватывающим края **рендера** того или иного меша.
**WIP: класс Weapon : Item и система экипировки**: сейчас веду работу над тем, чтобы создать систему экипировки оружия персонажем в каждую из рук, а также с возможностью двуручного хвата какого-либо оружия. Хочу сделать именно такую, похожую на таковую из soulsborne-игр систему, так как:
  1. Это привлекательный челлендж
  2. Эта система - основа для экспериментов игроков с билдостроением
  3. Мне интересно путём эксперимента лично узнать, какой потенциал у такого рода ситсемы есть в шутерах от первого лица
