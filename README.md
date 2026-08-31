# 🌿 3D Garden

Modello 3D interattivo e fotorealistico di un giardino, ricostruito a partire da foto, video e planimetria reali.

Il progetto gira nel browser (nessuna installazione) ed è pensato per essere navigabile con il mouse, con texture PBR realistiche.

## 🔗 Anteprima live

- **Aggiornata ad ogni iterazione (istantanea):** https://claude.ai/code/artifact/5762de8c-1595-4869-8e9b-429d183250a0
- **Il tuo dominio (GitHub Pages):** da attivare una volta sola — vedi sotto.

### Attivare GitHub Pages (il tuo dominio personale)
1. Vai su **Settings → Pages** del repo
2. In *Source* scegli **Deploy from a branch**
3. Branch: `claude/garden-3d-model-hqb1n1`, cartella `/ (root)` → **Save**
4. Dopo ~1 minuto il giardino sarà su `https://matte9826.github.io/3D-Garden/`

> La scena è un unico file `index.html` (Three.js da CDN): funziona anche aprendola in locale con doppio clic.

## 📁 Come caricare il materiale di riferimento

Metti foto, video e planimetria nelle cartelle dentro `reference/`, così vengono usate come base per ricostruire il giardino:

```
reference/
├── planimetria/   → la piantina del giardino (foto o PDF)
├── foto/          → foto singole (rinomina se puoi: aiuola-nord.jpg, vialetto.jpg, ...)
├── video/         → solo video leggeri/compressi (i pesanti condividili via link)
└── note.txt       → misure reali, orientamento (nord), materiali, note
```

### Consigli utili
- **Rinomina le foto** con nomi parlanti: aiutano a capire cosa sto guardando.
- **Le misure reali** (lunghezze vialetti, dimensioni aiuole, altezze piante/muri) sono fondamentali per la scala corretta.
- **Indica dov'è il nord**: serve per orientare luce e ombre in modo realistico.
- **Video pesanti (>100 MB)**: non caricarli nel repo, condividi un link (Google Drive / YouTube non in elenco).

## 🛠️ Stack tecnico (previsto)

- **Three.js** — motore 3D nel browser, interattivo
- **GitHub Pages** — hosting della webpage sempre aggiornata
- **Texture PBR** — erba, pietra, legno, foglie per un aspetto realistico (non cartoon)

## 📌 Stato del progetto

- [x] Setup repository e struttura cartelle
- [x] Raccolta materiale di riferimento (22 foto + 2 video + planimetria catastale)
- [x] **v0.1 — Scheletro 3D navigabile + webpage live** (villa, ala rosa, torretta, nocciolo, oleandri, cipressi, pino, palme, siepi, muro a secco, vialetto, corrimano, nastro di cantiere; sole regolabile; modalità orbita/cammina)
- [ ] v0.2 — Layout in scala reale dalla planimetria (con misure + orientamento nord)
- [ ] v0.3 — Texture fotografiche reali estratte dalle foto (intonaci, pietra, foglie)
- [ ] v0.4 — Chiome realistiche (foglie vere) e prato dettagliato
- [ ] v0.5 — Arredi, dettagli, ottimizzazione mobile

### Controlli
- **Orbita** (default): trascina per ruotare, rotella per zoom, tasto destro per spostarti
- **Cammina**: pulsante *Cammina* → `W A S D` + mouse, `Esc` per uscire
- **Ora del giorno**: slider in alto a destra (dall'alba al tramonto)
- **Punti di vista**: i pulsanti in basso a destra
