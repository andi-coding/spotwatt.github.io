# NEUE ABSCHNITTE FÜR DATENSCHUTZERKLÄRUNG - SpotWatt

**Stand:** Januar 2025
**Version:** 2.0 (erweitert um Firebase & RevenueCat)

---

## 📍 POSITION IM DOKUMENT

Diese neuen Abschnitte sollen **nach Abschnitt 2.3 (Website - GitHub Pages)** eingefügt werden.

---

## ✅ NEUER ABSCHNITT 2.4: Firebase Cloud Messaging & Cloud Firestore

```html
<h3>2.4 App - Firebase Cloud Messaging & Cloud Firestore (Push-Benachrichtigungen)</h3>
<p>
    Um Ihnen Push-Benachrichtigungen senden zu können (z.B. tägliche Preisübersicht,
    günstigste Zeiten, Geräte-Erinnerungen), nutzt SpotWatt Firebase Cloud Messaging (FCM)
    und Cloud Firestore von Google LLC.
</p>

<h4>Welche Daten werden verarbeitet?</h4>
<ul>
    <li><strong>FCM-Token:</strong> Eine eindeutige Geräte-ID, automatisch von Firebase generiert</li>
    <li><strong>Benachrichtigungseinstellungen:</strong> Aktivierte Benachrichtigungsarten, Zeiten, Schwellenwerte</li>
    <li><strong>Gerätenamen:</strong> Von Ihnen vergebene Namen für Geräte-Erinnerungen (z.B. "Waschmaschine")</li>
    <li><strong>Zeitfenster:</strong> Geplante Zeiten für Geräte-Erinnerungen</li>
    <li><strong>Marktauswahl:</strong> Gewähltes Land (Deutschland oder Österreich)</li>
    <li><strong>Platform:</strong> Betriebssystem (iOS oder Android)</li>
    <li><strong>IP-Adresse:</strong> Technisch notwendig für die Kommunikation mit Firebase-Servern</li>
</ul>

<h4>Speicherort</h4>
<p>
    Google Cloud Firestore (bevorzugt europäische Rechenzentren)
</p>

<h4>Zweck der Verarbeitung</h4>
<ul>
    <li>Versand von Push-Benachrichtigungen (täglich, günstigste Zeit, Preisschwellen)</li>
    <li>Geräte-Erinnerungen für optimale Strompreis-Zeitfenster</li>
    <li>Zeitplanung von Benachrichtigungen (über Google Cloud Functions)</li>
    <li>Synchronisation Ihrer Einstellungen zwischen App und Backend</li>
</ul>

<h4>Speicherdauer</h4>
<p>
    Die Daten werden gespeichert, solange Sie die App aktiv nutzen.
    Ungültige Daten (z.B. nach App-Deinstallation) werden automatisch bereinigt.
</p>

<h4>Rechtsgrundlage</h4>
<p>
    <strong>Art. 6 Abs. 1 lit. a DSGVO (Einwilligung):</strong> Sie willigen durch Aktivierung der Benachrichtigungen
    in die Verarbeitung ein.
</p>
<p>
    <strong>Art. 6 Abs. 1 lit. b DSGVO (Vertragserfüllung):</strong> Für Premium-Nutzer sind Benachrichtigungen
    Teil der gebuchten Leistung.
</p>

<h4>Internationale Datenübertragung</h4>
<p>
    Google LLC ist ein US-amerikanisches Unternehmen (1600 Amphitheatre Parkway, Mountain View, CA 94043, USA).
    Die Datenverarbeitung kann auch außerhalb der EU erfolgen. Rechtsgrundlage für die Drittlandübermittlung ist:
</p>
<ul>
    <li><strong>EU-US Data Privacy Framework</strong> (Angemessenheitsbeschluss der EU-Kommission gemäß Art. 45 DSGVO)</li>
    <li>Google Firebase nutzt europäische Rechenzentren (bevorzugt), kann aber auch US-Server verwenden</li>
</ul>
<p>
    <strong>Weitere Informationen:</strong><br>
    Google Firebase Datenschutzerklärung: <a href="https://firebase.google.com/support/privacy" target="_blank" rel="noopener">https://firebase.google.com/support/privacy</a><br>
    Google Cloud Datenschutz: <a href="https://cloud.google.com/privacy" target="_blank" rel="noopener">https://cloud.google.com/privacy</a>
</p>

<h4>Hinweis zu personenbezogenen Daten</h4>
<p>
    <strong>Anonymes System ohne Nutzer-Zuordnung:</strong><br>
    SpotWatt verwendet ein anonymes System ohne Nutzer-Accounts (keine E-Mails, keine Namen, keine Login-Daten).
    FCM-Tokens sind technische Geräte-Identifikatoren, die <strong>nicht einer bestimmten Person zugeordnet werden können</strong>.
</p>
<p>
    Gemäß <strong>Art. 11 Abs. 2 DSGVO</strong> finden die Betroffenenrechte (Art. 15-20 DSGVO, einschließlich Auskunfts- und Löschungsrecht)
    keine Anwendung, wenn der Verantwortliche nicht in der Lage ist, die betroffene Person zu identifizieren.
</p>
<p>
    <strong>Folge:</strong> Eine manuelle Löschung auf individuelle Anfrage ist rechtlich nicht erforderlich,
    da wir FCM-Tokens nicht einzelnen Personen zuordnen können. Die automatische Löschfrist von 180 Tagen ist angemessen
    und DSGVO-konform. Details zu Ihren Rechten finden Sie in Abschnitt 5.
</p>
```

