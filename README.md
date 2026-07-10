# OptionVisualizer — Downloads

Options-Strategie-Cockpit mit Live-Anbindung an Interactive Brokers (TWS/IB
Gateway) und Tastytrade: Multi-Leg-Payoff, Strategie-Erkennung, Chain-Analyse,
Trading-Journal. Läuft **komplett lokal** auf deinem Rechner (Single-User).

Dieses Repository enthält **nur die fertigen Pakete** — der Quellcode ist
privat.

## Download

Neueste Version unter **[Releases](../../releases)**:

| Plattform | Datei |
|---|---|
| **Windows** | `OptionVisualizerSetup-<version>.exe` (Installer) |
| **macOS** (Apple Silicon) | `OptionVisualizer-<version>-macOS-arm64.dmg` (App) · `.zip` (portabel) |

## Erste Schritte

1. **Voraussetzung:** laufende IBKR **TWS** oder **IB Gateway** mit aktivierter
   API (Socket-Port `7497` Paper / `7496` Live; Gateway `4002`/`4001`) und
   `127.0.0.1` als vertrauenswürdige IP.
2. **Windows:** SmartScreen zeigt „Unbekannter Herausgeber" → *Weitere
   Informationen → Trotzdem ausführen* (die App ist unsigniert).
3. **macOS:** Rechtsklick → *Öffnen*, bzw. *Systemeinstellungen →
   Datenschutz & Sicherheit → Dennoch öffnen*. Beim Start öffnet sich ein
   Terminal-Fenster mit den Live-Logs — das ist Absicht (Logs liegen unter
   `~/Library/Logs/OptionVisualizer/`).
4. Die App öffnet den Browser auf `http://localhost:8765`. Alles Weitere
   (Broker-Ports, API-Keys, Steuersätze) stellst du in der App unter
   **Einstellungen** ein.

## Sicherheit der Orders

Orders werden **nie automatisch** abgeschickt: IBKR-Orders landen zur
manuellen Bestätigung in der TWS („Stage in TWS"), erst dein Klick auf
*Transmit* dort sendet sie.

## Haftungsausschluss

Private Software, Nutzung **auf eigene Gefahr**. Dies ist **keine
Anlageberatung**; keine Gewähr für Richtigkeit von Kursen, Kennzahlen oder
Steuerschätzungen. Handel mit Optionen und Futures birgt erhebliche Risiken.

© 2026 Carsten Rachfahl — alle Rechte vorbehalten (siehe [LICENSE](LICENSE)).
