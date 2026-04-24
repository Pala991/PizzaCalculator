# AGENTS - PizzaCalculator

## Obiettivo

PWA per calcoli di impasto con persistenza locale, pianificazione fermentazione, storia e notifiche.

## Regole architetturali

1. Vanilla JS, HTML, CSS — niente framework pesanti
2. LocalStorage per persistenza dati (presets, history, settings)
3. Service Worker per offline-first experience
4. Notifiche browser per reminder fermentazione
5. Export in PDF, TXT, JSON per archivio pianificazione
6. Calcoli deterministici: stessa input → stessa output (no random, no tempo)
7. **Cache busting**: Dopo ogni modifica che viene pushata, incrementare il `CACHE_NAME` nel `sw.js` (es. `v4` → `v5`) per forzare il refresh del Service Worker e impedire che i client continuino a servire versioni vecchie

## Comandi utili

```bash
# Sviluppo locale
open index.html

# Deploy (GitHub Pages già configurate)
git push origin main

# Dopo ogni push, incrementare sw.js:
# CACHE_NAME = 'pizza-calc-vX' dove X = versione precedente + 1
```

## Features implementate

- ✅ Presets ricette (save/load/delete)
- ✅ Pianificazione fermentazione con timeline
- ✅ Notifiche browser con lead-time configurabile
- ✅ Storia impasti con rating e foto
- ✅ Compensazione temperatura ambiente
- ✅ Export PDF/TXT/JSON

## Note importanti

- Il PWA rimane disponibile offline, ma nuove versioni richiedono reload del SW
- Sempre incrementare versione cache quando si modifica `index.html`
- I preset e history sono salvati in LocalStorage — il clear cache del browser rimuove tutto
