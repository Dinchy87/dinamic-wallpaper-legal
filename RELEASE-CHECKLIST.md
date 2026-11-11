# Vor finaler Veröffentlichung zu ergänzen

Status: ENTWURF / NICHT FINAL FREIGEGEBEN (11.11.2026).

- [x] Name und ladungsfähige Anschrift vom Betreiber erhalten.
- [ ] Eigene öffentliche E-Mail-Adresse für Support und Datenschutz einrichten und testen.
- [ ] Betreiberstatus, gegebenenfalls Vertretung, Register, Umsatzsteuer-/Wirtschafts-ID, Beruf/Zulassung prüfen; nur zutreffende Angaben eintragen.
- [ ] Tatsächlich ausgelieferten iOS-Build sowie alle SDKs auf Werbung, Tracking, Diagnostik, Auth, Käufe und sonstige Datenerhebungen prüfen.
- [ ] Live-Datenfluss und wallpaper-engagement prüfen: empfangene Felder, Tabellen, Statistikzwecke, IP-/Fehlerlogs, Server-Zeitstempel und Weitergaben.
- [ ] Rechtsgrundlage für jede Verarbeitung einschließlich lokaler Kennung und Analyse bestimmen; gegebenenfalls Einwilligungsmechanismus und Widerspruch umsetzen.
- [ ] Vertragspartner und Rollen von Supabase, Cloudflare und GitHub Pages sowie später Outlook klären. AV-Verträge, Regionen, Unterauftragnehmer und Drittlandgarantien prüfen.
- [ ] Speicherdauer/Kriterien für Installation, Interaktionen, Favoriten, Logs, Cache, Support und Backups festlegen und technische Umsetzung prüfen.
- [ ] Löschung und Auskunft anhand installation_id sicher ermöglichen und testen; keine Deinstallations-Löschzusage.
- [ ] Zuständige Aufsichtsbehörde und gegebenenfalls Datenschutzbeauftragten bestimmen; Art.-13-Angaben zu Bereitstellungspflicht, Folgen und automatisierten Entscheidungen vervollständigen.
- [ ] Nutzungs-/Bildrechte, Quellen und Lizenzumfang klären; gegebenenfalls Verbraucher- und Kaufbedingungen ergänzen.
- [ ] Endgültige Texte und App-Store-Datenschutzangaben mit dem tatsächlich eingereichten Build abgleichen.
- [ ] Erst danach Entwurfsbanner/noindex/robots bewusst ändern und finale Freigabe dokumentieren.

## Befundgrenze

Geprüft: EngagementService, FavoritesStore, WallpaperImageLoader, WallpaperDetailView, WallpaperRepository, SettingsView sowie technische Projektdokumentation. installation_id ist lokale UUID; Favoritenänderungen und erfolgreiche Fotos-Speicherungen lösen Ereignisse an Supabase aus. Unbestätigte Ereignisse bleiben in UserDefaults. Bildabruf über signierte URL, lokaler Cache; R2 als Bildspeicher in Code/Projektdokumentation. Keine Live-Konfiguration oder vollständige Backend-/SDK-Prüfung erfolgt.

## Quellen zur Abschlussprüfung

- https://eur-lex.europa.eu/eli/reg/2016/679/oj/deu
- https://www.gesetze-im-internet.de/ddg/__5.html
- https://docs.github.com/en/site-policy/privacy-policies/github-general-privacy-statement
- https://docs.github.com/en/pages/getting-started-with-github-pages/configuring-a-publishing-source-for-your-github-pages-site
