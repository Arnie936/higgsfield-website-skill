# Craft: Scroll-Konzepte, Design-DNA, Qualitäts-Gates

## Die 7 Scroll-Konzepte

Wähle genau EIN Konzept. Leitfrage: **Was BEDEUTET Scrollen für dieses Produkt?** Das Konzept muss zum Produkt passen, nicht zum eigenen Geschmack. Begründe die Wahl in einem Satz und lass sie den Nutzer im Interview bestätigen.

- **A — Ambient Loop:** Ein Hero-Objekt, das einfach schön aussieht; Video loopt, Scroll enthüllt Sektionen. Für Stimmung ohne Transformation (Restaurant, Atmosphäre).
- **B — Scroll Scrub:** Das Produkt rotiert oder transformiert sich mit der Scroll-Position (Canvas-Framesequenz). Der Klassiker für Orbits.
- **C — Cursor Spotlight:** Das Produkt wird per Cursor aus der Dunkelheit enthüllt. Für Mystik/Reveal.
- **D — Horizontal Pan Lock:** Vertikales Scrollen bewegt seitlich durch einen Ort oder ein Lineup. Für Kollektionen, Räume, Landschaften.
- **E — Exploded View:** Ein gebautes Objekt zerlegt sich beim Scrollen in seine Einzelteile — rückwärts scrollen setzt es wieder zusammen. Für alles mit Innenleben (Uhren, Audio, Maschinen). Der stärkste Effekt für Premium-Produkte mit Teilen.
- **F — Push Through:** Die Kamera fliegt beim Scrollen in einen Raum hinein. Für Immobilien, Interieurs, Journeys.
- **G — Scrollytelling:** Ein Prozess entfaltet sich Schritt für Schritt. Für Herstellung, Storys, Anleitungen.

Template-Hinweise: Luxury Product → E oder B · Journey/Real Estate → F · E-Commerce → B + Hover-Spins · Restaurant → A oder G · Automotive → B (gechainte Fahrt) · SaaS → G oder B · Agency → B (abstrakt) · Portfolio → B (Orbit).

## Scrub-Regel: Nur der Hero scrubbt

Genau EIN Clip — der Hero — wird an die Scroll-Position gekoppelt (Canvas-Framesequenz). Alle Stütz-Clips (Macro, Kontext, Orbit …) werden als normale, selbstlaufende Videos eingebaut: `<video muted playsinline autoplay loop>`, ggf. gedimmt hinter Copy. Begründung aus der Praxis: ein zweiter Scrub wirkt wie ein eingefrorenes Bild ("Video spielt nicht"), konkurriert mit dem Hero-Wow und macht die Seite zäh. Autoplay zusätzlich per ScrollTrigger-Fallback starten, falls der Browser es blockiert.

## Video-Gesetze (entscheidend für scrubbare Clips)

- Kamerabewegung auf die Scroll-Achse locken: kein Drift, kein zufälliger Zoom, konstante Geschwindigkeit. Bewegung stoppt nur, wenn der Nutzer die Zeit kontrolliert (Scrub).
- Bei Transformationen (Exploded View!): das START-Objekt muss dem END-Objekt gleichen — sonst als Loop zurückfallen.
- Alle Clips müssen sich wie Geschwister anfühlen: gleiche Produktidentität, Materialsprache, Lichtrichtung, Farbwelt. Nur Bewegung oder Framing ändern. Konsistenz schlägt Spektakel.

## Design-DNA (vor dem Bauen festlegen)

1. **These-Zeile:** Ein Satz, dem die gesamte Seite dient. Kurz, spezifisch, einprägsam — kein Marketing-Fluff.
2. **Szenen-Satz:** "Wer benutzt dieses Produkt, wo, in welchem Licht?" Daraus folgt hell oder dunkel.
3. **Palette aus der Szene, nicht aus der Branche:**
   - Nur OKLCH-Farben. Nie reines `#000` oder `#fff`.
   - Jedes Neutral leicht zur Markenfarbe tönen.
   - Genau EIN gesättigter Akzent; alles andere bleibt ruhig.
   - Chroma reduzieren, wenn Lightness gegen 0 oder 1 geht (sonst grell).
   - Vier Tokens: `--bg`, `--ink`, `--muted`, `--accent`.
4. **Typografie:** eine Display-Schrift für Headlines, eine saubere Body-Schrift. Lesbar zuerst, stylisch danach.

## Copywriting-Regeln

- Headlines kurz; Captions 3–5 Wörter mit einem Akzent-Wort.
- Jede Behauptung konkret genug, um falsifizierbar zu sein. Schlecht: "Smooth und lecker." Besser: "Zwei Drittel weniger Säure."
- Kein Spec-Sheet-Clutter, kein Feature-Dumping, kein Jargon, keine wiederholten Headings, keine Einleitung, die den Titel wiederholt, keine Gedankenstriche.

## Anti-AI-Verbotsliste (Hard Bans)

Die Seite ist durchgefallen, wenn jemand sie ansehen und sagen könnte: **"Das hat eine KI gemacht."** Vermeide:

- Gradient-Text · Glassmorphism · identische Card-Grids · riesige Fake-Hero-Metriken
- überstrapazierte SaaS-Layout-Klischees · verschwommene AI-Background-Blobs · zufälliges Neon
- Stock-Foto-Leere · bedeutungslose Icons · Platzhalter-Sektionen
- Hero-Text ohne weichen dunklen Halo (Text darf nie auswaschen)

Die Seite muss designt wirken, nicht generiert.

## Asset-Abnahmekriterien (vor dem Einbau prüfen)

Jedes generierte Asset visuell inspizieren, BEVOR es in die Seite kommt. Ablehnen und neu generieren, wenn:

- die Produktidentität sich ändert oder die Objektform inkonsistent wird
- das Material falsch aussieht oder das Asset offensichtlich KI-generiert wirkt
- das Video seltsames Morphing zeigt
- Text im Bild/Video auftaucht
- Hände, Labels, Logos oder Details kaputt sind
- der Stil nicht zur Website passt

## Erweitertes QA (zusätzlich zu den Basis-Checks)

- Der Hero bewegt sich schon VOR dem ersten Scroll.
- Kein Layout-Overlap, kein abgeschnittener Text, Kontrast ausreichend.
- Alle Assets laden; keine sichtbaren Platzhalter; keine mehrfach verwendeten Frames als Füller.
- Desktop-, Tablet- UND Mobile-Breite testen.
- Final Gate: Wirkt irgendeine Stelle "generiert"? Dann fixen, bis sie beabsichtigt, spezifisch und shippable wirkt.

## Abschlussbericht (Format für Phase 7)

1. Localhost-URL
2. These-Zeile
3. Gewähltes Scroll-Konzept + Ein-Satz-Begründung
4. Szenen-Satz
5. Palette-Tokens (OKLCH)
6. Verwendete Higgsfield-Prompts
7. Kurzliste des Gebauten
8. QA-Checkliste mit Pass/Fail
9. Offene Einschränkungen, falls vorhanden
