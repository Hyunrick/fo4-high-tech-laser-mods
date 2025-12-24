High-Tech Laser Mods
================================================================================

This is a [Fallout 4 Mod (Creation)](https://creations.bethesda.net/fallout4/) for PC (Steam) and PlayStation (PS5).

Description
-----------

This creation adds a new set of laser weapon mods that scale with the Science! perk, giving energy weapons a distinct progression path separate from ballistics. Instead of raw damage alone, these mods emphasize precision, efficiency, and advanced energy behavior—rewarding intelligent builds with improved V.A.T.S. performance, critical potential, targeting, and utility effects.

- V.A.T.S. Capacitors reduce AP cost
- Electrocution Barrels cause damage over time
- Beam Modulation Muzzles highlight hostiles on hit
- Precision Headshot Scopes increase headshot chance
- Targeting Matrix Grips increase critical hit chance

Activate these benefits by crafting "High-Tech Laser Weapons" at the Chemistry Station under "Utilities" and read it. This will unlock the weapon mod benefits.

All mods use vanilla mechanics, require no new assets, and are fully compatible with PlayStation and PC.

The Big TL;DR
-------------

### Design Concept

The goal was to create some laser weapon components that added more differentiation
from ballistic builds--to lean into the intelligence/tech/science theme. These 
laser weapon mods scale on the Science! perk rather than the traditional method
of a crafting gate and leveled loot drops. Scaling on Science! provides additional
incentive to prioritize investment in the Intelligence/Science! path for energy
builds.

Another design goal was to think of energy weapons as being about precision and
efficiency over raw damage. 


### V.A.T.S. Capacitor

There is only one Capacitor (aka Receiver) which provides a reduction to AP cost
that scales on the level of the Science! perk (implicit level gate).

| Science!   | AP Cost |
|------------|--------:|
| 1 (lvl 6)  | -2      |
| 2 (lvl 17) | -4      |
| 3 (lvl 28) | -6      |
| 4 (lvl 41) | -8      |


### Electrocution Barrels

Electrocution barrels apply a _stacking_ damage-over-time (DoT) on hit.

Due to some implementation constraints, there are 4 Electrocution Barrels (Mk1 - Mk4)
rather than a single component that scales on Science!. Instead, each barrel's DoT 
is locked by the corresponding Science! perk.

The DoT lasts for 3 seconds and the rate-of-fire (RoF) is hard-capped at 4 shots
per second. This short-lived but stacking DoT rewards an aggressive single target
playstyle to maximize DPS.

The DoT is always 3 seconds but the magnitude (dmg per tick) scales on the 
Science! perk (implicit level gate).

| Tier | Science! Rank | Dmg/Tick |
|------|---------------|---------:|
| Mk1  | 1 (lvl 6)     | 3.00     |
| Mk2  | 2 (lvl 17)    | 3.75     |
| Mk3  | 3 (lvl 28)    | 4.25     |
| Mk4  | 4 (lvl 41)    | 5.00     |

The barrel's base damage, as shown in the Pip-Boy card and crafting menu is
misleading. It shows the base damage plus the per-tick damage of the DoT. The
base damage is reduced to account for the DoT, however, effort was also taken to 
ensure the damage reported in the Pip-Boy doesn't discourage the player.

The base progression damage for each barrel +2 → +4 → +8 → +12.

They also shoot a blue beam and have a blue electrocution FX on the targets while
the DoT is applied. 


### Targeting Matrix Grips

There are 2 grips--one to create a pistol and one to create a rifle. The grips
provide an increase to critical chance that scales on the level of the Science!
perk (implicit level gate).

| Science!   | Crit Chance |
|------------|------------:|
| 1 (lvl 6)  | +1%         |
| 2 (lvl 17) | +2%         |
| 3 (lvl 28) | +4%         |
| 4 (lvl 41) | +6%         |


### Precision Headshop Scopes

There are 3 scopes equivelent to the short, medium, and long on the vanilla laser
weapons. The scopes provide an increased chance to land a headshot in V.A.T.S. that
scales on the level of the Science! perk (implicit level gate).

The different scopes all have the same Science! scaling--they provide different
zoom levels to suit the player's preference/situation.

| Science!   | Headshot Chance |
|------------|----------------:|
| 1 (lvl 6)  | +1%             |
| 2 (lvl 17) | +2%             |
| 3 (lvl 28) | +3%             |
| 4 (lvl 41) | +4%             |


### Beam Modulating Muzzles

Beam Modulating Muzzles highlight (white glow) targets on hit making them easier
to track--especially in low light. There are three tiers of muzzle (Mk1 - Mk3)
which each have a Science! rank requirement.

| Tier | Science!   | Highlight |
|------|------------|----------:|
| Mk1  |            | 6s        |
| Mk2  | 1 (lvl 6)  | 8s        |
| Mk3  | 2 (lvl 17) | 12s       |

A player with Science! Rank 2 would be able to use _any_ of the muzzles and get
that muzzle's effect. A player with Rank 1 would only be able to use Mk1 and Mk2.

Author's Note about Balance
---------------------------

Balance is hard--especially when trying to create some unique effects. A lot of
math was done, and then thrown out after getting the "feel" while playing, and
then repeating that process over and over. From game difficulty setting to
enemy types and resistances to different builds stacking different stats--there
are too many permutations to account for them all.

So please, share your feedback with me. Even if it's just how it "feels" to
play with one or more of these weapon mods.
