RFC Series (ISSN 2070-1721)

This repository contains a txt copy of all entries found in the RFC Index.
The index can be found at:
https://www.rfc-editor.org/rfc-index.html

This repository was created to maintain a local copy of each RFC entry to be
used by the program ``rfc``.
The script can be found at:
https://github.com/Tdback/scripts

If you wish to scrape the entries yourself, the following method was used, which
sleeps between jobs to help prevent rate limiting:
``parallel wget "https://www.rfc-editor.org/rfc/rfc{}.txt"';' \
    sleep 2 ::: $(seq 1 9477)``

