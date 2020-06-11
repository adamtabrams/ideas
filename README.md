# About

Ideas is a simple tool for keeping notes, lists, and ideas close at hand.
It lets you quickly add, view, or edit your notes and will save them to a git repo.
That way your notes will stay backed up and access.


# Setup

* Create a new, private git repo. And name it something like `my-ideas`.

* Install fzf if you don't already have it
    * For MacOS: `brew install fzf`

* Clone this repo and your private repo.
    * `git clone https://github.com/you/private-repo.git`
    * `git clone https://github.com/adamtabrams/ideas.git`

* Add the executable to your path. Here are some options for how:
    * Add the whole directory: `export PATH="$HOME/repos/ideas:$PATH"`
    * Copy into current path: `cp ideas ~/.local/bin/`
    * Link to it (my favorite): `ln -s ~/repos/ideas/ideas ~/.local/bin/ideas`

* Set ideas to use your private repo `ideas init ~/repo/your-private-repo`


# Usage

Create new ideas with `ideas new` or `ideas add`

View or edit existing ideas with `ideas` or `ideas NAME`

Remove unneeded ideas with `ideas rm`

Ideas automatically handles keeping your private repo synced.
