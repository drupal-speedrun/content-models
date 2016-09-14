# Article

### Description:
Basic content type similar to "Basic Page".

### Benefit
As an editor, I often need a generic place to store textual information and
associated, unstructured media.

### Depends on
300x150 (image style)

### View Modes

* Full (Panelizer, choice allowed)
    - Default (Single column)
        - Authored By (no title, label hidden, Author formatter)
        - Authored On (no title, label hidden, Default formatter, Default medium date format)
        - Body (no title, label hidden, Default formatter)
    - Blog (9/3 Stacked)
        - Left
            - Authored By (no title, label inline, Label formatter, linked)
            - Authored On (no title, label inline, Default formatter, Default medium date format)
            - Image (no title, label hidden, Image formatter, no style, no link)
            - Body (no title, label hidden, Default formatter)
        - Right
            - Authored By (no title, label hidden, Rendered entity formatter, Compact view mode)
* Teaser
    - Image: label hidden, Image formatter, 300x150, linked to content
    - Body: label hidden, Summary or trimmed formatter, 600 character limit

### Attributes:

* Include in blog (boolean)
    - Checkbox
    - Machine name: field_blog
    - Checked by default: NO
    - Single value
* Image (image)
    - Machine name: field_image
    - No default value
    - Alt text enabled and required
    - Title not enabled
    - Required: NO
    - No minimum or maximum resolution

### Relationships:

* User (one author to many articles)
* Entity Block (implicit)
