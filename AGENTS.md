# ApplePulp Releases

- `ApplePulp.setup.exe` ist ein mit NSIS erstellter Installer. Er lädt bei der Ausführung das jeweils als `latest` markierte GitHub-Release herunter und sucht dort nach einem Asset namens `ApplePulp.zip`.
- Jedes neue reguläre Release muss daher `ApplePulp.zip` unter genau diesem Namen enthalten. Die Setup-EXE kann aus dem vorigen Release übernommen werden, solange sich ihr Verhalten nicht ändern soll.
- Im ZIP liegen die Programmdateien direkt auf oberster Ebene und die Sprachdateien unter `Languages/`. Vor dem Hochladen macOS-Metadaten wie `__MACOSX`, `._*` und `.DS_Store` entfernen und das Archiv prüfen.
