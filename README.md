# Ronak Film 🎬

**Ronak Film** is a modern, high-performance Video on Demand (VOD) application built for the Android platform (Mobile & Android TV). It provides a seamless streaming experience with clean architecture, modern UI components, and robust integration with local Iranian app stores and payment gateways.

---

## 🔗 دانلود و لینک‌های رسمی (Download & Links)

<div align="center">

[![Website](https://img.shields.io/badge/Website-Official_Site-4285F4?style=for-the-badge&logo=googlechrome&logoColor=white)](https://ronakfilm.com)
[![Cafe Bazaar](https://img.shields.io/badge/Cafe_Bazaar-Download-119143?style=for-the-badge&logo=android&logoColor=white)](https://cafebazaar.ir/app/com.ronak.ronakfilm)
[![Myket](https://img.shields.io/badge/Myket-Download-0083CA?style=for-the-badge&logo=googleplay&logoColor=white)](https://myket.ir/app/com.ronak.ronakfilm)

</div>

---

## 🌐 Tech Badges

<div align="center">

![Kotlin](https://img.shields.io/badge/Kotlin-2.0.20-7F52FF?style=flat-square&logo=kotlin&logoColor=white)
![Jetpack Compose](https://img.shields.io/badge/Jetpack_Compose-Material_3-4285F4?style=flat-square&logo=jetpackcompose&logoColor=white)
![Android TV](https://img.shields.io/badge/Android_TV-Supported-3DDC84?style=flat-square&logo=android&logoColor=white)
![Media3 ExoPlayer](https://img.shields.io/badge/Media3-ExoPlayer-FF6F00?style=flat-square&logo=youtube&logoColor=white)
![Clean Architecture](https://img.shields.io/badge/Architecture-Clean_%2B_Multi--Module-00C853?style=flat-square)

</div>

## 🚀 Key Features

- **Multi-Platform Support**: Tailored experiences for Mobile and **Android TV** devices with D-pad navigation support.
- **YouTube-Style Quality Manager**: Advanced video quality selection (Auto, High Quality, Data Saver, and custom HLS resolutions).
- **High-Quality Streaming**: Integrated with **Android Media3 (ExoPlayer)** for smooth HLS and DASH video playback.
- **Video Sequences & Recovery**: Operator banners, Next Episode auto-play, Skip Credits, and automatic network loss recovery overlay.
- **Rewards & Loyalty System**: Daily rewards, coin inventory, Lucky Wheel with server-driven win determination, and shopping history.
- **Dynamic UI**: Built entirely with **Jetpack Compose** following **Material 3** design guidelines.
- **Multi-Store Support**: Specialized build flavors for **Cafe Bazaar**, **Myket**, and direct integration via **Zarinpal**.
- **Kids Mode**: Dedicated interface and module for children's content (`:kids` and `:kids-tv`).
- **Advanced Search & Custom TV Keyboard**: Real-time search with filtering capabilities and custom TV remote-friendly keyboard.
- **Offline Capabilities**: Local caching using **Room Database** for a smooth offline-to-online transition.

---

## 🏗 Project Architecture & Multi-Module Setup

The project follows **Clean Architecture** principles and is structured into multiple modules for optimal scalability:

```
ronak_film/
├── :core       # Shared domain logic, repositories, networking, database, themes & dimensions
├── :app        # Main Mobile application
├── :tv         # Main Android TV application
├── :kids       # Kids Mobile application
└── :kids-tv    # Kids Android TV application
```

- **`:core`**: Shared utilities, base activities (`BaseActivity`), networking configurations (Retrofit/Kotlinx Serialization), database, logging, and common ViewModels.
- **`data`**: Implementation of repositories, remote API services, and local data sources.
- **`domain`**: Business logic, use cases, and repository interfaces.
- **`presentation`**: Feature-specific UI components, screen layouts, and themes.

---

## 🛠 Tech Stack & Libraries

### Core & UI
- **Kotlin**: Primary programming language.
- **Jetpack Compose**: Declarative UI toolkit with Material 3 design system.
- **Coil**: Image and thumbnail loading with custom state handlers.
- **Konfetti & Shimmer**: Enhanced UI animations and skeleton loading.

### Architecture & DI
- **Clean Architecture + MVVM**: Clear separation of concerns.
- **Hilt (Dagger)**: Dependency injection across all sub-modules.
- **Coroutines & Flow**: Asynchronous streams and reactive state handling.

### Data & Networking
- **Retrofit & OkHttp**: Type-safe HTTP client.
- **Kotlinx Serialization**: JSON parsing and serialization.
- **Room Database**: SQLite object mapping for offline persistence.
- **DataStore**: Modern key-value storage.
- **Paging 3**: Paginated data loading.

### Media & Services
- **Android Media3 (ExoPlayer)**: Modern video playback engine.
- **Firebase FCM**: Cloud messaging and push notifications.
- **Poolakey (Cafe Bazaar)**: In-app billing client integration.
- **Adivery (Yektanet)**: Monetization and ad integration SDK.

---

## ⚙️ Development & Build

### Build Flavors
The project utilizes Gradle flavors for distribution channels:
- `cafebazaar`: Integrated with Bazaar's In-App Billing (Poolakey).
- `myket`: Integrated with Myket Billing Client.
- `zarinpal`: Direct payment gateway integration via Zarinpal.

### Environment Setup
To build the project locally, configure the following keys in `local.properties`:
```properties
API_TOKEN=your_api_token
MY_API_ADDRESS=your_api_base_url
BAZAR_RSA_TOKEN=your_bazaar_rsa_key
MYKET_RSA_TOKEN=your_myket_rsa_key
ADIVERY_APP_ID=your_adivery_app_id
```

---

## 📄 License & Ownership (لایسنس و مالکیت معنوی)

تمامی حقوق مادی و معنوی این پروژه متعلق به **شرکت ارتباط گستران روناک** می‌باشد.

Copyright © 2026 **Ertebat Gostaran Ronak Co.** All rights reserved.

This software and associated documentation files are proprietary and confidential. Unauthorized copying, distribution, or modification of this file, via any medium, is strictly prohibited.

---

<div align="center">

**توسعه داده شده توسط تیم فنی شرکت ارتباط گستران روناک**

</div>
