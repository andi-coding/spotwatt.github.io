# RevenueCat Sales & Discounts Guide

## Problem: Google Play zeitliche Rabatte funktionieren nicht

Google Play Console erlaubt zeitlich begrenzte Rabatte für In-App-Produkte.
**Diese werden NICHT von RevenueCat unterstützt!**

### Was funktioniert NICHT:
- ❌ Zeitlich begrenzte Rabatte im Google Play Console
- ❌ `package.storeProduct.discounts` bleibt leer für Android
- ❌ User sehen nur den Original-Preis

---

## Lösung: RevenueCat Offerings für Sales verwenden

### Vorteile:
- ✅ Funktioniert für iOS UND Android
- ✅ Keine App-Updates nötig
- ✅ Remote-Steuerung über RevenueCat Dashboard
- ✅ A/B Testing möglich

### Setup:

#### 1. Erstelle mehrere Products im Store:

**Normal:**
- ID: `com.spotwatt.app.premium` (4,99€)

**Sale:**
- ID: `com.spotwatt.app.premium_sale` (3,99€)

#### 2. Erstelle 2 Offerings in RevenueCat:

**"Normal Offering":**
```
Lifetime Package:
  - Product: com.spotwatt.app.premium (4,99€)
```

**"Sale Offering":**
```
Lifetime Package:
  - Product: com.spotwatt.app.premium_sale (3,99€)
```

#### 3. Setze das aktive Offering:

In RevenueCat Dashboard:
- Markiere "Sale Offering" als **"Current"**
- App zeigt automatisch 3,99€

Wenn Sale vorbei:
- Markiere "Normal Offering" als **"Current"**
- App zeigt automatisch 4,99€

---

## Alternative: Introductory Offers (Empfohlen für Subscriptions)

### iOS & Android:

**Funktioniert mit RevenueCat!**

#### App Store Connect:
1. Subscription → **Introductory Offer**
2. Typ: "Pay as you go"
3. Dauer: z.B. "3 Monate"
4. Preis: z.B. "2,49€"

#### Google Play Console:
1. Subscription → **Introductory price**
2. Dauer: z.B. "3 months"
3. Preis: z.B. "2,49€"

#### Code:
```dart
if (package.storeProduct.introductoryPrice != null) {
  // Zeige "2,49€ für erste 3 Monate, dann 4,99€"
  salePrice = package.storeProduct.introductoryPrice!.priceString;
  regularPrice = package.storeProduct.priceString;
}
```

✅ **Das funktioniert automatisch mit unserem Code!**

---

## Was der aktuelle Code unterstützt:

### ✅ Funktioniert:
1. **Introductory Offers** (iOS/Android Subscriptions)
   - "7 Tage kostenlos"
   - "Erste 3 Monate 50% günstiger"

2. **iOS Promotional Offers** (StoreKit 2)
   - Nur iOS!
   - Für bestehende Subscriber

3. **RevenueCat Offerings**
   - Manuell verschiedene Products/Offerings erstellen

### ❌ Funktioniert NICHT:
- Google Play zeitliche Rabatte
- Google Play Developer-initiated sales

---

## Empfehlung für SpotWatt:

Da du ein **Subscription** (4,99€/Jahr) hast:

### Option 1: Introductory Offer
```
"Erste 3 Monate für 1,99€, dann 4,99€/Jahr"
```
- Konfiguriere in App Store Connect + Play Console
- Code funktioniert bereits! ✅

### Option 2: RevenueCat Offerings für Black Friday etc.
- Erstelle ein separates 3,99€ Subscription Product
- Wechsle das Current Offering für Sales
- Keine App-Updates nötig

---

## Zusammenfassung:

| Feature | iOS | Android | RevenueCat Support |
|---------|-----|---------|-------------------|
| Base Price | ✅ | ✅ | ✅ |
| Introductory Offers | ✅ | ✅ | ✅ |
| iOS Promotional Offers | ✅ | ❌ | ⚠️ Partial |
| Google Play Time-Limited Sales | ❌ | ❌ | ❌ |
| RevenueCat Offerings | ✅ | ✅ | ✅ |

**Beste Lösung**: Introductory Offers + RevenueCat Offerings
