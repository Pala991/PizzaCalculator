# 🍕 Pizza Calculator

Calcolatore di dosi per l'impasto della pizza perfetta. Web app statica, leggera, installabile come PWA.

## Funzionalità

- **Modalità Farina**: inserisci i grammi di farina e scegli il tipo di impasto; il numero panetti viene calcolato automaticamente
- **Profili impasto in Da Farina**: Napoletana, Classica, Pinsa/Pinza, Teglia, Pala e **Custom** con peso panetto automatico
- **Preset locali**: salva, carica ed elimina ricette personalizzate direttamente dal browser (LocalStorage)
- **Modalità Teglie**: scegli formato e numero di teglie, calcola automaticamente la farina necessaria
- **Idratazione regolabile** (50-85%)
- **Sale regolabile** (1.5-4%)
- **Tempi di lievitazione** preimpostati (da 2h a 72h in frigo)
- **Lievito fresco o secco** con conversione automatica
- **Compensazione temperatura ambiente**: la dose di lievito si adatta automaticamente ai °C impostati
- **Condivisione pianificazione**: inoltro rapido con Web Share, bottone WhatsApp e copia testo per app Note/Promemoria
- **Promemoria locali**: notifiche browser su pieghe, uscita frigo e stesura con anticipo configurabile
- **Export avanzato**: PDF stampabile e download TXT/JSON della pianificazione
- **Storico impasti**: salvataggio prove con voto, note e foto opzionale
- **PWA**: installabile su smartphone come app nativa
- **Offline**: funziona anche senza connessione

---

## 🚀 Hosting gratuito — 3 opzioni

### Opzione 1: GitHub Pages (consigliata)

1. Crea un repository su [github.com](https://github.com/new)
2. Carica tutti i file (`index.html`, `manifest.json`, `sw.js`)
3. Vai in **Settings → Pages**
4. Sotto "Source" seleziona **Deploy from a branch** → branch `main`, cartella `/ (root)`
5. Clicca **Save**
6. Dopo qualche minuto il sito sarà live su: `https://tuousername.github.io/nome-repo/`

```bash
# Oppure da terminale:
cd PizzaCalculator
git init
git add .
git commit -m "Pizza Calculator v1"
git branch -M main
git remote add origin https://github.com/TUOUSERNAME/pizza-calculator.git
git push -u origin main
```

### Opzione 2: Netlify

1. Vai su [app.netlify.com](https://app.netlify.com)
2. Trascina la cartella `PizzaCalculator` nella pagina
3. Il sito sarà live istantaneamente con un URL tipo `https://random-name.netlify.app`
4. Puoi personalizzare il nome del sito dalle impostazioni

### Opzione 3: Vercel

1. Vai su [vercel.com](https://vercel.com)
2. Collega il tuo repository GitHub
3. Deploy automatico ad ogni push

---

## 📱 Installazione su smartphone

Una volta aperto il link del sito:

- **Android**: tocca il banner "Installa l'app" oppure dal menu ⋮ → "Aggiungi a schermata Home"
- **iOS**: tocca il pulsante di condivisione → "Aggiungi a schermata Home"

---

## 🧠 Cosa può mancare (consigli pratici)

Per far crescere l'app in modo utile, queste sono le priorità consigliate:

1. **Salvataggio ricette e preset locali**: completato.
2. **Storico impasti con note risultato**: completato con voto finale, foto e commento.
3. **Scalatura ingredienti per ingredienti disponibili**: esempio, "ho solo 4g di lievito, quanta farina/acqua posso usare?".
4. **Modalità multi-forno**: consigli tempi e temperature in base a forno domestico, elettrico professionale o pizza steel.
5. **Export avanzato**: completato con PDF stampabile e file TXT/JSON per backup o condivisione.
6. **Notifiche intelligenti**: completato con promemoria locali su browser.
7. **Gestione temperatura ambiente**: completato con input temperatura cucina e adattamento automatico del lievito.

---

## 📁 Struttura

```
PizzaCalculator/
├── index.html      # App completa (HTML + CSS + JS)
├── manifest.json   # Manifest PWA
├── sw.js           # Service Worker per cache offline
└── README.md       # Questo file
```

---

## Licenza

MIT — Usa liberamente!
