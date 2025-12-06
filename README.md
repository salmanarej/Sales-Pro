<!--
	SEO: README optimized for GitHub Discoverability
	Keywords: Flutter Sales App, Inventory Management, POS, Drift SQLite, Barcode, Firebase, Localization Arabic English
-->

# Sales Pro | Flutter Sales & Inventory Management (Cross-Platform)

<div align="center">

![Flutter](https://img.shields.io/badge/Flutter-3.9.2-02569B?logo=flutter)
![Dart](https://img.shields.io/badge/Dart-3.9.2-0175C2?logo=dart)
![Platforms](https://img.shields.io/badge/Platforms-Android%20%7C%20iOS%20%7C%20Web%20%7C%20Desktop-blue)
![Localization](https://img.shields.io/badge/Localization-Arabic%20%7C%20English-green)
![Database](https://img.shields.io/badge/Database-Drift%20%7C%20SQLite-orange)
![License](https://img.shields.io/badge/License-MIT-green.svg)

**Modern sales and inventory management solution with localization, barcode scanning, and offline-first support.**

[العربية](#arabic)

</div>

---

## Why Sales Pro?
- Quick deployment with clear, scalable feature-based architecture
- Offline-first functionality via local Drift/SQLite database
- Full localization support (Arabic/English) with easy language extension
- Optional Firebase integration for notifications and analytics

## Core Features
- Secure authentication and login
- Invoices: Create, edit, delete, and track payments
- Inventory: Manage products and quantities
- Multi-store and order management
- Camera-based barcode scanning
- Push notifications and offline-first design

## Architecture Overview
```
lib/
	core/            # Configuration, SOAP, utilities
	features/        # auth, orders, invoice, catalog, store, balance, time
	screens/         # Main screens
	state/           # State management (Provider)
	repository/      # Data layer
	services/        # Firebase/Notifications
	db/              # Drift/SQLite database
	theme/           # Colors and styling
```

## Quick Start
```bash
git clone https://github.com/salmanarej/Sales-Pro.git
cd Sales-Pro
flutter pub get
flutter run
```

### Firebase Setup (Optional)
- Add `android/app/google-services.json`
- Create `lib/firebase_options.dart` with your project settings

### Production Build
```bash
flutter build apk --release
flutter build appbundle --release
flutter build web --release
flutter build windows --release
```

## Localization (Arabic/English)
- Language files: `assets/lang/ar.json`, `assets/lang/en.json`
- Add new language: Create `assets/lang/<code>.json` and update config in `lib/core/localization/`
- Extract strings:
```bash
python ./tool/extract_strings.py
```

## Testing & Quality
```bash
flutter test
```
- Follow `analysis_options.yaml` guidelines

## GitHub Discoverability & SEO
- Clear title with keywords: Flutter, Sales, Inventory
- Concise description and badge illustrations
- Organized sections: Quick Start, Features, Architecture, Localization
- Internal links to documentation
- Keywords in README comments

## Contributing & License
- Contributions welcome! Open a Pull Request or Issue
- License: [MIT](LICENSE)

## Support
Open an issue with platform details, steps, and logs.

---

## العربية
تطبيق Sales Pro هو حل حديث لإدارة المبيعات والمخزون مبني بـ Flutter، يدعم العمل دون اتصال، مسح الباركود، التوطين (عربي/إنجليزي)، Firebase اختياري، وبنية ميزات واضحة.

**البدء السريع:**
```bash
flutter pub get && flutter run
```
- 💼 GitHub: [@salmanarej](https://github.com/salmanarej/Sales-Pro)
