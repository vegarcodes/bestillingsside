# Bestillingsside

## Hva er dette?

Dette er en øvingsoppgave som skal hjelpe deg å få mengdetrening i bruk av JavaScript. Les oppgaveteksten nøye og forsøk å dele den opp i overkommelige blokker før du setter i gang.

## Case

En liten kaffebar kalt Quantum Café har fått laget en ny bestillingsside. Designet er ferdigstilt, og HTML og CSS for siden er laget. Men siden er ikke funksjonell! Når man trykker på knappene for å bestille skjer det foreløpig ingenting. Derfor er du kalt inn for å gjøre denne siden interaktiv!

## Hva menes med interaktiv?

- Knappene på hver produktlinje skal kunne trykkes på for å endre antall produkter man ønsker å bestille av hver type. Plussknappene legger til og minusknappene trekker fra antallet på det bestemte produktet.
- Når brukeren endrer antallet, skal også totalsummen som vises endres. Denne summen skal holdes oppdatert hele tiden, slik at når brukeren trykker på knappene, får hen alltid se hvor mye totalbeløpet kommer på.
- Når modalen vises idet brukeren trykker på bestillingsknappen, skal brukeren få beskjed i den om hva totalsummen ble. Du må altså oppdatere totalsummen flere steder.
- Det skal ikke være mulig å bestille færre enn null av noe.
- Det skal ikke være mulig å legge til bestillinger for mer enn 500 kroner. Dersom brukeren forsøker å legge til noe slik at summen ville blitt høyere enn 500 kroner, skal det vises en meldingsboks om at brukeren ikke får lov til å gjøre dette.

## Noen ekstra utfordringer

- Litt vanskelig: hvis brukeren trykker på bestillingsknappen uten at noe er bestilt, skal ikke modalen vises for brukeren.
- Vanskeligere: du skal legge prisene for hvert produkt inn i JavaScript, og når siden lastes inn skal JavaScript oppdatere prisene i grensesnittet. På denne måten skal man kunne endre prisene i JavaScript alene uten å røre HTML-koden.

## Tekniske krav

- Du får ikke lov til å endre HTML eller CSS i denne oppgaven. Kun JavaScript skal brukes, og all JavaScript du skriver skal ligge inne i `./scripts/script.js`. 
- Antall produkter en bruker har lagt til, samt totalsummen for bestillingen, skal defineres som variabler. Du skal bruke `const` der du vet at verdien ikke endres, og `let` der du vet at verdien vil endres.
- Alle funksjoner du skriver skal bindes opp til HTML ved bruk av event listeners.
- Du skal lage en funksjon som heter `addProduct` som legger til et produkt i bestillingen. Hvilket produkt som legges til skal du definere gjennom et parameter som heter `productName`. Funksjonen skal ta høyde for alle de ulike produktene en bruker kan legge til. Når du binder opp en event listener til knappene, kan du sende inn en verdi som parameter som identifiserer hvilket produkt som skal legges til.
- Du skal lage en tilsvarende funksjon som heter `subtractProduct` som trekker fra et produkt i bestillingen. I tillegg til kravene ovenfor skal denne funksjonen oppdage om det er mulig å trekke fra produktet eller ei, og hvis ikke skal ikke funksjonen gjøre noe.
- Du skal lage en funksjon som heter `calculateTotal`. Denne funksjonen regner ut totalsummen brukeren skal betale basert på informasjonen du har lagret i variablene.
- Du skal lage en funksjon som heter `updateUI`. Denne funksjonen skal oppdatere alle HTML-elementer med nye verdier der det trengs. Dette gjelder totalsum på oversiktssiden, totalsum i bekreftelsesmodalen, og antall produkter som er bestilt. Her må du bruke det du har lært så langt om DOM-manipulasjon til å gjøre det som trengs.

Utover dette står du fritt til å løse oppgaven som du ønsker, lage flere funksjoner eller variabler hvis du ser at det trengs, og du kan legge på ytterligere tilleggsfunksjonalitet om du vil utfordre deg selv.

Lykke til!