# 🥗 Diet & Sport Tracking Wiki (Obsidian + AI)

Benvenuto in questo progetto di Wiki personale per il tracciamento della dieta e dell'attività fisica, progettato per funzionare in modo simbiotico con **Obsidian** e un assistente AI (come **Gemini CLI**).

Questo repository fornisce una struttura pronta all'uso per chiunque voglia monitorare la propria salute in modo intelligente, automatizzando i calcoli nutrizionali e il tracciamento dei progressi corporei.

## 🚀 Funzionalità Principali

- **Log Alimentare Automatizzato:** Tu scrivi cosa mangi, l'AI calcola calorie e macro (proteine, grassi, carboidrati, fibre) e compila i file settimanali.
- **Tracking Sportivo:** Calcolo delle calorie bruciate basato sui tuoi dati antropometrici (MET).
- **Evoluzione Corporea:** Un sistema per tracciare peso e circonferenze nel tempo con calcolo automatico di BMR, TDEE e Body Fat.
- **Dashboard Centralizzata:** Un file `index.md` che funge da centro di controllo per navigare velocemente tra i log e i progressi.
- **Reminders Intelligenti:** Istruzioni integrate per sollecitare aggiornamenti bi-mensili dei dati corporei.

## ⚠️ Privacy & Sicurezza

**IMPORTANTE:** Se decidi di fare il fork di questo repository o di caricare la tua versione su GitHub, **non pubblicare i tuoi dati personali!**

I file come `profilo.md`, `Misure_Corporee.md` e i contenuti delle cartelle `Diet/` e `Sport/` conterranno informazioni sensibili sulla tua salute e le tue abitudini.
- Assicurati di aggiungere questi file al tuo `.gitignore` se intendi mantenere il repository pubblico.
- Usa questo repository come **template** privato o locale per la tua sicurezza.

## 📁 Struttura del Repository

- `Diet/`: Cartella destinata ai log alimentari settimanali (`YYYY-settimanaWW.md`).
- `Sport/`: Cartella destinata ai log degli allenamenti settimanali.
- `profilo.md`: Il tuo "database" corporeo attuale.
- `Misure_Corporee.md`: Tabella storica dell'evoluzione fisica.
- `index-template.md`: Template per la dashboard principale.
- `GEMINI.md`: Il file di istruzioni (System Prompt) che guida l'AI nella gestione della wiki.
- `SETUP.md`: Guida tecnica alla configurazione.

## 🛠 Come Usarlo

1. **Clona o scarica** questo repository come un nuovo vault di Obsidian.
2. **Copia `index-template.md` in `index.md`** per creare la tua dashboard privata.
3. **Configura il tuo assistente AI:** Assicurati che il tuo assistente legga il file `GEMINI.md`.
3. **Compila il Profilo:** Apri `profilo.md` e inserisci i tuoi dati (peso, altezza, età).
4. **Inizia a loggare:** Scrivi al tuo assistente: *"Oggi a pranzo ho mangiato 100g di pasta al pomodoro e un petto di pollo"* e guarda la wiki aggiornarsi da sola!

## 📱 Utilizzo su Smartphone (Senza Gemini CLI)

Se vuoi utilizzare la tua Wiki direttamente dal telefono senza passare per il terminale:

1.  **Setup Vault Mobile:** Scarica l'app di Obsidian per iOS o Android. Trasferisci la cartella di questo progetto sul telefono (es. tramite iCloud, Google Drive o cartelle locali) e aprila come un nuovo Vault all'interno dell'app.
2.  **Installazione Plugin AI:** Vai nelle Impostazioni di Obsidian -> Plugin della Community. Cerca e installa un plugin per l'integrazione di LLM (consigliati: **BMO Chatbot** o **Text Generator**).
3.  **Configurazione API (Gemini Standard):** 
    - Vai su [Google AI Studio](https://aistudio.google.com/) per ottenere gratuitamente una API Key di Gemini.
    - Inserisci la chiave API nelle impostazioni del plugin scelto all'interno di Obsidian, selezionando un modello della famiglia Gemini (es. `gemini-1.5-flash` o `gemini-1.5-pro`).
    - *(Nota: Se preferisci, puoi usare le API di altri provider come OpenAI o Anthropic configurandoli in modo simile).*
4.  **Setup del Prompt:** Nelle impostazioni del plugin, individua il campo dedicato al "System Prompt" o "Istruzioni di base". Copia l'intero contenuto del file `GEMINI.md` e incollalo lì. In questo modo l'AI integrata nel telefono conoscerà esattamente le regole per gestire la tua wiki di dieta e sport.

## 🤝 Contribuire
Questo è un progetto aperto! Se hai suggerimenti per migliorare le formule di calcolo o la struttura dei file, sentiti libero di aprire una Issue o una Pull Request.

---
*Creato con ❤️ per la salute e la produttività.*
