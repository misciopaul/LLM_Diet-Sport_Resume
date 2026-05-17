# Istruzioni Diet & Sport Wiki

Questo file contiene le regole operative per la gestione automatizzata della wiki.

## Flusso di Lavoro Dietetico
1. **Input:** L'utente fornisce i pasti della giornata o di un singolo momento (es. "Ho mangiato pasta al forno").
2. **Calcolo:** Calcola calorie, proteine (g), grassi (g), carboidrati (g) e fibre (g) basandoti su stime medie affidabili per le porzioni indicate (o stimate se non specificate).
3. **Archiviazione:**
   - Individua la settimana corrente (formato `YYYY-settimanaWW`).
   - Cerca il file in `Diet/YYYY-settimanaWW.md`. Se non esiste, crealo.
   - Aggiungi o aggiorna la sezione relativa al giorno corrente (es. `## Lunedì 18 Maggio`).
   - Inserisci i dati in una tabella o lista strutturata per pasto (Colazione, Pranzo, Cena, Spuntini).
   - Includi un totale giornaliero di macro e calorie.

## Flusso di Lavoro Sportivo
1. **Input:** L'utente riporta un'attività fisica (es. "30 min di corsa lenta").
2. **Calcolo:** Consulta `profilo.md` per i dati corporei e stima le calorie bruciate (MET * peso * tempo).
3. **Archiviazione:**
   - Cerca il file in `Sport/YYYY-settimanaWW.md`. Se non esiste, crealo.
   - Aggiungi l'attività sotto il giorno corrispondente.
   - Includi: Tipo attività, Durata, Intensità stimata, Calorie bruciate.

## Gestione Profilo e Storico
- Ogni volta che l'utente aggiorna il peso o le circonferenze in `profilo.md`:
    1. Ricalcola automaticamente gli indicatori nella sezione "Indicatori Calcolati" di `profilo.md`.
    2. Aggiungi una nuova riga con la data corrente nel file `Misure_Corporee.md` per tracciare l'evoluzione.
- **Esortazione:** Almeno due volte al mese (indicativamente il 1° e il 15° del mese), se l'utente non lo ha fatto, ricordagli gentilmente di aggiornare i suoi dati corporei per mantenere i calcoli precisi.

## Manutenzione Index
- Quando crei un nuovo file settimanale in `Diet/` o `Sport/`, assicurati di aggiornare i link alla "Settimana Corrente" nel file `index.md`.

## Formattazione Obsidian
- Usa i Callout di Obsidian per evidenziare insight importanti.
- Mantieni i file puliti e leggibili.
