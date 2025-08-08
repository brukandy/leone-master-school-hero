# Leone Master School - Componente Sfere Interattive

Componente embeddabile per LearnWorld che permette di trascinare e muovere le tre sfere del logo Leone Master School. Disponibile in versione widget compatta e hero section fullscreen.

## 🎯 Caratteristiche

- **Drag & Drop**: Le sfere possono essere trascinate con il mouse o touch
- **Responsive**: Si adatta a dispositivi mobili e desktop
- **Embeddabile**: Progettato specificamente per LearnWorld
- **Senza dipendenze**: Solo HTML, CSS e JavaScript vanilla
- **Reset**: Pulsante per ripristinare le posizioni originali
- **Hero Fullscreen**: Versione che occupa tutta la hero section come sfondo
- **Animazioni**: Effetti di floating e transizioni fluide

## 📁 Versioni Disponibili

1. **`index.html`** - Versione standalone per test e sviluppo
2. **`leone-spheres-embed.html`** - Widget compatto per sezioni del corso
3. **`leone-hero-fullscreen.html`** - Hero section fullscreen (standalone)
4. **`leone-hero-learnworld.html`** - Hero section ottimizzata per LearnWorld

## 📱 Come Integrare in LearnWorld

### Per Widget Compatto (sezioni del corso)
1. Apri il tuo corso in LearnWorld
2. Aggiungi un blocco "HTML personalizzato" o "Codice HTML"
3. Copia tutto il contenuto del file `leone-spheres-embed.html`
4. Incolla il codice nel blocco HTML
5. Salva e pubblica

### Per Hero Section Fullscreen
1. Nella pagina principale del corso o landing page
2. Aggiungi un blocco "HTML personalizzato" all'inizio della pagina
3. Copia tutto il contenuto del file `leone-hero-learnworld.html`
4. Incolla il codice nel blocco HTML
5. Assicurati che non ci siano altri elementi sopra questo blocco
6. Salva e pubblica

### Metodo Alternativo: iFrame
1. Carica il file desiderato su un server web
2. In LearnWorld, aggiungi un blocco iFrame
3. Inserisci l'URL del file caricato
4. Imposta altezza appropriata (300px per widget, 80vh per hero)

## 🎨 Personalizzazione

### Colori
Per cambiare i colori delle sfere, modifica queste righe nel CSS:
```css
background: linear-gradient(135deg, #1e3c72 0%, #2a5298 100%);
```

### Dimensioni
Per cambiare la dimensione delle sfere:
```css
width: 60px;
height: 60px;
```

### Posizioni Iniziali
Le sfere partono in formazione triangolare. Per modificare le posizioni iniziali, cambia:
```css
.sphere:nth-child(1) { top: 50px; left: 50%; }
.sphere:nth-child(2) { top: 120px; left: 30%; }
.sphere:nth-child(3) { top: 120px; left: 70%; }
```

## 🔧 Funzioni JavaScript Disponibili

- `resetLeoneSpheresPosition()`: Ripristina le sfere alle posizioni originali
- `window.LeoneSpheresWidget.init()`: Reinizializza il widget se necessario

## 📱 Compatibilità

- ✅ Chrome, Firefox, Safari, Edge (versioni moderne)
- ✅ iOS Safari, Chrome Mobile
- ✅ Dispositivi touch
- ✅ Responsive design

## 🎓 Utilizzo Didattico

Questo componente può essere utilizzato per:
- Attività interattive di coordinazione
- Esercizi di problem solving
- Gamification dei contenuti
- Pause interattive durante le lezioni

## 🛠️ Risoluzione Problemi

**Le sfere non si muovono:**
- Verifica che JavaScript sia abilitato
- Controlla la console del browser per errori

**Il componente non appare:**
- Assicurati che LearnWorld supporti HTML personalizzato
- Verifica che tutto il codice sia stato copiato correttamente

**Su mobile non funziona:**
- Il componente supporta eventi touch, verifica la versione del browser

## 📄 Licenza

Componente creato per Leone Master School. Libero utilizzo per scopi educativi.
