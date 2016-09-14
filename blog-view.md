# Blog

### Description
List of articles that are included in the blog.

### Benefit
As a site visitor, I want to see a chronological list of all blog articles.

### Dependencies
* Article content type

### Wizard
View name: Blog
Show **Content** of type **Article** sorted by: **Newest first**
Create a page:
    - Page title: Blog
    - Path: blog
    - Unformatted list of teasers
    - Display 10 items
    - Use a pager: YES
Create a block:
    - Block title: Blog
    - Unformatted list of teasers
    - Display 5 items
    
### Defaults
Filters:
    - Add "Include in blog (field_blog)", equal to True
