# PDF-fletter

Flet flere PDF'er til én. Alt sker lokalt i browseren — ingen filer uploades nogen steder.

**Brug den her:** https://scheel86.github.io/pdf-fletter/

## Sådan virker den

1. Træk dine PDF'er ind på siden (eller klik for at vælge dem)
2. Sæt rækkefølgen med pilene
3. Vil du kun have nogle af siderne med: tryk **Vælg sider** og klik de sider fra, du ikke vil have
4. Tryk **Flet** — den samlede PDF hentes ned til din maskine

## Teknisk

Én selvstændig HTML-fil. [pdf-lib](https://pdf-lib.js.org/) 1.17.1 (MIT) samler PDF'erne, og
[pdf.js](https://mozilla.github.io/pdf.js/) 6.2.108 (Apache-2.0) tegner sidebillederne. Begge er
indlejret i filen, så der hentes intet udefra. Ingen server, ingen sporing, ingen cookies.

Sidebillederne tegnes i en baggrundstråd. Åbnes filen direkte fra disken (`file://`) i stedet for
via en adresse, blokerer browseren normalt baggrundstråde — så skriver siden det ærligt, og
siderne vælges efter sidetal i stedet. Selve fletningen virker uanset hvad.
