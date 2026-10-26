# Private Workspace — sito per GitHub Pages

Sito statico responsive per la pagina pubblica, l’informativa privacy e i termini di servizio di **Private Workspace**.

## File inclusi

- `index.html` — pagina principale
- `privacy.html` — informativa privacy e uso dei dati Google
- `terms.html` — termini di servizio
- `style.css` — stile condiviso e responsive

## Pubblicazione su GitHub Pages

1. Crea un nuovo repository su GitHub, per esempio `private-workspace`.
2. Carica questi quattro file e il `README.md` nella cartella principale del repository, senza cambiare i nomi.
3. Apri **Settings → Pages** nel repository.
4. In **Build and deployment**, seleziona **Deploy from a branch**.
5. Seleziona il branch `main`, la cartella `/ (root)` e premi **Save**.
6. Dopo alcuni minuti, GitHub mostrerà l’indirizzo pubblico, normalmente `https://NOMEUTENTE.github.io/private-workspace/`.

Gli URL da usare nella configurazione OAuth saranno:

- home: `https://NOMEUTENTE.github.io/private-workspace/`
- privacy: `https://NOMEUTENTE.github.io/private-workspace/privacy.html`
- termini: `https://NOMEUTENTE.github.io/private-workspace/terms.html`

Sostituisci `NOMEUTENTE` e, se diverso, `private-workspace` con i valori reali. In Google Cloud Console, inserisci gli URL pubblici nei campi corrispondenti della schermata consenso OAuth. GitHub Pages ospita solo queste pagine informative: non è un redirect OAuth e non contiene il codice dell’app.

## Controllo necessario prima della pubblicazione

La sezione 5 di `privacy.html` evita di affermare pratiche tecniche non confermate. Prima di pubblicare o sottoporre l’app alla verifica OAuth, confrontala con il comportamento reale dell’app. Se l’app conserva token OAuth, email, allegati, file, log o altri dati su sistemi controllati dallo sviluppatore, aggiorna l’informativa indicando con precisione quali dati vengono conservati, dove, per quanto tempo e come richiederne la cancellazione.

## Modifiche rapide

- Email di contatto: cerca `federico.boni.ri@gmail.com` nei file HTML.
- Anno e data: aggiorna il footer e la data in apertura delle pagine legali quando pubblichi modifiche.
- Colori: modifica le variabili all’inizio di `style.css`.

Non sono richiesti framework, dipendenze o processi di build.