---

## ✅ NEUER ABSCHNITT 2.5: RevenueCat (In-App-Käufe)

```html
<h3>2.5 App - RevenueCat (In-App-Käufe & Premium-Features)</h3>
<p>
    Für die Verwaltung von In-App-Käufen (Premium-Version) nutzt SpotWatt den Dienst RevenueCat, Inc.
    RevenueCat verwaltet Ihre Käufe und Premium-Status geräteübergreifend.
</p>

<h4>Welche Daten werden verarbeitet?</h4>
<ul>
    <li><strong>RevenueCat User ID:</strong> Anonymisierte Nutzer-ID (generiert aus FCM-Token oder Geräte-ID)</li>
    <li><strong>Kauftransaktionen:</strong> Welche Premium-Features gekauft wurden (über Google Play / App Store)</li>
    <li><strong>Premium-Status (Entitlement):</strong> Ob Premium-Features freigeschaltet sind</li>
    <li><strong>Platform:</strong> Betriebssystem (iOS oder Android)</li>
    <li><strong>App-Version:</strong> Installierte App-Version</li>
    <li><strong>Store-Informationen:</strong> Kauf-Receipts von Google Play / Apple App Store</li>
</ul>

<h4>KEINE Verarbeitung von Zahlungsdaten</h4>
<p>
    <strong>Wichtig:</strong> RevenueCat und SpotWatt verarbeiten <strong>keine Zahlungsdaten</strong>
    (Kreditkartennummern, Bankverbindungen). Die Kaufabwicklung erfolgt ausschließlich über:
</p>
<ul>
    <li><strong>Android:</strong> Google Play Store (verwaltet von Google LLC)</li>
    <li><strong>iOS:</strong> Apple App Store (verwaltet von Apple Inc.)</li>
</ul>
<p>
    Es gelten die Datenschutzrichtlinien von
    <a href="https://policies.google.com/privacy" target="_blank" rel="noopener">Google Play</a> bzw.
    <a href="https://www.apple.com/legal/privacy/" target="_blank" rel="noopener">Apple</a>.
</p>

<h4>Zweck der Verarbeitung</h4>
<ul>
    <li>Verwaltung und Freischaltung von Premium-Features</li>
    <li>Wiederherstellung von Käufen bei App-Neuinstallation</li>
    <li>Geräteübergreifende Synchronisation des Premium-Status</li>
    <li>Verhinderung von Missbrauch (z.B. mehrfache Nutzung ohne Kauf)</li>
</ul>

<h4>Speicherdauer</h4>
<ul>
    <li><strong>Premium-Status:</strong> Solange Sie die App nutzen (bei Lifetime-Kauf: unbegrenzt)</li>
    <li><strong>Kaufbelege:</strong> 10 Jahre (steuerrechtliche Aufbewahrungspflicht gemäß § 132 BAO / § 147 AO)</li>
</ul>

<h4>Rechtsgrundlage</h4>
<p>
    <strong>Art. 6 Abs. 1 lit. b DSGVO (Vertragserfüllung):</strong> Die Datenverarbeitung ist erforderlich,
    um den Kaufvertrag zu erfüllen und Premium-Features bereitzustellen.
</p>
<p>
    <strong>Art. 6 Abs. 1 lit. c DSGVO (Rechtliche Verpflichtung):</strong> Aufbewahrung von Kaufbelegen
    für steuerliche Zwecke (gesetzliche Pflicht).
</p>

<h4>Internationale Datenübertragung</h4>
<p>
    RevenueCat, Inc. ist ein US-amerikanisches Unternehmen (548 Market St, PMB 61865, San Francisco, CA 94104, USA).
    Die Datenverarbeitung erfolgt in den USA. Rechtsgrundlage für die Drittlandübermittlung:
</p>
<ul>
    <li><strong>EU-US Data Privacy Framework</strong> (Angemessenheitsbeschluss der EU-Kommission gemäß Art. 45 DSGVO)</li>
    <li>Alternativ: EU-Standardvertragsklauseln (Standard Contractual Clauses)</li>
</ul>
<p>
    <strong>Weitere Informationen:</strong><br>
    RevenueCat Datenschutzerklärung: <a href="https://www.revenuecat.com/privacy" target="_blank" rel="noopener">https://www.revenuecat.com/privacy</a><br>
    RevenueCat DSGVO-Compliance: <a href="https://www.revenuecat.com/gdpr" target="_blank" rel="noopener">https://www.revenuecat.com/gdpr</a>
</p>

<h4>Hinweis zu personenbezogenen Daten</h4>
<p>
    <strong>Anonymes System:</strong><br>
    RevenueCat User-IDs sind anonymisierte technische Identifikatoren, die <strong>nicht einzelnen Personen zugeordnet werden können</strong>.
</p>
<p>
    Gemäß <strong>Art. 11 Abs. 2 DSGVO</strong> finden die Betroffenenrechte (Art. 15-20 DSGVO, einschließlich Auskunfts- und Löschungsrecht)
    keine Anwendung, wenn der Verantwortliche nicht in der Lage ist, die betroffene Person zu identifizieren.
</p>
<p>
    <strong>Ausnahme - Kaufbelege:</strong> Für steuerrechtliche Zwecke müssen Kaufbelege 10 Jahre aufbewahrt werden (§ 132 BAO / § 147 AO).
    Details zu Ihren Rechten finden Sie in Abschnitt 5.
</p>
```

