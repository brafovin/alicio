# Mampf Royale

Ein 3D-Browserspiel: Lauf über die Straßen einer Insel, sammel Essen ins Inventar und futter es von dort.
Mit jedem Level wirst du fetter – bis du auf Level 10 so groß bist wie die ganze Map.

## Spielen

`index.html` im Browser öffnen (Doppelklick reicht). Beim ersten Start wird die 3D-Grafik
(three.js) aus dem Internet geladen, danach läuft alles lokal im Browser. Der Spielstand wird
automatisch im Browser gespeichert.

Die Grafik ist auf realistisch getrimmt: physikalisch korrektes Licht mit echtem Himmel und
Sonnenstand, spiegelnde Glasfassaden, weiche Schatten, Fototexturen (Asphalt, Gehwegplatten,
Rasen, Backstein, Dachziegel) und eine menschliche Spielfigur, deren Bauch mit jedem Level
wächst. Alle Texturen werden beim Start im Browser erzeugt – es gibt keine Bilddateien.
Am flüssigsten läuft es auf einem Rechner mit Grafikkarte in Chrome, Edge oder Firefox.

## Regeln

| Essen          | Punkte | Hinweis                                    |
| -------------- | -----: | ------------------------------------------ |
| 🍕 Pizza       |  5.000 | liegt überall auf den Straßen              |
| 🥙 Döner       |  2.000 | liegt überall auf den Straßen              |
| 🦖 Dinosaurier |  5.000 | selten, läuft herum (oft im Dino-Dschungel) |

- **200.000 Punkte = 1 Level**, Level 10 ist das Maximum.
- Essen sammelst du ein, indem du darüber läufst. Es landet im **Inventar**.
  Punkte gibt es erst, wenn du es **aus dem Inventar isst**.
- Das Inventar hat ein Limit (Level 1: 20 Sachen, verdoppelt sich mit jedem Level).
- Mit jedem Level wirst du dicker und größer:
  - ab **Level 4** walzt du kleine Häuser platt,
  - ab **Level 5** sitzt du im **Rollstuhl**,
  - auf **Level 10** bist du so breit wie die ganze Insel (2,4 km).
- Die Insel ist 2,4 × 2,4 km groß – ungefähr so groß wie eine Fortnite-Map – mit Orten wie
  Fette Türme, Pizza-Park, Döner-Dorf und Dino-Dschungel.

## Steuerung

| Taste                     | Aktion                          |
| ------------------------- | ------------------------------- |
| `W A S D` / Pfeiltasten   | laufen                          |
| `Shift`                   | sprinten                        |
| Maus ziehen / Mausrad     | Kamera drehen / zoomen          |
| `1` `2` `3` / Slot klicken | Pizza / Döner / Dino essen     |
| `E` (halten)              | ausgewähltes Essen weiteressen  |
| `F`                       | ganzes Inventar futtern         |
| `K`                       | große Karte                     |
| `M`                       | Ton an/aus                      |
| `Esc`                     | Pause                           |

Auf dem Handy: links wischen = laufen, rechts wischen = Kamera, Slots antippen = essen.

## Werte ändern

Alle Spielregeln stehen oben im Skript in `index.html` (Abschnitt „Spielregeln“), z. B.
`FOOD` (Punkte pro Essen), `LEVEL_PTS` (Punkte pro Level), `CHAIR_LEVEL` (ab wann Rollstuhl)
und `N_PIZZA` / `N_DONER` / `N_DINO` (wie viel Essen auf der Insel liegt).
