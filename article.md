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
        - Body (no title, label above, Default formatter)
        - Blog (no title, label above, Field settings formatter)
    - Blog (Bootstrap Two Column 9/3)
        - Sidebar Right
            - Authored By (title visible, label above, Label formatter, linked)
            - Authored On (title visible, label above, Default formatter, Default medium date format)
            - Image (no title, label hidden, Image formatter, no style, no link)
            - Body (title visible, label above, Default formatter)
* Teaser
    - Image: label hidden, Image formatter, 300x150, linked to content
    - Body: label hidden, Summary or trimmed formatter, 600 character limit

### Attributes:

* Blog
    - Boolean checkbox. Visible when editing content. Labeled "Include in blog".
      NOT checked by default. Single value.
* Body
    - Rich text field. Visible when editing content. Labeled "Body". Empty by
      default. Created automatically with the content type.
* Image
    - Standard image field. Uses Lightning's image browser. Visible when editing
      content. Empty by default. No minimum or maximum resolution. Optional.
      Alt text enabled.

### Relationships:

* User (one author to many articles)
* Entity Block (implicit)
