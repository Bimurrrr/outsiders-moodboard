# THE OUTSIDERS — HANDOFF (Stand 2026-06-02)

Übergabe für den nächsten Chat. Alles Wichtige + offene Threads + Arbeitsregeln.

---

## ⚠️ ARBEITSREGELN (diese Session hart gelernt — bitte einhalten)

1. **NIE selbst Bilder/Videos in Higgsfield generieren.** Das verbrennt Dreamers
   Credits. Dreamer hat unlimited, wenn ER den Knopf drückt. → **Nur PROMPTS
   liefern**, Dreamer generiert selbst (+ zieht seine Referenzen mit rein).
2. **Keine Multishot-Funktion** (kostet extra) — Shots **einzeln**.
3. **1K reicht** erstmal, **kein 4K-Upscale** (Dreamer scannt finale Shots
   später hoch). Bessere Erkennbarkeit → Figur größer im Frame komponieren.
4. **Story IMMER aus Finns Trello ziehen, NICHT erfinden.** (Erster Skript-
   Entwurf war frei erfunden = Fehlschlag.) Board: https://trello.com/b/LhCfx81d/the-outsiders
5. **Vor JEDEM Push JS-Check** (gerade `"`-Anführungszeichen in den Lore-Texten
   brechen das CAST-Array → ganze Seite tot). Check:
   `awk '/<script>/{f++} f==1 && !/<script>/ && !/<\/script>/{print} /<\/script>/{if(f==1)exit}' index.html > /tmp/s.js && node --check /tmp/s.js`
6. **Neue Char-Bilder immer als JPEG optimieren** (sips -Z 1400 q80), sonst
   lädt die Seite ewig.
