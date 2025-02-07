# ClaimBar

Claimed mobs HP bar addon for Ashita v3

Shows HP bars of monsters claimed by party and alliance. The bar will display without the player needing to target them.

3 bars are displayed by default. Number of bars can be set with command `/cb bars x`

![img](https://i.imgur.com/N6MlNtX.png)


## Commands

`/cb bars` - set the number of bars to display. Default = 2

`/cb scale` - set the scale of the bars. Default = 1. \
Can use decimal numbers `/cb scale 0.8`

 `/cb anim` - set bar drain animation length in seconds. Default = 0.5

 `/cb theme` - set theme. Default = 2 (CustomHud)

 `/cb dynamode` - sets claimbar do show all claimed mobs instead of in party/instance. Default = off

 ###Available options:

 `/cb theme 1` - Darksouls

![img](https://i.imgur.com/723b2Xa.png)

 `/cb theme 2` - CustomHud
 
![img](https://i.imgur.com/wpDbR8M.png)


## Limitations

1. Monsters' buff/debuff are not exposed to the game client. The code relies on incoming packets and messages to track them. Status effects gained/lost outside the range you'd receive messages cannot be tracked.

2. The order of monsters displayed follows their positions in memory. If the bars are displaying mobs #5 and #6, and your party claimed mobs #1 and #2, they will take the bars' place.

## Special thanks

* Creators of Debuffed addon, Auk/beauxq. The status effect tracker used their code almost unaltered.
* CustomHud creator Syllendel (Syll#3694) which inspired the creation of this addon.
* Thorny and at0mos who put up with my barrage of questions and provided support.
