# PDF-fletter

Flet flere PDF'er til én. Alt sker lokalt i browseren — ingen filer uploades nogen steder.

**Brug den her:** https://scheel86.github.io/pdf-fletter/

## Sådan virker den

1. Træk dine PDF'er ind på siden (eller klik for at vælge dem)
2. Sæt rækkefølgen med pilene
3. Tryk **Flet** — den samlede PDF hentes ned til din maskine

Siden virker også uden internet: gem den (Ctrl+S) og åbn filen direkte.

## Teknisk

Én selvstændig HTML-fil. [pdf-lib](https://pdf-lib.js.org/) 1.17.1 (MIT) er indlejret i filen,
så der hentes intet udefra. Ingen server, ingen sporing, ingen cookies.
