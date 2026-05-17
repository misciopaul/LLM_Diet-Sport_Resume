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
- `index.md`: La dashboard principale per Obsidian.
- `GEMINI.md`: Il file di istruzioni (System Prompt) che guida l'AI nella gestione della wiki.
- `SETUP.md`: Guida tecnica alla configurazione.

## 🛠 Come Usarlo

1. **Clona o scarica** questo repository come un nuovo vault di Obsidian.
2. **Configura il tuo assistente AI:** Assicurati che il tuo assistente legga il file `GEMINI.md`. Se usi Gemini CLI, lo farà automaticamente.
3. **Compila il Profilo:** Apri `profilo.md` e inserisci i tuoi dati (peso, altezza, età).
4. **Inizia a loggare:** Scrivi al tuo assistente: *"Oggi a pranzo ho mangiato 100g di pasta al pomodoro e un petto di pollo"* e guarda la wiki aggiornarsi da sola!

## 🤝 Contribuire
Questo è un progetto aperto! Se hai suggerimenti per migliorare le formule di calcolo o la struttura dei file, sentiti libero di aprire una Issue o una Pull Request.

---
*Creato con ❤️ per la salute e la produttività.*
