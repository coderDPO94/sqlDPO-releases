# sqlDPO – Setups

MySQL/MariaDB-Client für Windows von syreta. Dieses Repository enthält nur die Setups (Releases), keinen Quellcode.

## Installieren

1. Unter [Releases](https://github.com/coderDPO94/sqlDPO-releases/releases/latest) die Datei `sqlDPO-<Version>-x64.msi` herunterladen.
2. Starten und den Anweisungen folgen (Administratorrechte nötig, Installation für alle Benutzer nach `C:\Program Files\syreta\sqlDPO`).

Still, z.B. per Softwareverteilung:

```
msiexec /i sqlDPO-<Version>-x64.msi /qn                      # mit SQL Runner
msiexec /i sqlDPO-<Version>-x64.msi /qn ADDLOCAL=Main         # ohne Erweiterungen
```

## Updates

Installierte sqlDPO suchen beim Start und alle 12 Stunden hier nach einer neuen Version, laden sie im Hintergrund und prüfen sie (SHA-256). Installiert wird über „Jetzt aktualisieren“ oder beim Beenden; danach zeigt sqlDPO die Neuerungen. Abschalten oder andere Quelle: Optionen → Allgemein → Updates.

Jede Release enthält das MSI und `sqldpo-update.json` (Version, Prüfsumme, Größe, Versionshinweise).
