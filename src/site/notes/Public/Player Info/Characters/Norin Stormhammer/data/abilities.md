---
{"dg-publish":true,"dg-path":"Player Info/Characters/Norin Stormhammer/data/abilities.md","permalink":"/player-info/characters/norin-stormhammer/data/abilities/"}
---


`=floor(((11-10)/2) + 99) - 99`
`=sum([floor(((11-10)/2) + 99),-99])`
`=floor(0/2)`
`=0/2`
0.5
`=floor(1/2)`
`=floor((11-10)/2)`
`=floor((10-10)/2)`


## Ability Modifiers

|           Skill |                                                           Modifier                                                            |
| --------------: | :---------------------------------------------------------------------------------------------------------------------------: |
|       Athletics |  **5**   |
|                 |                                                                                                                               |
|      Acrobatics | **1**   |
| Sleight of Hand | **1**    |
|         Stealth | **1**    |
|                 |                                                                                                                               |
|          Arcana | **`= sum([number(floor(([[data]].int - 10)/2) + 99),sum(filter([number([[data]].pb), 0], (x) => [[data]].arcanaP = true OR x = 0)),-99])`**     |
|         History | **`= sum([number(floor(([[data]].int - 10)/2)),sum(filter([number([[data]].pb), 0], (x) => [[data]].historyP = true OR x = 0))])`**    |
|   Investigation | **`= sum([number(floor(([[data]].int - 10)/2)),sum(filter([number([[data]].pb), 0], (x) => [[data]].investigationP = true OR x = 0))])`** |
|          Nature | **`= sum([number(floor(([[data]].int - 10)/2)),sum(filter([number([[data]].pb), 0], (x) => [[data]].natureP = true OR x = 0))])`**     |
|        Religion | **2**    |
|                 |                                                                                                                               |
| Animal Handling |    **1**     |
|         Insight |    **3**    |
|        Medicine |   **1**    |
|      Perception |  **3**   |
|        Survival |   **1**    |
|                 |                                                                                                                               |
|       Deception |   **-1**   |
|    Intimidation | **-1**  |
|     Performance |  **-1**  |
|      Persuasion |  **1**   |


## Saving Throws
| Ability           |        Score        |
| ----------------- | :-----------------: |
| Strength:         | **5 ** |
| Dexterity         | **3 ** |
| Constitution      | **3 ** |
| Intelligence      | **`= sum([number(floor(([[data]].int - 10)/2)),sum(filter([number([[data]].pb), 0], (x) => [[data]].intSTP = true OR x = 0))])` ** |
| Wisdom            | **1 ** |
| Charisma          | **-1 ** |