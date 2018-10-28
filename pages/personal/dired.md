# dired

- hide details
`dired-hide-details-mode  bind to {{(}}`

- mark/unmark
`| key         | operation               |`
`|-------------+-------------------------|`
`| *s          | mark all files          |`
`| % m <regex> | mark file by regex      |`
`| u           | unmark current file     |`
`| U           | unmark all marked files |`
`| t           | invert selection        |`

- rename multiple files
`C-x C-q (dired-toggle-read-only)`
`change file names`
`C-c C-c`

- open file in external app (windows)
`! start ""`

- open file in external app (Mac)
`! open`

- create zip from marked files
`! zip -r <file.zip> *`
