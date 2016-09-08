# Training Program

### Description:
A training service for trainers to level-up their pokemon.

### Benefit
A way to communicate our offerings to visitors.

### Attributes:

* Title
    - One line text field. Base field provided by Node module. Not
      configurable.
* Description
    - Rich text field. Not required. Empty by default.
* Trainer
    - Entity reference auto-completing text field. References users, not
      including anonymous. Optional. Empty by default.
* Pokemon
    - Entity reference auto-completing text field. References node of the
      Pokemon bundle only. Optional. Empty by default.
* Exercises
    - Rich text field. Unlimited values allowed. Not required. Empty by
      default.
* Image
    - Standard image field. Uses the core upload widget. Optional. Empty
      by default. Minimum resolution 1280x1024.
* Teaser Image
    - Standard image field. Uses the core upload widget. Optional. Empty
      by default. Minimum resolution 512x512.

### View Modes

* Default/Full
* Teaser

### Relationships:

* **User**: A normal user account that has at least one pokémon associated with it.
* **Pokémon**: Any Pokémon content.
* **Registrants**: Users who have registered for this program
