---
{"dg-publish":true,"dg-path":"Player Info/Characters/Norin Stormhammer/data/abilities.md","permalink":"/player-info/characters/norin-stormhammer/data/abilities/"}
---


| Ability           |        Score        | Saving Throw Proficient? |
| ----------------- | :-----------------: | :----------------------: |
| Strength:         | `INPUT[number:str]` |  `INPUT[toggle:strSTP]`  |
| Dexterity         | `INPUT[number:dex]` |  `INPUT[toggle:dexSTP]`  |
| Constitution      | `INPUT[number:con]` |  `INPUT[toggle:conSTP]`  |
| Intelligence      | `INPUT[number:int]` |  `INPUT[toggle:intSTP]`  |
| Wisdom            | `INPUT[number:wis]` |  `INPUT[toggle:wisSTP]`  |
| Charisma          | `INPUT[number:cha]` |  `INPUT[toggle:chaSTP]`  |
|                   |                     |                          |
| Proficiency Bonus | `INPUT[number:pb]`  |                          |

##### Ability Proficiencies

| Skill           |           Proficient           |
| --------------- | :----------------------------: |
| Athletics       |   `INPUT[toggle:athleticsP]`   |
|                 |                                |
| Acrobatics      |  `INPUT[toggle:acrobaticsP]`   |
| Sleight of Hand |    `INPUT[toggle:sleightP]`    |
| Stealth         |    `INPUT[toggle:stealthP]`    |
|                 |                                |
| Arcana          |    `INPUT[toggle:arcanaP]`     |
| History         |    `INPUT[toggle:historyP]`    |
| Investigation   | `INPUT[toggle:investigationP]` |
| Nature          |    `INPUT[toggle:natureP]`     |
| Religion        |   `INPUT[toggle:religionP]`    |
|                 |                                |
| Animal Handling |    `INPUT[toggle:animalP]`     |
| Insight         |    `INPUT[toggle:insightP]`    |
| Medicine        |   `INPUT[toggle:medicineP]`    |
| Perception      |  `INPUT[toggle:perceptionP]`   |
| Survival        |   `INPUT[toggle:survivalP]`    |
|                 |                                |
| Deception       |   `INPUT[toggle:deceptionP]`   |
| Intimidation    | `INPUT[toggle:intimidationP]`  |
| Performance     |  `INPUT[toggle:performanceP]`  |
| Persuasion      |  `INPUT[toggle:persuasionP]`   |



## Ability Modifiers

|           Skill |                                                           Modifier                                                            |
| --------------: | :---------------------------------------------------------------------------------------------------------------------------: |
|       Athletics |  **5 **   |
|                 |                                                                                                                               |
|      Acrobatics |  **1**   |
| Sleight of Hand |    **1**    |
|         Stealth |    **1**    |
|                 |                                                                                                                               |
|          Arcana |    **`= sum([number(floor((this.int - 10)/2)),sum(filter([number(this.pb), 0], (x) => this.arcanaP = true OR x = 0))])`**     |
|         History |    **2**    |
|   Investigation | **`= sum([number(floor((this.int - 10)/2)),sum(filter([number(this.pb), 0], (x) => this.investigationP = true OR x = 0))])`** |
|          Nature |    **2**     |
|        Religion |   **`= sum([number(floor((this.int - 10)/2)),sum(filter([number(this.pb), 0], (x) => this.religionP = true OR x = 0))])`**    |
|                 |                                                                                                                               |
| Animal Handling |    **3**     |
|         Insight |    **1**    |
|        Medicine |   **1**    |
|      Perception |  **1**   |
|        Survival |   **3**    |
|                 |                                                                                                                               |
|       Deception |   **1**   |
|    Intimidation | **1**  |
|     Performance |  **1**  |
|      Persuasion |  **1**   |


## Saving Throws
| Ability           |        Score        |
| ----------------- | :-----------------: |
| Strength:         | **5 ** |
| Dexterity         | **3 ** |
| Constitution      | **3 ** |
| Intelligence      | `INPUT[number:int]` |
| Wisdom            | `INPUT[number:wis]` |
| Charisma          | `INPUT[number:cha]` |