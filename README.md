# 🌍 Global Flag Challenge

Un quiz interattivo sulle bandiere del mondo, completamente client-side, senza dipendenze esterne e senza server. Scritto in HTML5, CSS3 e JavaScript vanilla puro.

---

## 🎮 Demo

> Apri `global-flag-challenge.html` direttamente nel browser — nessuna installazione richiesta.

---

## ✨ Funzionalità

### Gioco
- **160+ nazioni** nel database, nomi in italiano
- **50 domande** estratte casualmente ad ogni partita
- **3 livelli di difficoltà:**
  | Difficoltà | Opzioni | Layout | Moltiplicatore |
  |------------|---------|--------|----------------|
  | 🟢 Facile  | 4       | 1 col  | ×1             |
  | 🔵 Medio   | 8       | 2 col  | ×2             |
  | 🔴 Difficile | 12    | 3 col  | ×3             |

- **Punteggio:** +1 risposta corretta / −1 risposta errata
- **Cronometro** in tempo reale
- **Bandiere** renderizzate come emoji Unicode (nessuna richiesta di rete)

### Sistema di punteggio
Il rating finale usa una formula che bilancia precisione e velocità:

```
Rating = (Corrette² / 50) × Moltiplicatore × (1000 / Secondi) × 10
```

Il quadrato delle risposte corrette penalizza molto gli errori, rendendo la precisione più importante della velocità pura.

### Profili e Record
- **Nome giocatore** richiesto prima di ogni partita
- **Giocatori salvati**: i nomi precedenti sono selezionabili con un click
- **Record assoluto** salvato in `localStorage` con nome, rating, difficoltà, tempo e data
- Il record è visibile nella **home page** e nella **schermata risultati**
- Banner animato dorato quando si batte il record

---

## 🖥️ Design

- **Dark mode** con sfondo `#0f172a` e griglia animata
- **Glassmorphism** — card semi-trasparenti con bordi neon
- **Tema neon** — cyan, magenta, verde e oro
- **Font:** Orbitron (titoli) + Exo 2 (testo) via Google Fonts
- **Hover** sulla bandiera con zoom fluido e glow neon
- **Feedback visivo** immediato: verde per corretto, rosso per errato
- **Fully responsive** — layout ottimizzato per mobile e desktop

---

## 📁 Struttura

```
global-flag-challenge/
├── global-flag-challenge.html   # Tutta l'app in un singolo file
└── README.md
```

Nessuna dipendenza, nessun build step, nessun framework.

---

## 🚀 Come usarlo

### Localmente
```bash
git clone https://github.com/TUO-USERNAME/global-flag-challenge.git
cd global-flag-challenge
# Apri global-flag-challenge.html nel browser
```

### GitHub Pages
1. Vai su **Settings → Pages** nel repository
2. Seleziona il branch `main` e la cartella `/ (root)`
3. Salva — la pagina sarà disponibile su `https://TUO-USERNAME.github.io/global-flag-challenge/global-flag-challenge.html`

---

## 🛠️ Tecnologie

| Tecnologia | Uso |
|------------|-----|
| HTML5 | Struttura e semantica |
| CSS3 | Glassmorphism, animazioni, responsive layout |
| JavaScript ES6+ | Logica di gioco, localStorage, generazione dinamica |
| Unicode Regional Indicators | Emoji bandiere senza CDN esterni |
| Google Fonts | Orbitron + Exo 2 |
| localStorage | Salvataggio record e lista giocatori |

---

## 📸 Screenshot

| Splash / Home | Gioco | Risultati |
|---|---|---|
| Schermata iniziale con record e difficoltà | Card con bandiera e opzioni | Rating finale e confronto record |

---

## 📄 Licenza

MIT — libero di usare, modificare e distribuire.

---

*Fatto con ❤️ e un po' di geopolitica.*
