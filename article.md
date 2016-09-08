# Article

### Description:
Basic content type similar to "Basic Page".

### Benefit
As an editor, I often need a generic place to store textual information and
associated, unstructured media.

### View Modes

* Full (Panelizer, choice allowed)
    - Default (Single column)
        - Authored By (no title, label hidden, Author formatter)
        - Authored On (no title, label hidden, Default formatter, Default medium date format, )
        - Body (no title, label above, Default formatter)
        - Blog (no title, label above, Field settings formatter)
    - Blog (Bootstrap Two Column 9/3)
        - Sidebar Right
            - Authored By (title visible, label above, Label formatter, linked)
            - Authored On (title visible, label above, Default formatter, Default medium date format)
            - Image (no title, label hidden, Image formatter, no style, no link)
            - Body (title visible, label above, Default formatter)
* Teaser
    - Image: label hidden, Image formatter, Medium style, linked to content
    - Body: label hidden, Summary or trimmed formatter, 600 character limit
* Featured Teaser

### Attributes:

* Title
    - One-line text field. Base field provided by Node module.
      Not configurable.
* Author
    - User reference. Base field provided by Node module. Not configurable.
* Date Created
    - Date field. Base field provided by Node module. Not configurable.
* Published
    - Boolean checkbox. Base field provided by Node module. Not configurable;
      controlled by Workbench Moderation. Not visible on when editing content.
* Blog
    - Boolean checkbox. Visible when editing content. Labeled "Include in blog".
      NOT checked by default.
* Body
    - Rich text field. Visible when editing content. Labeled "Body". Empty by
      default.
* Image
    - Standard image field. Uses Lightning's image browser. Visible when editing
      content. Empty by default. No minimum or maximum resolution.
* Moderation State
    - Entity reference select list. Base field provided by Workbench Moderation.
      Visible when editing content. "Draft" by default. Not configurable.

### Relationships:

* User (one author to many articles)
* Entity Block (implicit)
