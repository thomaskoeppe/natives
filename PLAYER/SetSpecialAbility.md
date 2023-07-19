---
ns: PLAYER
aliases: ["0xB214D570EAD7F81A"]
---
## _SET_SPECIAL_ABILITY

```c
// 0xB214D570EAD7F81A
void _SET_SPECIAL_ABILITY(Player player, int ability);
```

```
NativeDB Added Parameter 3: Any p2
```

Sets the Special Ability for a player.

Possible integers for ability:
1 - 
2 - Franklin Slowmotion Ability

## Parameters
* **player**: The player
* **ability**: Any int from 0 to ...

## Examples
```lua
-- Active the Franklin Slowmotion SpecialAbility for 10 seconds
SetSpecialAbility(PlayerId(), 2)
SpecialAbilityActivate(PlayerId())

Citizen.Wait(10 * 1000)

SetSpecialAbility(PlayerId(), 3)
SpecialAbilityActivate(PlayerId())
SpecialAbilityDeactivate()
```
