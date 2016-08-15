# Program

### Description:
??

### Benefit
??

### Attributes:

* **Description**: Short free-form text, accepts HTML
* **User**: Reference to a normal user account to demonstrate this training
* **Pokémon**: Reference to a single pokémon to demonstrate the training.
  (The pokémon's stats are displayed by default, but are not attributes of
  the program.)
* **Exercises**: Repeatable field set with attributes:
  * **Description**: Short free-form text, not accepting HTML
  * **Deals damage**: Boolean checkbox
  * **Chance of damage**: Floating-point numeric field indicating probability
    of damaged inflicted by the exercise.
  * **Recoil**: Floating-point numeric field indicating what kind of damage the
    user will receive from recoil.

### View Modes

* Default/Full
* Teaser

### Relationships:

* **User**: A normal user account that has at least one pokémon associated with it.
* **Pokémon**: Any Pokémon content.
