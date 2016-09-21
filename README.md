# Pre-built Things

Article node type
- Fields

Pokemon node type
- Fields
- Teaser view display
- User flag
- Page view of all pokemon in the system
- Block view of all pokemon flagged by the user

Training Program node type
- Content type shell entity
- User flag
- Block view of all training programs flagged by the user

User
- Fields
- Default view display, with Panelizer layouts:
  - Default
- Compact view display
- Register form display

Landing Page block type:
- Fields
- Default view display

Media block type:
- Fields
- Default view display

Type taxonomy vocabulary

220x220 image style

300x150 image style

# Live-built Things

Article node type
- Full Content view display with Panelizer layouts:
  - Normal
  - Blog
- Teaser view display
- Page view of article teasers that are flagged as blog articles
- Block view of article teasers that are flagged as blog articles

Pokemon node type
- Data import

Training Program node type
- Fields
- Full Content view display, with Panelizer layouts:
  - Default
  - Alternative

Tweet stream view
- Show media tweets
- Add a block, items to display: 3
- Add a filter "promoted to front page"

Content entry:
- Home page (landing page)
- Trainings page (landing page)
- Two trainings (training program) -- the other two are pre-built and imported somehow
- One blog post (article) -- several others are pre-built and imported

# Content Models for Drupalcon Dublin Speedrun Session

"*F" denotes anything that is pre-packaged in the speedrun feature.

Article (node bundle)
- Fields *F
- Full Content (view display, panelized)
  - Normal (default)
  - Blog
- Teaser (view display)
- Full-page teaser view of articles marked as being in the blog
- Block teaser view of articles marked as being in the blog

Pokemon (node bundle)
- Fields *F
- Teaser (display) *F
- Per-user ownership flag (I have this Pokemon) *F
- Block view of pokemon flagged by the user *F
- Page view of all pokemon in the system *F
- Data import

Training Program (node bundle)
- Fields
- Full Content (view display, panelized)
  - Template 1/Default
  - Template 2
- Teaser (view display)
- Per-user registration flag (I am signed up for this training) *F
- Block view of training programs the user has registered for *F

User *F
- Fields
- Default (view display, panelized)
- Compact (view display)
- Register (form display)

Landing Page Block (block bundle) *F
- Fields
- Default (display)

Media Block (block bundle) *F
- Fields
- Default (display)

Type (taxonomy vocabulary) *F

220x220 (image style) *F
- Scale & crop 220x220

300x150 (image style) *F
- Scale & crop 300x150

## Task checklist

**Content Models and layouts**
- [ ] Image style (850 x 150)
- [ ] Article
  - [ ] Full content (panelized)
  - [ ] blog
  - [ ] Teaser

- [ ] Blog (view)
  - [ ] Page
  - [ ] Block

- [ ] Training Program
  - [ ] Fields
  - [ ] Full content (panelized)
  - [ ] Default
  - [ ] Alternate

- [ ] Tweet stream (view)
- [ ] Article Moderation
  - [ ] New state (NLR)
  - [ ] Limited trainsitions

**Content Entry**
- [ ] Trainings

- [ ] About Us
  - [ ] Train with the best
  - [ ] We are passionate about fitness

- [ ] Homepage
  - [ ] Blocks
  - [ ] Train with the best
  - [ ] Be the best
  - [ ] Summer Speacial (premade)
  - [ ] Tweet
  
**Misc**
- [ ] Upload logo
- [ ] Set homepage path
