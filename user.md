# User

### Description:

A user of the site with login credentials and personal collection of Pokemon.

### Benefits:

### Attributes:

* Username
    - One line text field. Base field provided by User module. Not configurable.
* Picture
    - Standard image field. Uses core upload widget. Required. Defaults to a
      picture of a pokeball, which is installed by the Speedrun User Display
      feature. Minimum resolution 480x480.
* Pokemon enthusiast since
    - Date field. Defaults to current date. Exposes year, month, and day select
      lists. Optional.

## View Mode

* Full
* Teaser

### Relationships:

* (many) Pokemon to (many) User
* (many) Role to (manu) user

