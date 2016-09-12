# User

### Description:
A user of the site with login credentials and personal collection of Pokemon.

### Depends on:
- 220x220 (image style)
- pokemon (view)
- My trainings (view)

### Attributes:

* Picture
    - Standard image field. Uses core upload widget. Required. Defaults to a
      picture of a pokeball, which is installed by the Speedrun User Display
      feature. Minimum resolution 480x480.
* Pokemon enthusiast since
    - Date field. Defaults to current date. Exposes year, month, and day select
      lists. Optional.

## Form Mode

* Register
    - User name and password (visible)

## View Mode

* Default (Panelizer)
    - Pokedex (Two column stacked)
        - Left side:
            - Picture (no title, Image formatter, Medium Square style, no link)
            - Pokemon enthusiast since (no title, label above, Default formatter, HTML Year format)
        - Right side:
            - My Trainings (title visible)
        - Bottom:
            - Pokedex: Pokedex Block (title visible)
* Compact (Panelizer)
    - Default (Single column)
        - Picture (no title, label hidden, Image formatter, Thumbnail style, linked to content)
        - Name (no title, label hidden, User name formatter, linked to user)

### Relationships:

* (many) Pokemon to (many) User
* (many) Role to (manu) user

