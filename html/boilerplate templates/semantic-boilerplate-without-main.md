# Semantic Layout

NOTE ON BOILERPLATE TEMPLATES WITH VS CODE: VS Code has a shortcut. Delete everything in the index.html file. Click the ! and you'll be presented with a couple of options. Choose the first option.

Notes

* You may omit the header and it's decendants if it's only a sole headline and replace it with h1.

* In this example the navigation nav is a page specific navigation, hence after the page header.

* If the nav is a global navigation, it might also be before the first page header.

semantic-layout.txt
  +-----------------------------------+
  |               header              |
  +-----------------------------------+
  |                 nav               |
  +---------------------+-------------+
  |                     |             |
  |       section       |    aside    |
  |                     |             |
  |                     |             |
  | +-----------------+ |             |
  | |     article     | |             |
  | +-----------------+ |             |
  | |     article     | |             |
  | +-----------------+ |             |
  +---------------------+-------------+
  |               footer              |
  +-----------------------------------+
