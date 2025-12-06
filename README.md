<!--
	SEO: Arabic-first README optimized for GitHub Discoverability
	Keywords: Flutter Sales App, Inventory Management, POS, Drift SQLite, Barcode, Firebase, Localization Arabic English
-->

# تطبيق Sales Pro | إدارة المبيعات والمخزون بـ Flutter (متعدد المنصات)

<div align="center">

![Flutter](https://img.shields.io/badge/Flutter-3.9.2-02569B?logo=flutter)
![Dart](https://img.shields.io/badge/Dart-3.9.2-0175C2?logo=dart)
![Platforms](https://img.shields.io/badge/Platforms-Android%20%7C%20iOS%20%7C%20Web%20%7C%20Desktop-blue)
![Localization](https://img.shields.io/badge/Localization-Arabic%20%7C%20English-green)
![Database](https://img.shields.io/badge/Database-Drift%20%7C%20SQLite-orange)
![License](https://img.shields.io/badge/License-MIT-green.svg)

**حل حديث لإدارة المبيعات والمخزون، يدعم التوطين، الباركود، والعمل دون اتصال.**

[English README](#english)

</div>

---

## لماذا «تطبيق Sales Pro»؟
- سرعة الإطلاق عبر هيكل ميزات واضح وقابل للتوسعة.
- يعمل بدون اتصال عبر قاعدة بيانات محلية Drift/SQLite.
- جاهزية كاملة للتوطين (Arabic/English) وإضافة لغات بسهولة.
- تكاملات اختيارية مع Firebase للإشعارات والتحليلات.

## الميزات الأساسية
- المصادقة الآمنة وتسجيل الدخول.
- فواتير: إنشاء/تعديل/حذف وتتبّع المدفوعات.
- مخزون: إدارة المنتجات والكميات.
- طلبات ومتاجر متعددة.
- مسح باركود بالكاميرا.
- إشعارات ودعم Offline-First.

## لقطة سريعة للبنية
```
lib/
	core/            # إعدادات و SOAP وأدوات مشتركة
	features/        # auth, orders, invoice, catalog, store, balance, time
	screens/         # شاشات رئيسية
	state/           # إدارة الحالة (Provider)
	repository/      # طبقة البيانات
	services/        # Firebase/Notifications
	db/              # Drift/SQLite
	theme/           # الألوان والتصميم
```

## البداية السريعة
```powershell
git clone https://github.com/salmanarej/Sales-Pro.git ; cd Sales-Pro
flutter pub get
flutter run
```

### إعداد Firebase (اختياري)
- أضف `android/app/google-services.json`.
- أنشئ `lib/firebase_options.dart` بإعدادات مشروعك.

### البناء للإنتاج
```powershell
flutter build apk --release
flutter build appbundle --release
flutter build web --release
flutter build windows --release
```

## التوطين (Arabic/English)
- ملفات اللغات: `assets/lang/ar.json`, `assets/lang/en.json`.
- أضف لغة: أنشئ `assets/lang/<code>.json` ثم حدّث الإعداد في `lib/core/localization/`.
- استخراج النصوص:
```powershell
python .\tool\extract_strings.py
```

## الاختبارات والجودة
```powershell
flutter test
```
- اتبع `analysis_options.yaml`.

## اكتشاف GitHub وتحسين SEO
- عنوان واضح يتضمن كلمات مفتاحية: Flutter, Sales, Inventory.
- وصف موجز جذاب وصور/شارات توضيحية.
- أقسام مرتبة: Quick Start، Features، Architecture، Localization.
- روابط داخلية لملفات الأدلة.
- كلمات مفتاحية في التعليقات أعلى README.

## المساهمة والترخيص
- المساهمات مرحب بها! افتح Pull Request أو Issue.
- الترخيص: [MIT](LICENSE).

## الدعم
افتح قضية مع تفاصيل المنصة والخطوات واللوج.

---

## English (Brief)
Sales Pro is a modern Flutter app for Sales and Inventory with Offline support, Barcode scanning, Localization (Arabic/English), optional Firebase, and a clean feature-oriented structure. Quick start:
```bash
flutter pub get && flutter run
```
- 💼 GitHub: [@salmanarej](https://github.com/salmanarej/Sales-Pro)
