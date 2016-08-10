# Pokemon

### Description:

I have no idea.

### Benefits:
As a normal user, I want to view information about various Pokémon so that
I can add them to my repertoire and compare them to other Pokémon.

### Value:

### Attributes:

* Name (text, any length up to database limit)
* Types (direct relationship to any number of types)
* Species (text, any length up to database limit)
* Height (numeric)
* Weight (numeric)
* Japanese Name (text, any length up to database limit), in Romanized
  ASCII characters
* Growth Rate (text, possibly one of several limited values)

### Relationships:

* (many) User to (many) Pokémon -- users who have this Pokémon
* (many) Type to (many) Pokemon -- each Pokémon can have any number of
  types
