# Messale Ambrosiano — Composizione della Messa

Applicazione web a **file singolo**, offline, per comporre e consultare il testo della Messa secondo il Rito Ambrosiano. Pensata per un celebrante che vuole avere sull'ambone un unico testo pronto da seguire, senza dover sfogliare più volumi del Messale.

## Funzionalità principali

- Composizione guidata di tutte le parti della Messa (riti di introduzione, liturgia della parola, liturgia eucaristica, riti di conclusione, riti particolari), aperte in finestre dedicate a scomparsa.
- Le 12 Preghiere Eucaristiche ambrosiane (ordinarie I-VI, della Riconciliazione I-II, per varie necessità 1-4) con parti proprie (Communicantes, Hanc igitur, tempo liturgico, anamnesi) selezionabili.
- Blocchi fissi non ometti bili, gruppi di scelta a esclusione reciproca (es. atto penitenziale/aspersione), anteprima del testo prima di selezionarlo.
- Campi liberi (anche con formattazione minima) per le parti proprie del giorno: letture, salmo, orazioni, omelia, preghiera dei fedeli, avvisi.
- Rubriche in rosso, risposte dell'assemblea in grassetto, sigle CP/CC/1°C-4°C per la concelebrazione.
- Guida di consultazione rapida alle Premesse e Prænotanda del Messale, e una guida "Come funziona l'app".
- **Modalità celebrazione**: vista a schermo intero, testo ingrandibile, pensata per leggere durante la Messa da tablet/telefono.
- Stampa/PDF del testo composto.
- Funziona interamente offline: nessuna dipendenza esterna, nessuna connessione richiesta.

## Come usarla

Basta aprire `index.html` con un doppio click in qualunque browser moderno (Chrome, Safari, Firefox, Edge): l'app funziona anche senza connessione a internet e senza installazione.

In alternativa, se il repository viene pubblicato con GitHub Pages, l'app è raggiungibile direttamente da browser all'indirizzo pubblicato.

## Struttura del progetto

```
.
├── index.html       # l'intera applicazione (HTML + CSS + JS, nessuna dipendenza esterna)
├── manifest.json    # manifest per l'installazione come app (PWA) su smartphone/tablet
├── icons/           # set di icone (favicon, apple-touch-icon, icone PWA)
└── README.md
```

## Nota sui diritti dei testi liturgici

I testi liturgici contenuti nell'applicazione sono tratti dal **Messale Ambrosiano, II edizione (2024)**, © ITL srl / Arcidiocesi di Milano. Questo repository è pensato per un **uso personale del celebrante** e va mantenuto **privato**: i diritti sui testi restano dei rispettivi titolari e non è concessa alcuna licenza alla loro ridistribuzione.

Il codice dell'applicazione (HTML/CSS/JavaScript) può essere riutilizzato e adattato liberamente per uso personale; si raccomanda comunque di non ridistribuire pubblicamente i testi liturgici in esso contenuti.

## Pubblicare su GitHub (repository privato)

```bash
cd messale-ambrosiano-app
git init
git add .
git commit -m "Prima versione dell'app Messale Ambrosiano"
git branch -M main
git remote add origin https://github.com/<tuo-utente>/messale-ambrosiano-app.git
git push -u origin main
```

Ricorda di creare il repository su GitHub come **privato** prima di eseguire il push (spunta "Private" in fase di creazione, o imposta la visibilità da Settings → General → Danger Zone se il repository esiste già).