---

## ✅ NEUER ABSCHNITT 2.6: Google Play Store & Apple App Store

```html
<h3>2.6 App - Google Play Store & Apple App Store</h3>
<p>
    Die SpotWatt App wird über den Google Play Store (Android) und Apple App Store (iOS) verteilt.
    Beim Download, bei Updates und bei In-App-Käufen werden Daten durch diese Stores verarbeitet.
</p>

<h4>Welche Daten werden verarbeitet?</h4>
<p>
    Die Stores verarbeiten folgende Daten (unabhängig von SpotWatt):
</p>
<ul>
    <li><strong>Google Play Store:</strong> Google-Konto, Zahlungsdaten, Installationsdatum, Geräteinformationen, Bewertungen</li>
    <li><strong>Apple App Store:</strong> Apple-ID, Zahlungsdaten, Installationsdatum, Geräteinformationen, Bewertungen</li>
</ul>

<h4>Zweck</h4>
<ul>
    <li>Bereitstellung und Installation der App</li>
    <li>Verwaltung von Updates</li>
    <li>Kaufabwicklung bei Premium-Features</li>
    <li>Bewertungen und Reviews</li>
</ul>

<h4>Verantwortlicher</h4>
<p>
    Für die Datenverarbeitung durch die Stores sind <strong>Google LLC</strong> bzw. <strong>Apple Inc.</strong>
    verantwortlich, nicht SpotWatt. SpotWatt hat keinen Zugriff auf diese Daten.
</p>

<h4>Weitere Informationen</h4>
<ul>
    <li><strong>Google Play:</strong> <a href="https://policies.google.com/privacy" target="_blank" rel="noopener">Google Datenschutzerklärung</a></li>
    <li><strong>Apple App Store:</strong> <a href="https://www.apple.com/legal/privacy/" target="_blank" rel="noopener">Apple Datenschutzerklärung</a></li>
</ul>
```

---

## ❌ ABSCHNITT 2.7 "EXTERNE LINKS" ENTFERNT

**Begründung:**
- Ko-fi wird aus der App entfernt
- SMARD.de ist bereits in Abschnitt 2.2 (CloudFlare API) erwähnt
- CC BY Link ist nur Lizenz-Info, keine Datenverarbeitung
- Eigene Website-Links (spotwatt.at) sind kein Drittanbieter
- Abschnitt ist rechtlich nicht notwendig und würde nur verwirren

