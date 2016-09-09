# Training Program

### Description:
A training service for trainers to level-up their pokemon.

### Benefit
A way to communicate our offerings to visitors.

### Attributes:

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

* Full Content (Panelizer, choice allowed)
    - Default (Two column bricks)
        - Left above:
            - Trainer (title visible, label hidden, Rendered entity formatter, Compact view mode)
        - Right above:
            - Pokemon (title visibel, label hidden, Rendered entity formatter, Teaser view mode)
        - Middle:
            - Description (no title, label hidden, Default formatter)
        - Bottom:
            - Exercises (no title, label above, Default formatter)
    - Training 2 (Bootstrap Two Column 9/3)
        - Sidebar Right:
            - Body (no title, label hidden, Default formatter)
            - Exercises (no title, label hidden, Default formatter)
        - Sidebar Left:
            - Trainer (title visible, label hidden, Rendered entity formatter, Compact view mode)
            - Pokemon (title visible, label hidden, Rendered entity formatter, Teaser view mode)
* Teaser
    - Flag - Registrants: Visible
    - Links: Visible
    - Description: label hidden, Summary or trimmed formatter, 600 character limit

### Relationships:

* **User**: A normal user account that has at least one pokémon associated with it.
* **Pokémon**: Any Pokémon content.
* **Registrants**: Users who have registered for this program
