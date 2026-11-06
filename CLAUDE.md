# CLAUDE.md

geldmaepple: Das Repository ist noch leer (nur `README.md`). Tech-Stack und Struktur stehen noch nicht fest.

Sobald der Stack gewählt ist, diese Datei um die Abschnitte **Tech-Stack**, **Befehle**, **Struktur** und **stackspezifische Konventionen** ergänzen (Vorlage: die CLAUDE.md-Dateien der anderen Repos in `C:\_Repos`, z. B. `forstbetrieb-ecker` oder `framework`).

## Beim Projektstart

- Bei der Wahl des Stacks den Nutzer einbeziehen und nicht eigenmächtig festlegen.
- Von Anfang an: `.gitignore`, Lockfile, Formatter/Linter, ein Test-Setup und eine README mit Setup-Befehlen.
- TypeScript im `strict`-Modus bevorzugen, wenn es ein JS-Projekt wird.
- Geht es um Geldbeträge: als Integer in der kleinsten Einheit (Cent) oder mit einem Decimal-Typ rechnen, **nie mit Floats**. Währung immer mitführen, erst in der Anzeige mit `Intl.NumberFormat` formatieren.

## Arbeitsweise

- Lies vor dem Schreiben und folge bestehenden Mustern.
- Nur die gestellte Aufgabe lösen, kein Overengineering, keine spekulativen Abstraktionen.
- Keine neuen Abhängigkeiten ohne Begründung.
- Jede Änderung verifizieren (Tests, Build) und Ergebnisse ehrlich berichten.
- Keine Secrets im Code; Konfiguration über Umgebungsvariablen.
- Commits nach Conventional Commits (`feat:`, `fix:`, `refactor:`, `test:`, `docs:`, `chore:`).
