# Ciclo di Kendra

App web personale per il ciclo: calendario con cicli, previsioni, giorni fertili e ovulazione, registro dei sintomi e consigli.

- La data del prossimo ciclo si calcola dall'ultimo ciclo segnato più la durata media (ultimi 6 cicli, all'inizio 28 giorni). Non si sposta da sola: se il ciclo non arriva, l'app conta i giorni di ritardo.
- I file del sito vengono pubblicati con GitHub Pages dalla cartella principale.
- I dati sono salvati su Supabase nella tabella `ciclo_kendra`, protetti da login e da regole di accesso.
- In `config.js` ci sono solo l'indirizzo del progetto e la chiave pubblica: nessuna password.
- Le notifiche arrivano dalla funzione "promemoria" del progetto Supabase (dispositivi con `app = 'ciclo'`).
