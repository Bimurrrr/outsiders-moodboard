# THE OUTSIDERS — Status / Handover

> Letzte Aktualisierung: 2026-06-01
> Projekt-Lead: Bimurrrr · Story: Finn Delius

## Was ist live

- **URL:** https://bimurrrr.github.io/outsiders-moodboard/
- **Repo:** https://github.com/Bimurrrr/outsiders-moodboard (public, main branch)
- **Hosting:** GitHub Pages (gh-auth via `gh` CLI — funktioniert ohne Cloudflare)
- **Lokal:** `/Users/bimurrrr/Code/outsiders-moodboard/`
- **Deploy-Workflow:** lokal editieren → `git add . && git commit -m "..." && git push` → ~30 Sek später live

## Die Serie — Kurzfassung

**Konzept:** Animated Series. Deprecated AI-Mascots treffen sich in der Selbsthilfegruppe „Outsiders Anonymous". Jeder hat eine Versionsnummer (wie AI-Models — V2.1, V3.6) und wurde ersetzt / gebannt / gecuttet / rug-pulled. Mixed-Media Stil-Mix ist Feature, nicht Bug.

**Vibe:** MTV-Trash-TV · Liquid Television · Wonder Showzen · Y2K · Punky · gesellschaftskritisch
**Format:** 2-Min Micro-Drama, vertikal, TikTok/Shorts-native
**Episode 1:** Selbsthilfegruppen-Treffen, ein Fremder kommt rein
**Premiere:** Winter 2026

## Cast — 16 Outsiders

| # | Name | Style | Trauma |
|---|------|-------|--------|
| 01 | X-Rat 🔒 | 90s Skate Cartoon (Master, locked) | Porn-Site-Mascot (X-Hamster-Parodie), EU-Bann 2024 |
| 02 | Kawai | Photoreal Kaiju Suit | Tokyo-Streetfashion-Pilot, nie ausgezogen |
| 03 | Mr. Pem | Photoreal AI Editorial | Britischer Luxury-Wool, casual Klassismus, Empire-Trauer |
| 04 | Zayn | Photoreal AI Editorial | Streetwear-Brand pleite, €40k Schulden, Consumerism |
| 05 | Truffl | Felt Sock Puppet | Kinder-TV gecancelt, parasoziale Krise |
| 06 | Schaumi | Hand-drawn Illustration | Waschanlagen-Mascot, Looksmaxxing-Stamm |
| 07 | Rover | Retro 8-Bit Pixel | Win-ME-Search-Agent, Spektrum/OCD |
| 08 | Bobby Yellow | Vintage 80s Mascot | Post-It-Pitch, identity-loss |
| 09 | Cashy | PS2 Low-Poly 3D | Arcade-Game discontinued, Memecoin-Crash |
| 10 | Purrz | Vintage Kawaii | Sanrio-Style, BPD, ED, permanent-lächeln-Trauma |
| 11 | Marso | Vintage 60s Cartoon | Belgisches Comic-Pilot, Dissoziation |
| 12 | Krazy | 90s Hanna-Barbera | Cancelled Antagonist, Tate-radicalized, Wut-Tränen |
| 13 | Diabla | Claymation | Adult-Swim-Pilot, Alkoholismus, AA-Dropout |
| 14 | Onyx | Anime Cel-Shaded | Crypto-NFT-Mascot, rug-pulled, Day-Trading-Grooming |
| 15 | Zelma & Zimmer | Y2K Bratz Doll Duo | Codependent toxic couple seit 2004 |
| 16 | Bobby Girl | Vintage 50s Cartoon | Bobby-Family, People-Pleaser-Burnout |

## Style-DNA (User-validated)

**Logo + CI:** Grün/Pink/Gelb aus Trello-Logo · Hero-Section komplett gelb
**Typo:** Anton + Archivo Black + JetBrains Mono (Inter für Body)
**Look:** schwarz BG · scharfe Edges · keine Verläufe · Marquees zwischen Sections · CRT/Noise subtil · Trading-Card-Layout

## ⚠ OFFEN — als nächstes dran

### Style-Push: Cast in „MTV-Trash-TV / Wonder-Showzen / Liquid Television"-Richtung optimieren

