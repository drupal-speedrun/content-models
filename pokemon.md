# Pokemon

### Description:
A species of Pokemon and it's attributes.

### Benefit
As a normal user, I want to view information about various Pokémon so that
I can add them to my repertoire and compare them to other Pokémon.

### View Modes

* Teaser
    - Image: label hidden, Image formatter, Medium Square style
    - Types: label hidden, Label formatter, no link
    - Flag - Pokedex: Visible
* Expanded Teaser

### Attributes:

* Types (direct relationship to any number of types)
    - Machine name: field_type
    - Auto-completing text field
    - References taxonomy terms, Type (type) vocabulary only
    - Unlimited values
    - No default value
    - Optional
* Species (text, plain)
    - Machine name: field_species
    - No default value
    - Optional
    - Maximum values: 1
* Height (numeric, decimal)
    - Machine name: field_height
    - Optional
    - No default value
    - Minimum value: 0
* Weight (numeric, decimal)
    - Machine name: field_weight
    - Optional
    - No default value
    - Minimum value: 0
* Japanese Name (text, plain)
    - Machine name: field_japanese_name
    - Optional
    - No default value
    - Maximum values: 1
* Growth Rate (text, plain)
    - Machine name: field_growth_rate
    - Optional
    - No default value
    - Maximum values: 1
* Image
    - Machine name: field_image
    - Standard Lightning image browser
    - No default value
    - Optional
    - Alt text enabled and required
    - No minimum or maximum resolution
* Abilities (text, plain)
    - Machine name: field_abilities
    - Unlimited values
    - No default value
    - Optional

### Relationships:

* (many) User to (many) Pokémon -- users who have this Pokémon
    - Flag type: Content
    - Label: Pokedex
    - Scope: Personal
    - Flag link text: Add to Pokedex
    - Flagged message: This Pokemon has been added to your Pokedex.
    - Unflag link text: Remove from Pokedex
    - Unflagged message: This Pokemon has been removed from your Pokedex.
    - Flaggable types: Pokemon
    - Display link as field: YES
    - Link type: AJAX link
* (many) Type to (many) Pokemon -- each Pokémon can have any number of
  types
    - Related through Types field.
* Program (Zero or one pokemon to one Program)
    - Related through Training Program type's Pokemon field.
