# Landing Page Block

### Description
Block type with special settings for landing pages

### Benefit
As an editor, I want control over how landing pages look including background
images, columns, and references.

### Attributes
* Background Image (image)
  - Description: *"Optionally, upload an image which will be displayed behind the contents of this block."*
  - Required: FALSE
  - Disable alt and title fields
  - Machine name: `field_background_image`
  - Number of values: 0 or 1
* Body
  - Default
* Column (text - formatted, long)
  - Description: *"Optionally, use this repeatable field to add columns of content to the bottom of the block."*
  - Number of values: 0, 1, or many
  - Machine name: `field_column`
* Content width (Number - integer)
  - Description: *"Enter the number of columns this content should take up."*
  - Default value: 12
  - Required: TRUE
  - Min/Max: 1/12
  - Machine name: `field_content_width`
  - Number of values: 1
* Offset (Number - integer)
  - Description: *"Enter the number of columns this content should be offset from the left. This value plus the value for width cannot exceed 12."*
  - Default value: 0
  - Required: TRUE
  - Min/Max: 0/11
  - Machine name: `field_offset`
  - Number of values: 1
* User Reference (Entity reference)
  - Machine name: `field_user_reference`
  - Number of values: 0, 1, or many
  - Type of item to reference: User

