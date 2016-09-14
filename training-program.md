# Training Program

### Description:
A training service for trainers to level-up their pokemon.

### Benefit
A way to communicate our offerings to visitors.

### Attributes:

* Description (text, long, formatted)
    - Renamed body field.
* Trainer (entity reference)
    - References users
    - Auto-completing text field
    - Required: NO
    - No default avlue
    - Does NOT include anonymous user
    - Maximum values: 1
* Pokemon (entity reference)
    - References content, Pokemon bundle only
    - Auto-completing text field
    - Required: NO
    - No default value
    - Maximum values: 1
* Exercises (text, long, formatted)
    - Required: NO
    - No default value
    - Unlimited values
* Image (image)
    - Required: NO
    - No default value
    - Minimum resolution 1280x1024
    - Maximum values: 1
    - Uses core upload widget
* Teaser Image
    - Required: NO
    - No default value
    - Minimum resolution: 512x512
    - Maximum values: 1
    - Uses core upload widget

### View Modes

* Full Content (Panelizer, choice allowed)
    - Default (Stripey Stacked)
        - Top:
            - Description (no title, label hidden, Default formatter)
        - Left (6 columns):
            - Trainer (title visible, label hidden, Rendered entity formatter, Compact view mode)
        - Right (6 columns):
            - Pokemon (title visible, label hidden, Rendered entity formatter, Teaser view mode)
        - Bottom:
            - Exercises (no title, label hidden, Default formatter)
    - Alternative (Stripey Stacked):
        - Left (6 columns):
            - Body (no title, label hidden, Default formatter)
        - Right (3 columns):
            - Trainer (title visible, label hidden, Rendered entity formatter, Compact view mode)
            - Pokemon (title visible, label hidden, Rendered entity formatter, Teaser view mode)
        - Bottom (containerless):
            - Exercises (no title, label hidden, Default formatter)
* Teaser
    - Teaser Image: label hidden, Image formatter, 220x220 style, linked to content
    - Description: label hidden, Summary or trimmed formatter, 600 character limit

### Relationships:

* **User**: A normal user account that has at least one pokémon associated with it.
* **Pokémon**: Any Pokémon content.
* **Registrants**: Users who have registered for this program
