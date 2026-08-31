# 🌿 3D Garden

Modello 3D interattivo e fotorealistico di un giardino, ricostruito a partire da foto, video e planimetria reali.

Il progetto gira nel browser (nessuna installazione) ed è pensato per essere navigabile con il mouse, con texture PBR realistiche.

## 🔗 Anteprima live

> _Il link comparirà qui appena la webpage sarà online (GitHub Pages)._

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
- [ ] Raccolta materiale di riferimento (foto / video / planimetria)
- [ ] Scheletro scena 3D + webpage live
- [ ] Ricostruzione layout dalla planimetria
- [ ] Modellazione elementi (aiuole, piante, vialetti, arredi)
- [ ] Texture e illuminazione realistiche
- [ ] Rifinitura e ottimizzazione
