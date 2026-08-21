TROVIAMOCI - pagina link

Immagini:
- img/foto.png = logo "Ti va un caffè" in alto a sinistra (sfondo trasparente)
- img/sfondo.png = immagine di sfondo a tutta pagina
- img/foto2.png = icona "vietato ai minori" mostrata nel pulsante "Sito"

Puoi sostituire img/foto.png, img/foto2.png e img/sfondo.png direttamente da GitHub
mantenendo gli stessi nomi. Se la nuova foto.png ha uno sfondo bianco pieno, chiedi di
renderla trasparente prima di caricarla, altrimenti apparirà un riquadro bianco intorno al logo.

Link attuali:
Chat -> https://anonima-jb41.onrender.com
Sito -> https://xchat60.duckdns.org

Layout pagina:
- Logo in alto a sinistra (non copre il viso del personaggio sullo sfondo)
- Pulsante "Chat" in basso, stile chiaro con bordo dorato e icona rotonda marrone
- Pulsante "Sito" sotto "Chat", stesso stile, con l'icona "vietato ai minori" al posto
  dell'icona a fumetto
- Nessun titolo di testo sopra i pulsanti (rimosso su richiesta)

Per aggiungere altri pulsanti, copia il blocco <a class="chat-button">...</a> dentro index.html
e cambia link/testo/icona.

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
