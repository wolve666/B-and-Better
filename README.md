# B&Better

Gestionale per B&B e case vacanza, app Android realizzata da **E-Duck Garage**.

## Download

Scarica l'ultima `BandBetter.apk` da [Releases](https://github.com/wolve666/b-and-better/releases/latest) e installala sul telefono.

## Cosa fa

- Calendario delle prenotazioni con vista anno, mese e settimana (resta memorizzata l'ultima scelta). Scorri a destra e sinistra per cambiare periodo.
- Colonna delle case in gestione, ognuna con nome e colore: un tocco mostra solo quella casa, il secondo apre il suo menu.
- Tasto + per aggiungere check-in e check-out, con controllo delle sovrapposizioni e calcolo della tassa di soggiorno.
- Movimenti dei prossimi 30 giorni, conteggi del mese, archivio dei soggiorni conclusi.
- Backup e ripristino dei dati come testo.
- Versione accanto al nome: toccandola verifica gli aggiornamenti. All'avvio l'app controlla da sola e mostra una finestra quando c'è una versione nuova.

## Aggiornamenti

- La pagina dell'app (`www/index.html`) si aggiorna dentro l'app: basta alzare `APPV` in `www/index.html` e `version` in `version.json`.
- Se cambia la parte Android, si alza anche `NATIVE` e `native`: l'app proporrà di scaricare la nuova APK.

## Compilazione

GitHub Actions (`.github/workflows/build.yml`) compila e firma l'APK quando cambia `version.json` e la pubblica nella release `v<versione>`.
La firma usa i secret `KEYSTORE_B64` e `KEYSTORE_PASS`.
