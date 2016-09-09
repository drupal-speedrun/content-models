# Pokedex

### Description:
Grid display of pokemon

### Benefit
As a user of the site, I want a way to view all available pokemon and be able
to view just those that have been added to my pokedex.

### Depends on
- Pokemon (node bundle)
- Pokemon <-> User (flag)

### Wizard
* View Settings
  - Show: Content
  - Type: Pokemon
  - Sorted by: Title
* Page settings
  - Create page: TRUE
  - Page title: "All Pokemon"
  - Path: `/pokemon`
  - Display format
    - Unformatted List
    - Teasers
  - Items to display: 0
  - Use pager: TRUE
* Block settings
  - Create block: TRUE
  - Block title: Pokedex
  - Display format
    - Unformatted List
    - Teasers
  - Items per block: 0

### Defaults
* Format
  - Unformatted list
    - Row class: "col-lg-3 col-md-4 col-sm-6"
  - Content: Teaser
* Filters
  - Published: TRUE
  - Content Type: Pokemon
  - Content Title (Exposed)
    - Label: Filter
    - Operator: Starts With
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
      - Flagged
        - Relationship: Pokedex Current User Flag
        - Status: Flagged
* All Pokemon (page)
  - Path: /pokemon
  - Menu: Normal: All Pokemon