---

## ✅ ABSCHNITT 3 ÜBERARBEITEN: Datensparsamkeit und Datenvermeidung

**ERSETZE den aktuellen Text durch:**

```html
<h2>3. Datensparsamkeit und Datenvermeidung</h2>
<p>
    Wir respektieren Ihre Privatsphäre und beschränken die Datenerfassung
    auf das absolut Notwendige für die Funktionalität der App.
</p>

<h3>3.1 Was wir NICHT erfassen</h3>
<p>
    Folgende Daten werden <strong>nicht</strong> erfasst oder übertragen:
</p>
<ul>
    <li>Nutzungsdaten oder detailliertes Analytics (z.B. welche Seiten Sie besuchen)</li>
    <li>Persönliche Profile oder Accounts mit Login</li>
    <li>Standortdaten an externe Server (Geofencing nur lokal auf Gerät)</li>
    <li>Kontakte oder Telefonbuch</li>
    <li>Fotos oder Mediendateien</li>
    <li>Browser-Verlauf oder App-Nutzung außerhalb von SpotWatt</li>
    <li>Detaillierte Crash-Reports mit persönlichen Daten</li>
    <li>Werbe-IDs oder Tracking-Cookies</li>
</ul>

<h3>3.2 Minimalprinzip</h3>
<p>
    Bei allen Datenverarbeitungen halten wir uns an das <strong>Minimalprinzip</strong> (Art. 5 Abs. 1 lit. c DSGVO):
</p>
<ul>
    <li><strong>Firebase:</strong> Nur FCM-Token + minimal notwendige Einstellungen, keine Geräte-IDs oder Nutzerprofile</li>
    <li><strong>RevenueCat:</strong> Nur anonymisierte User-IDs + Kaufstatus, keine Zahlungsdaten</li>
    <li><strong>CloudFlare:</strong> Nur IP-Adresse für Strompreis-Abruf (technisch zwingend notwendig)</li>
</ul>

<h3>3.3 Lokale Verarbeitung bevorzugt</h3>
<p>
    Wo immer möglich, werden Daten <strong>lokal auf Ihrem Gerät</strong> verarbeitet:
</p>
<ul>
    <li>Strompreisdaten (24-48h gecacht)</li>
    <li>App-Einstellungen (SharedPreferences)</li>
    <li>Standortdaten für Geofencing (optional, nur lokal)</li>
    <li>Preisberechnungen (Vollkosten-Modus)</li>
</ul>
```

---

## ✅ ABSCHNITT 5 ERWEITERN: Ihre Rechte

**FÜGE nach Abschnitt 5 (Ihre Rechte) HINZU:**