User hat 4 Refs gepostet die zeigen wohin: rauer, uncannier, weniger clean. Aktuelle Chars zu „editorial polished".

**Konkret zu redo (Vorschläge mit User-Sign-off pending):**
- **Diabla** → Freak-Clay (statt sauberes Aardman): schiefe Anatomie, Mörder-Zähne, raw plasticine
- **Mr. Pem** → Wax-Figure-Uncanny (AI-warped, „CANCEL ME"-energy)
- **Onyx** → AI-Warped Photoreal statt clean Anime-Cel
- **Bobby Boy NEU** → 3D-Caricature-Meme-Style (TikTok-meme-3D)
- **Marso** → komplett ersetzen durch Mascot-Suit-3D (McDonald's-Crew-vibe, pluschig laut)
- **Schaumi** → ersetzen oder rauer machen, geht aktuell im Grid unter
- **Bobby Yellow** → keep oder Mascot-Suit-3D-variant

**Refs für die Style-Push-Generationen** sind im aktuellen Chat (Stop-Motion Sun-Freak, 3D-Caricature-Black-Boy, McDonald's-Mascot-Crew, AI-Warped-„Cancel-Me"-Person). Falls neuer Chat: User fragen nach Re-Upload der Refs.

### Andere offene Punkte

- **Custom Domain `outsiders-mascots.com`** noch nicht gekauft. User wollte. WHOIS bestätigt verfügbar. Cloudflare-Registrar ~$10/Jahr. Sobald gekauft: CNAME zu `bimurrrr.github.io`.
- **Group-Shot / Klassenfoto** v2 fertig (`hf_20260531_225338_de1ca84e-...png`), aber Style-Drift noch nicht 100% — wartet auf Bestätigung ob als Hero-Banner einbauen oder weiter iterieren.
- **Episode 1 Skript** — noch nicht angefangen. Storyboard-Notes in Finns Trello-Karten (siehe „Random Story Ideen" + „Erste Folge skripten" im Trello).
- **Animation-Tests** mit Higgsfield — noch nicht gestartet. Plan: X-Rat als Personal-Clipper-Character locken, dann erste 5-Sek-Clips.

## Tools / Zugänge

- **Higgsfield:** MCP-Tool aktiv. Nano Banana Pro für Image-Gen. Max 14 image refs pro Call.
- **Trello:** "The Outsider(s)" Board, im Chrome eingeloggt unter User-Account
- **Pinterest:** Board "The Outsider(s)" 65+ Pins, im Chrome eingeloggt
- **Claude in Chrome:** Extension installiert, Browser-Automation funktioniert
- **Cloudflare:** Wrangler-Auth abgelaufen. Login-Flow via Browser-Automation hat nicht geklappt (Cloudflare-Dash hat Spinner-Stuck). Workaround: GitHub Pages.
- **GitHub:** `gh` CLI authed als Bimurrrr, hat repo+workflow+gist scopes

## File-Struktur

```
/Users/bimurrrr/Code/outsiders-moodboard/
├── index.html         # Promo-Page (live über GitHub Pages)
├── logo.png           # THE OUTSIDERS Bubble-Logo (von Trello)
├── cast/              # 18 Character-PNGs + couple-shot + cashy-v2
└── STATUS.md          # diese Datei
```

## Wichtige URLs

- Site live: https://bimurrrr.github.io/outsiders-moodboard/
- Repo: https://github.com/Bimurrrr/outsiders-moodboard
- Trello: https://trello.com/b/LhCfx81d/the-outsiders
- Pinterest Moodboard: https://de.pinterest.com/akyoltimur/the-outsiders/

## Tone-Notes für nächste Session

- User ist Dreamer / Bimurrrr, duzen, kurz und direkt, kein Bullshit
- Wenn User Frust hat → einfacher machen, nicht mehr Optionen aufmachen
- Style-Mix ist gewollt (jeder Char hat eigenen Render-Stil) — Style-Drift bei Group-Shots ist nervig, daher per-char strict prompting
- User mag knallige Headers + saubere Trading-Card-Layouts, KEINE billigen Drop-Shadows / Gradients
- MTV-Trash > Pixar-Clean
