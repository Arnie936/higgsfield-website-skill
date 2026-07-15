# Die 10 Website-Templates

Jedes Template definiert: Shot-Struktur (Clips), Website-Sektionen, Design-Richtung, Copy-Ton. Das Scroll-Konzept (A–G) wird separat und bewusst gewählt — siehe `craft.md`, dort steht auch die Template→Konzept-Zuordnung (z.B. Luxury Product → Exploded View oder Scroll Scrub). Marken-/Beispieldaten sind Platzhalter — durch die Angaben des Nutzers ersetzen. Gemeinsame Defaults: Seedance 2.0, std mode, 16:9 (außer angegeben), kein Audio, ~8s pro Clip, Hero-Bild als Referenz in jedem Clip, Lenis smooth scroll, Scroll-Scrub-Hero als Canvas-Framesequenz. Nur der Hero scrubbt — alle Stütz-Clips als normale Autoplay-Loops einbauen (siehe Scrub-Regel in craft.md).

## 01 · Luxury Product (Uhren, Schmuck, Audio, Sneaker — Premium-Produkte)
- Clips: HERO ORBIT (360°-Studio-Turntable im schwarzen Void, Rim-Light) · MACRO FLY-THROUGH (extreme Nahaufnahme über Details) · EXPLODED ASSEMBLY (Produkt setzt sich aus schwebenden Einzelteilen zusammen)
- Sektionen: Hero mit Markenname tracking-in → Story → Macro-Details (Scrub Clip 2) → Exploded-View mit Spec-Callouts → Edition/Preis → Waitlist-CTA
- Design: Off-Black, Gold-Akzent, kontrastreiche Serif-Display + minimale Sans. Copy: leise, teuer, sehr wenige Worte.

## 02 · Journey (Erlebnisse, Tourismus, Expeditionen, Museen — Scroll = Reise)
- Clips: 5 gechainte Etappen (z.B. Oberfläche → Zonen → Ziel). KRITISCH: in Reihenfolge generieren, letztes Frame = start_image des nächsten, alle zu EINEM nahtlosen Scrub konkatenieren.
- Sektionen: fixes HUD (z.B. Tiefen-/Höhenmesser mit Scroll-Fortschritt), pro Zone eine gepinnte Sektion mit einem Fakt → Specs → Preis/Termin → CTA
- Design: Farbverlauf mit der Reise (z.B. Navy → Schwarz), ein leuchtender Akzent, dünne technische Sans mit HUD-Details.
- Funktioniert auch für: Bergaufstieg, Raketenstart, Höhlentour, Fabrik-Rundgang.

## 03 · Personal Portfolio (Creator, Freelancer, Berater) — Input-Foto nötig!
- Identitätsreferenz: Nutzerfoto auf JEDE Generierung; Garderobe konstant halten. 2–3 Takes des Hero-Orbits, den mit stabilster Likeness behalten.
- Clips: HERO ORBIT (Person, Arme verschränkt, 360°-Orbit, Rim-Light) · THE BUILDER (am Schreibtisch mit holografischen Screens, Push-in) · THE CLOSER (geht auf Kamera zu, Hero-Pose)
- Sektionen: Name in massivem Display-Type letter-by-letter → Stats-Strip mit Count-up → drei Pillars/Angebote über Clip 2 → Work-Cards über Clip 3 → CTA + Socials
- Design: Ink-Black, ein Akzent (z.B. Emerald), Creme-Typo, Bold Condensed Display, Kinetic Type, Grain.

## 04 · E-Commerce / Drop (Fashion, Merch, Limited Releases)
- Clips: HERO 16:9 (Model läuft durch Szenerie auf Kamera zu) · PRODUCT SPINS (je Produkt ein 1:1-Turntable-Clip) · FABRIC MACRO (Nähte, Details)
- Sektionen: Hero-Scrub + Countdown zum Drop → Produkt-Grid, Spin-Clips per Hover-Autoplay, Preis/Size-Selector/Add-to-Cart (Demo-Checkout ok) → Quality-Manifesto über Macro → Sticky Cart, Marquee-Strips, "Notify me"-Capture
- Design: z.B. Beton-Grau + Matt-Schwarz, ein Akzent, brutalistisch-kondensierte Typo.
- Für echte Stores: echte Produktfotos als Referenzen.

## 05 · Restaurant / Local Business (Restaurants, Cafés, Bars)
- Clips: HERO (Slow-Motion-Macro des Signature-Elements, z.B. Steak über Flamme) · THE ROOM (Dolly durch den Gastraum, Golden Hour) · THE CRAFT (Overhead: Anrichten, Dampf)
- Sektionen: Full-bleed Hero + Claim → Story → Menü zweispaltig, edle Typo → Private Dining → Öffnungszeiten + Karte + Reservierungs-CTA mit Datum/Personen-Formular
- Design: Fast-Schwarz, warmes Creme, Glut-Akzent, Film Grain, langsame Parallax. Copy: sparsam, sinnlich. Mobile: Menü einspaltig.
- Verkaufsfähig an echte Lokale: echtes Menü + echte Food-Fotos als Referenzen.

