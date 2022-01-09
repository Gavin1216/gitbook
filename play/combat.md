# 🌃 Combat

### Hit point

The ability of the warship to withstand damage, that is, the amount of his blood. At the beginning of entering the replica, each warship will display its own health. When the warship receives damage, the health will be reduced, and when the health is reduced to 0, the warship will withdraw from the battle. At the end of a PVE or PVP battle, the warship will restore all health.

$$
Hit point = 5 * vitality * (1+0.2* (warship level-1))
$$

### Attack

An attack can cause damage to the enemy. The physical damage character's attack is a physical attack, and the energy damage character's attack is an energy attack.

$$
Physical attack = Firepower* (1+0.2* (warship level-1))
$$

$$
Energy attack = Technology * (1+0.2* (warship level-1))
$$

### Physical defense

The ability of a warship to withstand physical damage.

$$
Physical defense = armor * (1+ 0.2* (warship level-1))
$$

The actual loss of the warship when it suffers physical damage.

$$
Health = opponent's Physical attack * (0.5-1.5 * random number) * 100 / (warship's Physical defense + 100)
$$

For example, when a warship with a defense of 100 points is attacked by an attack with a damage of 70 points, the actual damage suffered = 70 \* 100 / (100+100) = 35. That is, the warship will lose 35 health in this attack.

### Energy defense

The ability of a warship to withstand energy damage.

$$
energy defense = energy shield * (1+ 0.2* (warship level-1))
$$

The actual loss of the warship when it is damaged by energy

$$
Health = opponent's Energy attack * (0.5-1.5 random number) * 100 / (the warship's energy defense + 100)
$$

For example, when a warship with 100 energy defense is attacked by an attack with 70 damage, the actual damage it takes = 70\*100 / (100+ 100) = 35. That is, the warship will lose 35 health in this attack.

### Hit

The probability of hitting an opponent.

$$
Hit rate = attack square curvature engine / (attack square curvature engine + defense square curvature engine / 2)
$$

For example, when a warship with a curvature engine of 90 attacks a warship with a hit rate of 60, its hit rate = 90 / (90 + 60/2) = 75%, that is, there is a 75% chance that the attack will hit the opponent.
