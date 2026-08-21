TROVIAMOCI - pagina link

Immagini:
- img/foto.png = logo/foto circolare
- img/sfondo.png = immagine di sfondo

Puoi sostituire queste immagini direttamente da GitHub mantenendo gli stessi nomi.

Link attuale:
Chat -> https://anonima-jb41.onrender.com

Per aggiungere altri pulsanti, copia il blocco <a class="link-button">...</a> dentro index.html.

INSTALLAZIONE COME APP (PWA)
La pagina ora è installabile come una vera app, non solo come scorciatoia:
- Su Chrome Android: comparirà un pulsante "Installa app" appena il sito rileva che è installabile.
- Se il pulsante non compare (es. Safari su iPhone, o alcuni browser), viene mostrato un
  messaggio che spiega di usare il menu del browser -> "Aggiungi a schermata Home".

File aggiunti per la PWA:
- manifest.json = nome, icone e colori dell'app installata
- sw.js = service worker, necessario per l'installazione e per il funzionamento offline base
- img/icon-192.png e img/icon-512.png = icone generate da img/foto.png

Se cambi img/foto.png e vuoi aggiornare anche l'icona dell'app, rigenera icon-192.png e
icon-512.png (192x192 e 512x512 px) con lo stesso contenuto della nuova foto.

IMPORTANTE: la PWA (manifest + service worker) funziona solo se il sito è servito in HTTPS
(GitHub Pages lo è già di default), altrimenti il browser non mostrerà mai il pulsante di
installazione.