## 06 · Real Estate (Makler, Developer, Ferienwohnungen, Hotels)
- Clips: THE APPROACH (Drohne um das Gebäude, Dusk) · dann 2–4 gechainte Innen-Clips (Ankunft → Flow durch Räume → Terrasse/Highlight) als eine kontinuierliche Tour
- Sektionen: Hero-Claim → Fakten-Strip (Zimmer/Fläche/Features) → Galerie → Amenities mit Reveals → Preis → "Private Showing"-Formular mit Agent-Card; fixer Fortschritts-Indikator, der Räume beim Vorbeiscrollen benennt
- Design: Ink, Champagner-Gold, dünne elegante Serif, viel Weißraum.
- Für echte Listings: echte Fotos als start_frames — Seedance macht aus Stills cinematische Bewegung.

## 07 · Automotive / Big Product (Fahrzeuge, Drohnen, Bikes, Maschinen)
- Clips (gechained): REVEAL (Produkt in Umgebung enthüllt) · THE RUN (Tracking bei Fahrt/Bewegung) · ENVIRONMENT (anspruchsvolles Terrain) · NIGHT MODE (nur Lichtsignatur)
- Sektionen: Hero in Ultrawide-Type → Performance-Stats mit Count-up → Design-Sektion mit Macro-Stills → Night-Mode → Konfigurator-Teaser (Farboptionen recoloren ein Hero-Still) → Reserve-CTA; Tacho-HUD synchron zum Scroll
- Design: Black on Black, ein elektrischer Akzent, Ultrawide Condensed, Motion-Blur-Übergänge.

## 08 · SaaS / App (Software, KI-Tools, Startups)
- Clips: HERO (Datenpartikel formen sich zum schwebenden Dashboard-UI) · THE SIGNAL (Macro über holografische Charts, eine Anomalie leuchtet auf) · THE CALM (Produkt auf Laptop im hellen Office)
- Sektionen: Hero-Scrub (Dashboard baut sich beim Scrollen) + Claim + "Start free" → Logo-Strip → 3 Feature-Blöcke gepinnt über Clip 2 → Metrik-Counter → Screenshot in Browser-Mockup → Pricing (3 Tiers, Mitte hervorgehoben) → FAQ-Accordion → Final-CTA über Clip 3
- Design: dunkler Hero, der ins Weiß des Bodys übergeht, ein Akzent, geometrische Sans. Feature-Blöcke individuell layouten — keine identischen Card-Grids, kein Glassmorphism (siehe Anti-AI-Verbotsliste in craft.md).
- Credibility-Combo: generierter Hero + echte Produkt-Screenshots.

## 09 · Agency / Studio (Agenturen, Studios, Produktionsfirmen)
- Clips: HERO (abstrakt-atmosphärisch, z.B. Tinte in Wasser mit Gold-Flashes) · THE WORK (Showreel: Poster/Screens gleiten vorbei) · THE PEOPLE (Team-Silhouetten im Studio)
- Sektionen: Riesiger Markenname (80% Viewport) über Hero-Scrub, Manifesto tippt sich → kinetische Manifesto-Sektion (pro Scroll-Step knallt EIN Wort) → Work-Grid mit Hover-Video-Reveals → Services editorial zweispaltig → Team → Oversized-Footer-CTA
- Design: Schwarz + Bone-White, Akzentfarbe exakt 3× auf der ganzen Seite, Brutalist Display + edle Serif, Custom-Cursor (Punkt + Trailing-Ring).

## 10 · Gym / Fitness (Gyms, Coaches, Kampfsport, Sportmarken)
- Clips: HERO (Slow-Motion-Signature-Moment, z.B. Chalk-Cloud im Lichtschacht) · THE IRON (Macro Equipment/Griff) · THE GRIND (Athlet in Bewegung, tiefe schnelle Kamera)
- Sektionen: Hero + Motto punching-in → Philosophie (ein Satz pro Scroll-Step) → Programm-Grid mit Hover → Coaches-Cards → Results-Counter → Pricing (3 Tiers, "First week free") → Stundenplan + Karte + Anmeldeformular
- Design: Charcoal, Bone-White, ein Blutrot-Akzent, Heavy Condensed, Grain + Vignette. Mobile: Programme als Swipe-Cards.

## Eigene Struktur (kein Template passt)
Baue nach demselben Muster: 1 Hero-Clip (Orbit, Reveal oder Journey-Start) + 2–4 Stütz-Clips (Macro/Detail, Kontext/Raum, Mensch/Emotion), Hero-Bild als Referenz überall, Scroll-Scrub-Hero, 5–8 Sektionen mit einem klaren CTA, dunkle Basis + genau ein Akzent, wenig Copy.
