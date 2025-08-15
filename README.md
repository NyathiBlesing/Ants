# Ants

<img width="470" height="239" alt="Capture" src="https://github.com/user-attachments/assets/9841bc1a-7126-42bd-9f69-e78efb1cae46" />

This is a tower defense game called Ants Vs. SomeBees. As the ant queen, populate colony with the bravest ants muster. Ants must protect their queen from the evil bees that invade the territory. They must Irritate the bees enough by throwing leaves at them, and they will be vanquished. Fail to pester the airborne intruders adequately, and the queen will succumb to the bees' wrath. This game is inspired by PopCap Games' Plants Vs. Zombies ®.

## Core Concepts

A game of Ants Vs. SomeBees consists of a series of turns. In each turn, new bees may enter the ant colony. Then, new ants are placed. Finally, all insects (ants, then bees) take individual actions: bees sting ants, and ants throw leaves at bees. The game ends either when a bee reaches the ant queen (you lose), or the entire bee flotilla has been vanquished (you win).

The Colony: The colony consists of several places that are chained together. The exit of each Place leads to another Place.

Placing Ants: There are two constraints that limit ant production. Placing an ant uses up some amount of the colony's food, a different amount for each type of ant. Also, only one ant can occupy each Place.

Bees: When it is time to act, a bee either moves to the exit of its current Place if no ant blocks its path, or stings an ant that blocks its path.

Ants: Each type of ant takes a different action and requires a different amount of food to place. The two most basic ant types are the HarvesterAnt, which adds one food to the colony during each turn, and the ThrowerAnt, which throws a leaf at a bee each turn.

However, with great power comes great responsibility. The Queen is governed by three special rules:

1. If a bee ever enters the place occupied by the queen, then the bees immediately win the game. The game ends even if the queen is protected by a bodyguard. The bees also win if any bee reaches the end of a tunnel where the queen normally would reside.

2. There can be only one true queen. Any queen beyond the first one is an impostor and should die immediately (its armor reduced to 0) upon taking its first action, without doubling any ant's damage or throwing anything. Impostor queens should not affect the colony's queen attribute. You can detect impostor queens by counting the number of times that an instance of a QueenAnt has been constructed, using a class attribute. Any QueenAnt beyond the first one created is an impostor. You should not have to search through the colony places to find other queens.

3. The true (first) queen cannot be removed. Attempts to remove the queen should have no effect.


This project combines functional and object-oriented programming paradigms.

## Programming Language used:

Python

Credits:  John DeNero