```html
<h3>5.2 So machen Sie Ihre Rechte geltend</h3>

<h4>Auskunftsrecht, Löschungsrecht und Datenübertragbarkeit (Art. 15, 17, 20 DSGVO)</h4>
<p>
    <strong>Keine Identifizierung möglich (Art. 11 Abs. 2 DSGVO):</strong><br>
    SpotWatt verwendet ein anonymes System ohne Nutzer-Accounts (keine E-Mail, kein Name, keine Login-Daten).
    Die gespeicherten FCM-Tokens und RevenueCat User-IDs sind technische Identifikatoren,
    die wir <strong>nicht einzelnen Personen zuordnen können</strong>.
</p>
<p>
    Gemäß <strong>Art. 11 Abs. 2 DSGVO</strong> finden folgende Betroffenenrechte (Art. 15-20 DSGVO)
    <strong>keine Anwendung</strong>, wenn der Verantwortliche nicht in der Lage ist, die betroffene Person zu identifizieren:
</p>
<ul>
    <li><strong>Auskunftsrecht (Art. 15):</strong> Wir können nicht feststellen, welche Daten zu Ihnen gehören</li>
    <li><strong>Berichtigungsrecht (Art. 16):</strong> Wir können nicht identifizieren, welche Daten berichtigt werden sollen</li>
    <li><strong>Löschungsrecht (Art. 17):</strong> Wir können nicht bestimmen, welche Daten gelöscht werden sollen</li>
    <li><strong>Einschränkungsrecht (Art. 18):</strong> Wir können nicht zuordnen, welche Verarbeitung eingeschränkt werden soll</li>
    <li><strong>Datenübertragbarkeit (Art. 20):</strong> Wir können nicht ermitteln, welche Daten übertragen werden sollen</li>
</ul>

<h4>Was Sie selbst tun können</h4>
<p>
    Da keine Nutzer-Zuordnung möglich ist, können Sie Ihre Daten selbst verwalten:
</p>
<ul>
    <li><strong>Daten einsehen:</strong> Alle Ihre Einstellungen sind in der App sichtbar (Einstellungen → Benachrichtigungen, Premium-Status)</li>
    <li><strong>Daten ändern:</strong> Sie können alle Einstellungen jederzeit in der App ändern</li>
    <li><strong>Daten löschen:</strong> App deinstallieren → Sofortige Löschung lokal + automatische Bereinigung aus Firestore nach spätestens 180 Tagen</li>
    <li><strong>Daten exportieren:</strong> Technisch nicht möglich wegen fehlender Nutzer-Zuordnung. Sie können Ihre Einstellungen aber manuell notieren.</li>
</ul>

<h4>Widerspruchsrecht (Art. 21 DSGVO)</h4>
<p>
    Sie können der Datenverarbeitung jederzeit widersprechen:
</p>
<ul>
    <li><strong>Benachrichtigungen deaktivieren:</strong> App-Einstellungen → Benachrichtigungen → Alle deaktivieren</li>
    <li><strong>Vollständiger Widerspruch:</strong> App deinstallieren (löscht alle Daten)</li>
</ul>

<h4>Einwilligung widerrufen</h4>
<p>
    Soweit die Verarbeitung auf Ihrer Einwilligung beruht (z.B. Benachrichtigungen),
    können Sie diese jederzeit widerrufen:
</p>
<ul>
    <li><strong>Ohne Angabe von Gründen</strong></li>
    <li><strong>Mit Wirkung für die Zukunft</strong> (bisherige Verarbeitung bleibt rechtmäßig)</li>
    <li><strong>In der App:</strong> Einstellungen → Benachrichtigungen → Alle deaktivieren</li>
</ul>
```

---

## ✅ NEUER ABSCHNITT 8: Automatisierte Entscheidungsfindung

**FÜGE nach Abschnitt 7 (Kinder) EIN:**

```html
<h2>8. Automatisierte Entscheidungsfindung und Profiling</h2>

<p>
    SpotWatt verwendet <strong>keine automatisierte Entscheidungsfindung</strong> gemäß Art. 22 DSGVO und
    erstellt <strong>keine Nutzerprofile</strong> zu Marketing- oder Werbezwecken.
</p>

<p>
    Die App führt ausschließlich technische Berechnungen durch:
</p>
<ul>
    <li>Preisberechnungen (Vollkosten-Modus)</li>
    <li>Zeitplanung für Benachrichtigungen</li>
    <li>Optimierung von Geräteeinsatz-Zeiten</li>
</ul>

<p>
    Diese Berechnungen haben <strong>keine rechtlichen Folgen</strong> für Sie und dienen
    ausschließlich der App-Funktionalität (Anzeige optimaler Strompreis-Zeiten).
</p>
```

---

## ✅ ALTE ABSCHNITTE UMNUMMERIEREN

- Alt: Abschnitt 8 (Änderungen) → **Neu: Abschnitt 9**
- Alt: Abschnitt 9 (Kontakt) → **Neu: Abschnitt 10**
- Alt: Abschnitt 10 (Aufsichtsbehörde) → **Neu: Abschnitt 11**

---

## ✅ DATUM AKTUALISIEREN

**Ändere in Zeile 73:**

```html
<div class="last-updated">
    <strong>Stand:</strong> Januar 2025
</div>
```

---

## 📄 ZUSAMMENFASSUNG DER ÄNDERUNGEN

### NEUE ABSCHNITTE:
- ✅ 2.4 Firebase Cloud Messaging & Cloud Firestore
- ✅ 2.5 RevenueCat (In-App-Käufe)
- ✅ 2.6 Google Play Store & Apple App Store
- ✅ 2.7 Externe Links (umbenannt von 2.4)
- ✅ 8 Automatisierte Entscheidungsfindung

### ÜBERARBEITETE ABSCHNITTE:
- ✅ 3 Datensparsamkeit (angepasst an neue Services)
- ✅ 5.2 Ihre Rechte (detaillierte Anleitung)

### UMNUMMERIERT:
- Abschnitte 8-10 → 9-11

---

Soll ich jetzt die komplette aktualisierte `privacy.html` Datei erstellen?
