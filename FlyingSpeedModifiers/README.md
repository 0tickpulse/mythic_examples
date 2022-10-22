# Flying Speed Modifier

A skill that changes the flying speed of a mob.

To use the skill, one needs to add the following line to their flying mobs:

```yml
- skill{s=Speed_ChangeFlyingSpeed_Initialize;speedcap=[speedcap];interval=[interval]} @Self ~onSpawn
```

Parameters:

* `speedcap` - the maximum blocks the entity can move from the last iteration of the skill before the skill modifies the entity's speed
* `interval` - the number of ticks between iterations of the skill

For example, if one want the entity to move at max two blocks every half a second, one would write the following:

```yml
- skill{s=Speed_ChangeFlyingSpeed_Initialize;speedcap=2;interval=10} @Self ~onSpawn
```

## Credits

Author: @LorenzoPierro

Editor: @0tickpulse