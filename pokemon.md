# Pokemon

### Description:
A species of Pokemon and it's attributes.

### Benefit
As a normal user, I want to view information about various Pokémon so that
I can add them to my repertoire and compare them to other Pokémon.

### View Modes

* Full
* Teaser
* Expanded Teaser

### Attributes:

* Name
    - One line text field. Base field provided by Node module. Not configurable.
* Types (direct relationship to any number of types)
    - Entity reference auto-completing text field. References taxonomy terms in
      the Types vocabulary. Unlimited number of values. Empty by default. Not
      required.
* Species
    - One line text field. Empty by default.
* Height (numeric)
    - Short text field. Accepts numbers only, including decimals. Not required.
      Empty by default.
* Weight (numeric)
    - Short text field. Accepts numbers only, including decimals. Not required.
      Empty by default.
* Japanese Name
    - One line text field. Empty by default. Optional.
* Growth Rate
    - One line text field. Empty by default. Optional.
* Image
    - Standard image field. Uses Lightning's image browser. No default value.
      Not required. Empty by default. Alt field enabled. No minimum or
      maximum resolution.
* Abilities
    - Single line text field. Unlimited values allowed. Empty by default.
      Optional.

### Relationships:

* (many) User to (many) Pokémon -- users who have this Pokémon
* (many) Type to (many) Pokemon -- each Pokémon can have any number of
  types
* Program (Zero or one pokemon to one Program)

