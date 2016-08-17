# Training Program

### Description:
A training service for trainers to level-up their pokemon.

### Benefit
A way to communicate our offerings to visitors.

### Attributes:

* **Description**: Short free-form text, accepts HTML
* **User**: Reference to a normal user account to demonstrate this training
* **Pokémon**: Reference to a single pokémon to demonstrate the training.
  (The pokémon's stats are displayed by default, but are not attributes of
  the program.)
* **Image**: (Optional) Minimum resolution 1280x1024.
* **Teaser Image** (required) Minimum resolution 512x512
* **Exercises**: Repeatable field set with attributes:
  * **Description**: Long free-form text, accepts HTML

### View Modes

* Default/Full
* Teaser

### Relationships:

* **User**: A normal user account that has at least one pokémon associated with it.
* **Pokémon**: Any Pokémon content.
* **Registrants**: Users who have registered for this program
