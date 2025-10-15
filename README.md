# Portfolio Analyzer 📈

Uno strumento Python pensato per l'analisi approfondita di portafogli di investimento. Esegue una decomposizione ("look-through") degli ETF per svelare le sovrapposizioni nascoste, visualizza l'esposizione di mercato reale, stima il rischio potenziale tramite simulazioni Monte Carlo ed esporta report dettagliati in Excel.

---

### Cosa Fa in Pratica?

* **Spacchetta gli ETF:** Prende un ETF e trova le azioni che contiene.
* **Mostra le sovrapposizioni:** Ti fa vedere se hai la stessa azione in più posti (es. comprata singolarmente e dentro un ETF).
* **Calcola l'esposizione reale:** Unisce tutto e ti dice la percentuale vera del tuo portafoglio per ogni paese e settore (es. 15% USA, 10% tech).
* **Esporta un report in Excel:** Crea un file Excel pulito con tutti i risultati.

---

### Come Funziona (I Passaggi Logici)

1.  **Input:** Fornisci la lista dei tuoi ticker (azioni/ETF) e le quantità.
2.  **Analisi:** Per ogni ticker, il codice capisce se è un'azione o un ETF. Se è un ETF, ne estrae le componenti. Per ogni azione, recupera dati come settore e paese.
3.  **Aggregazione:** Tutti i dati vengono uniti. Se hai Apple sia direttamente che in due ETF, il codice somma tutto e ti dà il valore totale che possiedi di Apple.
4.  **Output:** I risultati finali vengono mostrati in una semplice dashboard web e salvati in un file Excel.

---

### Strumenti Utilizzati

* **Python**
* **Pandas** per gestire i dati
* **yfinance** per i dati di azioni e prezzi
* **requests** e **BeautifulSoup4** per "leggere" le pagine web degli ETF
* **Streamlit** per la dashboard web
* **openpyxl** per scrivere i file Excel

---

### Roadmap (Cose da Fare)

- [ ] **1. Scrivere la funzione per "spacchettare" un ETF.** (Il primo passo, il più importante)
- [ ] **2. Creare la logica per aggregare i dati di un intero portafoglio.**
- [ ] **3. Costruire la dashboard e la funzione per esportare il report Excel.**
- [ ] **4. (Opzionale) Aggiungere la simulazione Monte Carlo per l'analisi del rischio.**
