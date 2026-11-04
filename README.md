# Rapport Generator

Der Rapport Generator erstellt kundenbezogene Arbeitsrapporte als PDF aus Terminen in einem Outlook- oder CalDAV-Kalender. Er hilft dabei, Arbeitszeiten, Material und weitere Kostenstellen aus den Terminangaben zu übernehmen und übersichtlich pro Kunde abzurechnen.

## Download

[**Aktuellen Windows-Installer herunterladen**](https://github.com/LuRo/Rapport-Generator-Releases/releases/latest/download/RapportGeneratorSetup.exe)  
[Alle verfügbaren Releases ansehen](https://github.com/LuRo/Rapport-Generator-Releases/releases)

## Hilfe
Über diese Seite kann man die Seite direkt anzeigen lassen: https://luro.github.io/Rapport-Generator-Releases/HILFE.html

## Was die App kann

- Termine aus einem frei wählbaren Zeitraum aus Outlook oder einem CalDAV-Kalender laden
- Kunden aus den Kalenderterminen erkennen und passende Einträge direkt anzeigen
- Kunden per Volltextsuche finden und einen oder mehrere Kunden auswählen
- Pro Kunde einen eigenen PDF-Rapport mit Arbeitszeiten, Material und Kosten erstellen
- Rapporte je nach Bedarf im Hoch- oder Querformat erstellen
- Tätigkeiten und verwendetes Material nach Tagen im Rapport ausweisen
- PDFs in der App ansehen, durchblättern und drucken
- Mitarbeiter, Materialien, Kostenstellen, Ansätze, Einheiten und PDF-Layout anpassen
- Einstellungen und PDF-Layout exportieren und auf einem anderen Gerät wieder importieren
- Beim Start automatisch nach einer neuen Version suchen oder die Suche manuell auslösen
- Fehlgeschlagene Verarbeitung mit zusätzlichen Angaben im Protokoll nachvollziehen

Die Bedienoberfläche ist auf Deutsch und Englisch verfügbar.

## Typischer Ablauf

1. Den Berichtszeitraum auswählen.
2. Die App lädt die dazugehörigen Kalendertermine und zeigt die gefundenen Kunden an.
3. Einen oder mehrere Kunden auswählen. Bei Bedarf die Volltextsuche zum Filtern verwenden.
4. Rapportoptionen wie Ausrichtung oder Tätigkeiten und Material pro Tag festlegen.
5. Die Rapporte erstellen, in der Vorschau kontrollieren und bei Bedarf drucken.

Die fertigen PDFs werden im eingestellten Ausgabeordner gespeichert.

## Angaben in Kalenderterminen

Die App liest Kunde, Arbeit und Abrechnungspositionen aus dem Betreff eines Termins. Das Standardformat lautet:

```text
<Kunde> -- <Arbeit> //<Kürzel>:<Menge>[:<Detail>]//<Kürzel>:<Menge>
```

Beispiel:

```text
Muster AG -- Fenster montieren //RG:2:Montage//TH:1.5//Auto:32
```

Dabei steht `Muster AG` für den Kunden und `Fenster montieren` für die Arbeit. Die Kürzel `RG`, `TH` und `Auto` werden den in der App eingerichteten Mitarbeitern, Materialien oder Kostenstellen zugeordnet. Mengen und Preise werden anhand der gespeicherten Einstellungen berechnet. Die Trennzeichen lassen sich anpassen.

Wenn Termine Tätigkeits- oder Materialbeschreibungen enthalten, kann der Rapport diese Positionen nach Tagen zusammenfassen und aufführen.

## Einstellungen und Datensicherung

In den Einstellungen lassen sich unter anderem folgende Angaben verwalten:

- Mitarbeiter und Materialien samt Kürzeln, Ansätzen und Einheiten
- Kostenstellen und die Trennzeichen für Kalenderbetreffzeilen
- Ausgabeordner, Dateinamen und Datumsformat
- PDF-Kopfzeile, Logo, Rapportfelder und Fusszeile
- Ausrichtung und weitere Rapportoptionen

Die Einstellungen und das PDF-Layout können gemeinsam als Paket exportiert und später wieder importiert werden. Ein verwendetes Logo wird mitgesichert. Das CalDAV-Passwort ist aus Sicherheitsgründen nicht Bestandteil des Pakets und muss nach einem Import erneut eingegeben werden.

Bei der Deinstallation fragt der Installer, ob eine Sicherung der Einstellungen im Downloads-Ordner erstellt werden soll. Bereits erstellte Rapporte im Ausgabeordner werden durch die Deinstallation nicht gelöscht.

## Kalenderzugriff

- **Outlook:** Benötigt eine eingerichtete Microsoft-Outlook-Desktopanwendung.
- **CalDAV:** Benötigt die HTTPS-Adresse des Kalenders sowie ein gültiges Passwort oder App-Passwort.

Während Kalenderdaten geladen und Rapporte verarbeitet werden, zeigt das Protokoll den Fortschritt und bei Problemen zusätzliche Informationen an.

## Aktualisierungen

Die App prüft beim Start automatisch auf eine neue stabile Version. Diese Prüfung kann in den Einstellungen deaktiviert werden. Über **Nach Updates suchen** lässt sich jederzeit eine manuelle Prüfung starten.

Ein Update wird erst nach Zustimmung heruntergeladen. Unter Windows wird der vollständige Installer im Downloads-Ordner abgelegt und von dort gestartet.
