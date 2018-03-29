# documentation

architecture decision records (ADRs), diagrams, explanation of processes, any other reference material and reports of past issues never solved

## table of contents

- architecture-decision-records

**TODO**: this can probably become a template+makefile combo (see actual-cookbook for reference)

## how to use this repo

### guidelines

- **use markdown**: textual, simple and github renders it nicely for free
- **curate commit messages**: they're the tool to keep track of change so make them communicate
- **use consistent terminology**: allows simple search tools like "find in page" and `grep` to be highly effective
- **be concise**: nobody likes to read or write documentation when documents are as long as the lord of the rings
- **explain reasoning**: presprictive statements can become dogma, explaining reasonsing allows to challenge past decisions in a changing future
- **source for binaries**: if you have source files for binaries commit them as well to enable reproducibility (e.g. the `xml` export of a [draw.io](https://draw.io/) diagram as well as the `png`)
- **don't ask for permission, ask for reality check**: if you want to edit or add anything just go ahead and do it but make sure that what you're writing is understandable and not your unilateral opinion

### searching this repo

#### on your filesystem

you can use `grep` to match words or regular expressions. an example common usage would be:

`grep -rin "terms" .`

from this repo's top-level directory. this searches for the word "terms" (replace with your search, ofc) in this directory and all subdirectories recursively (`-r`), will match your search case-insensitively (`-i`) and output the filename and line number along matches (`-n`).

for more advanced use of `grep` refer to the manual (`man grep`)

#### on web

use the "find in page" function of your browser to find specific content in a file

on github you can use the top search bar to find words in this repo

## markdown cheatsheet

full documentation is available on [daring fireball](https://daringfireball.net/projects/markdown/), a quick list of the most common things you might need:

- `# section header`
- `## smaller section header, the more #s the smaller the header`
- `- list item`
- `  - sub list item (2 spaces for each nest level)`
- `\`inline code\``
- `*italic*`
- `**bold**`
- `[make this text a link](https://example.com)`
- if you want to force a newline, you need an entire blank line (so two newlines)

