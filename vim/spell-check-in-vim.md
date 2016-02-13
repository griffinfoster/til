# Spell check in vim

Don't let typos sneak into production, you can use a spell checker right from Vim. Here's how:

`:set spell`

To navigate between spelling mistakes use `]s` and `[s`.

To correct spelling mistakes, go to the mistake and use `z=` to see suggestions.

P.S. if the spelling errors don't show up, make sure to check two things:

1. That you are not a fantastic speller and a true scholar
2. That the file type you are checking spell on is allowed (you can test it by setting your syntax to txt `:set syntax=txt`)

[source](https://til.hashrocket.com/posts/69d22497b7-spell-check-in-vim)
