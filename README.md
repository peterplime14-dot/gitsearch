gitsearch.sh

A CLI utility for searching GitHub repositories and users using parallel fetching and Python-based JSON processing.
Requirements


Bash: Shell environment.

curl: For API communication and fetching data.

python3: For JSON data extraction and parsing.

git: To clone repositories.

Core Utilities: sed, tail, wc, and cut.


Installation

Download the script as gitsearch.sh.

 Make executable:
  Bash

 chmod +x gitsearch.sh

Usage
Bash

./gitsearch.sh [FLAGS] <query> [language]

Flags

-u, --user: Search for users instead of repositories.

-n, --num: Specify the number of results to display (Default: 15).

Repository Search Logic

The script takes the first non-flag argument as the search term.

If a second non-flag argument is provided, it is used to filter by programming language.

    Spaces in queries are automatically converted to %20 for API compatibility.
