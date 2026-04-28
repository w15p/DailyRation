# DailyRation

DailyRation is a nutrition-tracking app for iOS and macOS built by w15p. It is designed to work without accounts, servers, or subscriptions. Your data stays yours.

**Effective date:** April 9, 2026

---

## The Short Version

DailyRation does not collect, transmit, or sell your personal data. There is no server, no analytics, no advertising, and no tracking. Everything lives on your device (and, optionally, in your private iCloud account).

---

## Data Storage

All app data --- recipes, ingredients, meal logs, nutrition information, and your settings --- is stored locally on your device using SwiftData (backed by SQLite). No data is stored on any server controlled by the developer.

### iCloud Sync

iCloud sync is **on by default** and can be turned off in the app's settings. When enabled, your recipes, ingredients, and meal log entries sync across your Apple devices through Apple's CloudKit private database. This data is tied to your Apple ID and is accessible only to you. Apple's iCloud terms and privacy policy govern that storage.

Your app settings (nutrition targets, accent color, nutrient display preferences) always sync via iCloud regardless of the sync toggle. This ensures a consistent experience across devices and contains no health or nutrition data.

If you disable iCloud sync, recipes, ingredients, and meal logs remain on-device only.

## Network Requests

DailyRation makes exactly two kinds of network requests, both initiated by you:

### USDA FoodData Central

When you search for an ingredient by name, the app queries the [USDA FoodData Central](https://fdc.nal.usda.gov/) API directly from your device. The only data sent is the food name you typed. No personal information, device identifiers, or usage data is included.

### Open Food Facts

When you scan a barcode, the app queries the [Open Food Facts](https://world.openfoodfacts.org/) API directly from your device. If no match is found, it falls back to USDA FoodData Central using the same barcode. The only data sent is the barcode number. No personal information, device identifiers, or usage data is included.

No other network requests are made by the app.

## Apple Health Integration

DailyRation offers optional Apple Health (HealthKit) integration, controlled by two independent toggles that are both **off by default**:

- **Write nutrition data to Health** --- logs each meal's nutrition (calories, protein, etc.) to Apple Health.
- **Read active energy burned** --- reads your active calorie expenditure from Apple Health to display alongside nutrition data.

Both features run entirely on-device through Apple's HealthKit framework. No health data is sent to any server. You can enable or disable either toggle at any time in the app's settings, and you can revoke Health access at the system level in Settings > Health > DailyRation.

## Nutrition Label Scanning

The app can use your device's camera to scan nutrition labels via Apple's Vision framework (on-device OCR). Images are processed locally and are never transmitted, stored, or uploaded anywhere. The app requests camera access only when you initiate a label scan, and you can revoke camera permission at any time in system settings.

## UserDefaults

The app stores a small number of per-device preferences in UserDefaults, such as HealthKit opt-in states and iCloud sync preference. These are local device flags that never leave your device.

## Third-Party SDKs

There are none. DailyRation uses only Apple's first-party frameworks. There are no third-party SDKs, no analytics services, no crash reporters, no ad networks, no cookies, and no fingerprinting.

## Tracking

DailyRation does not track you. It does not participate in App Tracking Transparency because there is nothing to track. No data is shared with third parties for advertising, analytics, or any other purpose.

## Children's Privacy

DailyRation does not knowingly collect information from children under 13. The app does not collect information from anyone --- it has no server and no data collection mechanism.

## Changes to This Policy

If this policy changes, the updated version will be posted at this URL with a new effective date. Material changes will also be noted in the App Store release notes.

## Contact

Questions or concerns about this privacy policy can be raised via GitHub Issues:

[github.com/w15p/DailyRation/issues](https://github.com/w15p/DailyRation/issues)

---

&copy; 2026 w15p. All rights reserved.
