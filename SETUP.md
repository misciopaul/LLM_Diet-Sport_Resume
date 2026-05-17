# Setup Wiki Diet & Sport

Questa guida spiega come è stata configurata la wiki e come può essere modificata o riprodotta.

## Architettura del Sistema
Il sistema si basa su tre pilastri:
1. **`profilo.md`**: Il database dei dati corporei.
2. **`Diet/` & `Sport/`**: Cartelle per i log settimanali.
3. **`GEMINI.md`**: Il motore di automazione che istruisce l'AI su come processare i dati.

## Come Modificare il Sistema
- **Cambiare i calcoli:** Se vuoi cambiare le formule per il BMR o la Body Fat, modifica le istruzioni in `GEMINI.md`.
- **Cambiare il formato dei file:** Se preferisci un formato diverso per i nomi dei file (es. `Settimana-20-2026.md`), aggiorna la sezione "Archiviazione" in `GEMINI.md`.
- **Aggiungere nuovi parametri:** Se vuoi tracciare altro (es. ore di sonno, passi), aggiungi una nuova sezione in `GEMINI.md` descrivendo come vuoi che i dati vengano salvati.

## Riproduzione
Per replicare questo sistema in un nuovo vault Obsidian:
1. Copia il file `GEMINI.md` nella root del nuovo vault.
2. Crea le cartelle `Diet/` e `Sport/`.
3. Crea il file `profilo.md` con i parametri desiderati.
4. Gemini riconoscerà automaticamente le istruzioni e inizierà a gestire i log.
