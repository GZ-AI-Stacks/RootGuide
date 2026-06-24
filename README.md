# RootGuide — Repo

Live-URL (Ziel): https://www.gz-ai-stacks.de/rootguide/ oder eigene Subdomain.

## Struktur

```
rg-repo/
├── index.html          # Landingpage (Verkaufsseite)
├── HANDBUCH.html       # Vollständiges Handbuch (18 Sektionen, Glossar, Troubleshooting)
├── agb.html            # AGB
├── widerruf.html       # Widerrufsbelehrung + Muster-Formular
├── datenschutz.html    # DSGVO-Erklärung
├── impressum.html      # Impressum (§ 5 DDG)
├── demo/               # (geplant) Demo-Version der App
├── img/                # Bilder/Screenshots (noch zu füllen)
└── digistore/          # Auslieferungs-Notizen (nicht öffentlich!)
```

## Stand 2026-06-23 (durch Claude vorbereitet)

- [x] Landingpage `index.html` mit Cyberpunk-Grow-Look (passend zur App)
- [x] AGB, Widerruf, Datenschutz, Impressum erstellt
- [x] Earlybird (19,90 €, limit 30) + Vollversion (29,90 €) Preiskarten vorbereitet
- [x] Buttons `aria-disabled="true"` mit „DEMNÄCHST"-Tag — **Digistore-URLs später einsetzen**
- [x] Update-Garantie: 3 Jahre (wie Handwerker-Web)
- [x] Positionierung: Indoor-Pflanzen & Hydroponik (neutral)
- [x] Walkthrough-Tour in App-`index.html` eingebaut (8 Schritte, Auto-Start beim ersten Öffnen, Tour-Button im Header)
- [x] HANDBUCH.html im App-Look erstellt — 18 Sektionen, Glossar (pH/EC/PPFD/DLI/VPD/NPK/...), 9 Troubleshooting-Boxen, Tastatur-Kürzel, PWA-Anleitung

## TODOs für Gee

1. **Digistore-Produkte anlegen** — Earlybird + Vollversion, dann die Checkout-URLs in `index.html` einsetzen (Grep nach `aria-disabled="true"` findet die 3 Buttons).
2. **Lizenz-Gate** in App `index.html` einbauen (Klartext im JS wie bei Survival-Kompass: Käufer-Code + Master-Code, localStorage-Key `rootguide_lizenz`).
3. **App-Screenshots** in `img/` legen und Platzhalter in `index.html` (Hero-Visual) durch echtes `<img>` ersetzen.
4. **Demo-HTML** in `demo/index.html` — abgespeckte Version ohne Lizenz-Inhalte.
5. **Repo erstellen** auf GitHub: `GZ-AI-Stacks/RootGuide` (analog Survival-Kompass) und Pages aktivieren.

## Verbotene Begriffe (Digistore-Compliance!)

In Verkaufstexten NIE: „für immer", „lebenslang", „dauerhaft", „unbegrenzt", „lifetime".  
Stattdessen: „jederzeit nutzen", „24/7-Zugang", „Einmalkauf — Updates 3 Jahre inklusive".

Vor Digistore-Antrag: `grep -i "lebenslang\|für immer\|dauerhaft\|unbegrenzt\|lifetime"` über alle HTMLs.

## Quellen

- App-Quelle: `C:\Claude Workspace\Rootguide\RootGuide-main\RootGuide-main\index.html`
- Vorlage Landingpage: `C:\Claude Workspace\sk-repo\index.html` (Survival-Kompass)
- Vorlage Rechtstexte: `C:\Claude Workspace\sk-repo\*.html`