7. Dreamer prüft am Live-Link, will Tempo, knappe Antworten, kein Bullshit.
   Deutsch, duzen. Format-Regel (#N-Blöcke) gilt.

---

## SEITE / DEPLOY

- **Live:** https://bimurrrr.github.io/outsiders-moodboard/
- **Repo:** `~/Code/outsiders-moodboard/` · GitHub Pages (main)
- **Deploy:** `git add . && git commit -m "…" && git push` → ~30 s live
- **Cache:** nach Push immer **Hard-Reload** (Cmd+Shift+R) erwähnen.
- Lokaler Vorschau-Server (Claude Preview) **zickt diese Maschine**
  (PermissionError sips/python http.server) → konnte nicht lokal rendern,
  via `curl` + `node --check` verifiziert + Dreamer testet live.

## SEITE — was gebaut ist (alles live)

- **18 Cast-Karten** als **Trading-Cards**: rounded, Bild-Rahmen, große
  #-Nummer (pink #), Holo-Sheen on hover, Stats-Box (Version·Style·♀/♂),
  Name fix auf 2-Zeilen-Höhe. Grid **fest 6 Spalten** (3×6=18), responsive 3/2.
- **Shuffle** bei jedem Reload (Fisher-Yates).
- **Modal** „ultrakrass": Karte poppt groß rein, **3D-Tilt zur Maus + Holo**,
  fette Lore rechts, Pills, **Download-Button** → lädt Karte als JPEG
  (Canvas, „outsiders-<n>-<name>.jpg") für Prompting + Fan-Sammlerei.
- **Nav** = floating Glass-Pill (zentriert, ohne „OUTSIDERS"-Wort).
- **Sound-Toggle** (Equalizer-Button u. rechts): verstecktes YouTube-Audio,
  **muted-Autoplay ab Load + Ton bei erster Geste** (Browser-Limit, mehr geht
  nicht). Song aktuell: **MSI „Stupid MF"** (YT `fzHui4ybChU`).
- **Bilder optimiert**: alle Cast → JPEG (1400px), Logo → JPEG. ~101 MB → 3 MB.
  Original-PNGs liegen unreferenziert im Repo als Backup.
- CI: schwarz, pink #ff2d95, gelb #f5e000, grün #00e88a, cyan #18c9ff, Film-Grain.
- **Hero-Format-Text korrigiert:** Querformat 16:9 / YouTube / 2–5 min (NICHT
  mehr vertikal/TikTok). Team: „Timur Akyol" (nicht Bimurrrr).

## CAST (18, in index.html CAST-Array)

✓ neuer Style · ⚠ = noch alter „editorial" Style, Restyle offen
01 X-Rat 🔒 (90s Skate, locked) · 02 Kawai ⚠ · 03 **Mr. Robinson** ✓ (hyperreal anthro-cat)
· 04 **Chico** ✓ (Chimp, war Zayn) · 05 Schaumi ✓ (Plush) · 06 **Fetch** ✓ (Low-Poly dog, war Rover)
· 07 Bobby Yellow ✓ (Plush) · 08 Cashy ⚠ · 09 Purrz ⚠ · 10 **Jojo** ⚠ (war Marso, →Style B Aardman geplant)
· 11 Krazy ⚠ · 12 Diabla ⚠ · 13 Onyx ✓ (Panther/Moncler `onyx_v3.jpg`) · 14 **Bunny & Angel** ✓ (Bratz v4, V2.0)
· 15 Bobby Girl ⚠ · 16 Spanky ✓ (war „JOLT") · 17 Baby Bizz ✓ · 18 Franky Deaky Joe ✓ (war „CLOUT")
- **Truffl wurde entfernt** (war #05), Cast neu durchnummeriert.
- **Style-Module A–H** für Restyles stehen im alten Chat (Charlie-Eth-Hall AI-Warped,
  Aardman-Clay, Felt-Puppet, Low-Fi-3D-on-footage, Daz3D-Y2K, Crochet, Bobblehead,
  Furry-Clay-Hybrid). Pinterest-Board für Refs: https://de.pinterest.com/akyoltimur/the-outsiders/

## SKRIPT — Episode 01 (`episode-01.md` + `.pdf`, v2)

**Basis = FINNS Trello-Konzept** (Karte „Erste Folge skripten" Kommentar
28.05 + „Random Story Ideen"). Struktur:
1. Cold Open: **2 Grafiker, echte Welt, cringe KI-Talk** (Finns Idee)
2. Anonyme **Main-Figur** kommt durch Flur ins Gebäude → Stuhlkreis (Fokus auf sie, Background-Hinweise)
3. Andere Figur (z. B. X-Rat) **teilt Geschichte** → Folge wird ihr **Flashback**
4. **Bruch:** zu emotional → aus dem Flashback zurück in den Kreis gerissen
5. **Cliffhanger:** Main-Figur hebt Kopf, spricht erstmals „Hallo, mein Name ist…"
- PDF für Finn: https://bimurrrr.github.io/outsiders-moodboard/episode-01.pdf
- **OFFEN (Finns Call):** Wer ist die Main-Figur? (Cast-Lore: X-Rat spricht erst
  am Ende → X-Rat = Main? Dann erzählt in Beat 3 jemand anderes.) Wessen Flashback?

## LOCATIONS (Dreamer generiert, Bilder in seiner Higgsfield-History)

- **Finaler Raum-Look = Mid-Century-LIMINAL** (60/70er: Holzpaneele, roter
  Teppich, Leucht-Rasterdecke, Designer-Stuhlkreis 8–9 Stühle KEINE Sessel,
  + Rand-Details Kaffeemaschine/Uhr/Pinnwand/Wasserspender). **NICHT** gelb-
  Meme-Backrooms, **NICHT** modern-minimalist (beide waren Fehlversuche).
  Raum-Wide ✅ sitzt. Prompt = #91 im alten Chat / unten als Vorlage.
- **Flur** ✅ generiert (Kubrick-Symmetrie, matcht Raum), X-Rat-Shots laufen.
- Refs kamen aus Dreamers Pinterest-Board (liminal meeting-rooms, monochrom).

## INTRO (`intro.html`, v2)

Logo unverändert, in 16 vertikale Streifen die schnell nacheinander von unten
reinschnappen (Y2K-Skate-Vibe), kein Glitch, gelber BG, kein Sound (legt
Dreamer drauf). https://bimurrrr.github.io/outsiders-moodboard/intro.html

## FILMPLAKAT (`Task offen`)

2 KI-Varianten generiert (Backrooms-Gruppe, Titel). Sollen **neu im finalen
Mid-Century-Raum** + später Dreamers **echte Figuren + echtes Logo** rein.

---

## 🎬 NÄCHSTER SCHRITT (Dreamers letzte Anfrage): mehr Shot-Prompts auf Basis des Skripts

Einzeln, 16:9, Mid-Century-liminal-Look, Dreamer generiert selbst + Char-Ref dazu.
Schon im alten Chat geliefert: 4 Flur-Shots (X-Rat von hinten / Beine-Close /
Medium / an der Tür). **Noch zu schreiben** (aus Skript v2):

- **Cold Open — 2 Grafiker:** nüchternes Grafikbüro, echte Welt, zwei Nerd-
  Grafiker am Mac, snobistisch über KI redend. Live-action-Look, Kontrast zur
  KI-Welt.
- **Ankunft — Main-Figur betritt Raum:** Tür von innen, Figur (anonym, von
  hinten/Schatten) tritt aus dem Flur in den großen Mid-Century-Saal.
- **Setzen:** Main-Figur von hinten, geht zum Stuhlkreis, nimmt Platz.
- **Raum-Wide BESETZT:** der Stuhlkreis mit mehreren Outsiders (Mixed-Media-
  Mix) — Master-Shot des Treffens.
- **Close erzählende Figur:** Close-up der Figur die ihre Story teilt (X-Rat?),
  emotional, im Kreis.
- **Flashback-Plates:** je nach gewählter Figur/Story (offen bis Finn klärt).
- **Bruch:** harter Rückschnitt zum Kreis, Figur überfordert.
- **Schluss-Cliffhanger:** Main-Figur **frontal**, hebt den Kopf, schaut in die
  Cam — „Hallo, mein Name ist…".

Raum-Prompt-Vorlage (v4, hat funktioniert): siehe `episode-01.md` Setting +
„Mid-Century liminal, Holzpaneele, roter Teppich, Leuchtrasterdecke, 8–9
Designer-Shell-Chairs im Kreis (keine Sessel), Rand-Props Kaffeemaschine/Uhr/
Pinnwand, vintage medium-format film, leer, 16:9, no people".

## Auch offen
- **Cinematic-Tool-Workflow:** Dreamer will ein Tool das alle Shots/Szenen auf
  einmal generiert (statt shot-by-shot). → klären WELCHES Tool, dann Skript als
  Szenen-/Shot-Liste auf dessen Input zuschneiden.
- Restliche **⚠-Chars restylen** (Kawai, Cashy, Purrz, Jojo, Krazy, Diabla, Bobby Girl).
- Filmplakat final. Onyx ist erledigt (onyx_v3 live).
