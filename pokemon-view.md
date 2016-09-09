# Pokedex

### Description:
Grid display of pokemon

### Benefit
As a user of the site, I want a way to view all available pokemon and be able
to view just those that have been added to my pokedex.

### Depends on
- Pokemon (node bundle)
- Pokemon <-> User (flag)

### Defaults
* Format
  - Unformatted list
    - Row class: "col-lg-3 col-md-4 col-sm-6"
  - Content: Teaser
* Filters
  - Published: TRUE
  - Content Type: Pokemon
  - Content Title (Exposed)
* Sort Criteria
  - Title: asc
* Access: Permission (View published content)

### Displays
* Pokedex Block (block)
  - Overrides
    - Relationship
      - Content Flag
        - Administrative title: "Pokedex Current User Flag"
        - Include only flagged content: TRUE
        - Flag: Pokedex
        - By: Current user
    - Filters
      - Inherit all defaults
      - Pokedex Current User Flag:
        - Flagged: TRUE
* All Pokemon (page)
  - Path: /pokemon
  - Menu: Normal: All Pokemon

