# Verhaltenskonzept Jahrgang 5/6 — „Zeit gewinnen statt Zeit verlieren"

Gesamtschule NRW · Konferenzvorlage, Einführungsfahrplan und druckfertiges Material.
Die Unterlagen liegen zusätzlich als Website vor, damit Kollegium und Eltern sie ohne Dateidownload öffnen können.

**Website: https://ryze-o.github.io/verhaltenskonzept-5-6/**

## Der Kern in drei Sätzen

Zwei der drei bestehenden Systeme erfassen einzelne Kinder namentlich, öffentlich und ausschließlich negativ; das einzige positive erfasst die Klasse. Der Vorschlag dreht diese Schieflage um, indem das KlasseKinderSpiel den Zeitfresser-Strahl ablöst und den bestehenden Zeitsparer nach einer klaren Regel füllt. Damit kommt kein System hinzu — es fällt eines weg.

## Website (wird von GitHub Pages ausgeliefert)

| Seite | Für wen |
|---|---|
| `index.html` | Startseite mit Übersicht |
| `konzept.html` | Konzeptpapier, 14 Kapitel — Konferenz und Schulleitung |
| `kurzfassung.html` | Eine Seite: was sich für mich als Fachlehrkraft ändert |
| `materialpaket.html` | Sieben druckfertige Bögen, direkt aus dem Browser druckbar |
| `fahrplan.html` | Sechs-Wochen-Fahrplan inkl. Skript für die Einführungsstunden |
| `elternbrief.html` | Elternbrief zum Ausfüllen und Ausdrucken |
| `kommunikation/schuelerinfo.html` | Kindgerechte Erklärung für die Klasse |
| `quellen.html` | Alle Belege mit geprüften Links |
| `assets/site.css` | Gemeinsames Stylesheet |

## Einzelne Druckbögen

Im Ordner `material/`. Alle im Browser öffnen und mit <kbd>Strg</kbd>+<kbd>P</kbd> drucken.
Die Hintergrundfarben drucken automatisch mit (`print-color-adjust: exact`), die Checkbox
„Hintergrundgrafiken" muss niemand mehr suchen.

**Jeder Bogen ist auf exakte Seitenzahl geprüft** (Headless-Chromium, Seitenformate aus dem
erzeugten PDF ausgelesen). Stand: alle sieben Bögen paginieren korrekt.

> **Eine Einschränkung bei `materialpaket.html`:** Weil dieses eine Dokument A4 hoch, A4 quer
> und A3 mischt, erzeugt Chromium prinzipbedingt **eine leere erste Seite**. Im Druckdialog
> deshalb **Seiten 2–11** eingeben. Beim Druck der Einzeldateien aus `material/` tritt das
> nicht auf — dort stimmt jede Seite. Das ist eine Eigenheit der Browser-Druckengine bei
> gemischten Papierformaten, kein Fehler im Dokument.

| Datei | Format | Zweck |
|---|---|---|
| `erfassungsbogen_woche.html` | A4 quer | Das Arbeitspferd, ein Blatt pro Klasse und Woche |
| `klassenposter_regeln.html` | A3 | Regeln, von den Kindern selbst einzutragen |
| `verstaerker_menue.html` | A3 | Preisliste, mit der Klasse auszuhandeln |
| `abgrenzung_ampel_gbg.html` | A4 | Wann Ampel, wann Spiel — fürs Lehrerzimmer |
| `ampel_neu.html` | A4 | Überarbeitete Ampel + Sichtschutz-Klappe |
| `verhaltensvereinbarung_tagesrueckmeldung.html` | A4 | Baustein 3 + Tageskarten zum Ausschneiden |

## Markdown-Quellen

Die Langtexte liegen zusätzlich als Markdown vor — bequemer zum Weiterschreiben, und GitHub
zeigt sie direkt im Repo an:

```
konzept/Belohnungskonzept_Jg5-6.md     Hauptdokument
konzept/Kurzfassung_Kollegium.md       Kurzfassung fürs Kollegium
einfuehrung/fahrplan_6_wochen.md       Einführungsfahrplan
kommunikation/elternbrief.md           Elternbrief
quellen/literatur.md                   Quellenverzeichnis
```

Wer etwas ändert, sollte es **in beiden** Fassungen tun — Markdown und HTML werden nicht
automatisch synchronisiert.

## Vor der Konferenz zu erledigen

1. **Alle `[ANPASSEN: ...]`-Stellen füllen.** Vor allem Datum, Namen, Reset-Rhythmus der Ampel und ab wann Eltern informiert werden.
2. **Baseline-Daten erheben** — Auszeitraum-Verweise, Zeitfresser, Zeitsparer-Minuten, Ampel Rot, jeweils pro Woche über die letzten vier Wochen. Kostet eine halbe Stunde und entscheidet darüber, ob die Evaluation nach dem Halbjahr überhaupt etwas aussagt.
3. **Konzept der schulischen Datenschutzbeauftragten vorlegen.** Die Aussagen zu VO-DV I in Kapitel 7 sind recherchiert, aber keine Rechtsauskunft.
4. **Druckprobe machen.** Jeden Bogen einmal in der Druckvorschau ansehen.

## Sichtbarkeit

Die Seite trägt `robots.txt` und `<meta name="robots" content="noindex,nofollow">`, ist also
für Suchmaschinen gesperrt. Wer die URL hat, kann sie dennoch öffnen — GitHub Pages kennt
keinen Passwortschutz. Keine Schülernamen und keine personenbezogenen Daten in dieses Repo.

## Änderungen veröffentlichen

```bash
git add -A
git commit -m "Beschreibung der Änderung"
git push
```

Nach etwa einer Minute ist die Website aktualisiert.
