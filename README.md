<div align="center">
  <img src="assets/app_icon.png" alt="SKLR Logo" width="120" />

  # SKLR

  ### Share · Learn · Repeat

  [![Flutter](https://img.shields.io/badge/Flutter-02569B?style=for-the-badge&logo=flutter&logoColor=white)](https://flutter.dev)
  [![Dart](https://img.shields.io/badge/Dart-0175C2?style=for-the-badge&logo=dart&logoColor=white)](https://dart.dev)
  [![Supabase](https://img.shields.io/badge/Supabase-3FCF8E?style=for-the-badge&logo=supabase&logoColor=white)](https://supabase.com)
  [![PostgreSQL](https://img.shields.io/badge/PostgreSQL-4169E1?style=for-the-badge&logo=postgresql&logoColor=white)](https://www.postgresql.org)
  [![Figma](https://img.shields.io/badge/Figma-F24E1E?style=for-the-badge&logo=figma&logoColor=white)](https://www.figma.com/design/89T97CQIlNzEuWu7WIvWpq/SKLR_Group1?node-id=0-1&t=rwyJmYOgasuW5eAQ-1)

  <br/>

  > _A skill-based economy app where your talent is the currency._
  >
  > List your skills, discover others, book sessions, and exchange knowledge — all through an in-app credit system.

  <br/>

  **[Explore the Figma Design »](https://www.figma.com/design/89T97CQIlNzEuWu7WIvWpq/SKLR_Group1?node-id=0-1&t=rwyJmYOgasuW5eAQ-1)**

</div>

<br/>

---

## 📖 About

**SKLR** is a cross-platform mobile marketplace that connects people through their skills. Instead of traditional payments, users earn and spend **credits** by teaching and learning from each other — whether that's photography, coding, cooking, music, or anything in between.

The app fosters a community-driven ecosystem where continuous learning meets real-world demand.

<br/>

## ✨ Features

| | Feature | Description |
|---|---|---|
| 💬 | **Real-Time Chat** | Instant messaging powered by Supabase Realtime — syncs messages across devices instantly |
| 🔍 | **Smart Skill Discovery** | Browse by category, search services, and view popular listings with a polished home feed |
| 💳 | **Credit Economy** | Automated credit transfers on session completion, cancellation, and refunds via PostgreSQL triggers |
| 🔐 | **Multi-Method Auth** | Email, phone (OTP), and Apple Sign-In — with email verification and "Remember Me" |
| 👤 | **Rich User Profiles** | Profile pictures (cloud-stored), dashboards, skill portfolios, ratings & reviews |
| 🛡️ | **Content Moderation** | Built-in moderation tools to keep the marketplace safe and trustworthy |
| 📱 | **Cross-Platform** | Single codebase targeting Android, iOS, Web, Windows, macOS, and Linux |
| 🌍 | **Multi-Language Support** | Language selection for a global user base |
| 🔔 | **Notification Controls** | Granular notification preferences so users stay in control |
| 🆘 | **In-App Support** | Dedicated support finder and help pages |

<br/>

## 🏗️ Architecture

```
lib/
├── main.dart                 # App entry point, Supabase init, auth routing
├── Auth/                     # Login, register, OTP, email verification, password reset
├── Chat/                     # Real-time messaging & chat session management
├── Home/                     # Home feed, categories, search, popular services
├── Skills/                   # Skill creation, listings, orders, moderation
├── Profile/                  # User profiles, dashboards, edit profile, avatars
├── Support/                  # In-app help & support finder
├── Util/                     # Splash screen, start page, navigation bar, privacy policy
└── database/                 # Supabase service layer, DB helpers, presence, models
```

<br/>

## 🛠️ Tech Stack

<div align="center">

| Layer | Technology | Purpose |
|:---:|:---:|:---|
| **Frontend** | Flutter + Dart | Cross-platform UI with a single codebase |
| **Backend** | Supabase | Auth, Realtime DB, Storage, Edge Functions |
| **Database** | PostgreSQL | Relational data + automated credit triggers |
| **Design** | Figma | UI/UX planning & prototyping |
| **Storage** | Supabase Storage | Profile pictures & listing images (cloud buckets) |

</div>

### Notable Libraries

`supabase_flutter` · `google_fonts` · `shimmer` · `image_picker` · `flutter_rating_bar` · `country_picker` · `pin_code_fields` · `sign_in_with_apple` · `shared_preferences`

<br/>

## 🚀 Getting Started

### Prerequisites

- [Flutter SDK](https://docs.flutter.dev/get-started/install) `>=3.6.0`
- Dart SDK (bundled with Flutter)
- A Supabase project (or use the existing config)

### Installation

```bash
# Clone the repository
git clone https://github.com/NadimBaboun/sklr.git
cd sklr

# Install dependencies
flutter pub get

# Run the app
flutter run
```

<br/>

## 🗄️ Database

The backend uses **Supabase (PostgreSQL)** with:

- **Users** table with credit balances
- **Skills** and **Categories** for the marketplace
- **Sessions** and **Transactions** for booking flow
- **PostgreSQL triggers** that automatically handle credit transfers:
  - **Completed** → credits transferred to the provider
  - **Cancelled / Declined** → credits refunded to the requester

<br/>

## 👥 Team

<table>
  <tr>
    <td align="center"><strong>Nadeem Baboun</strong><br/><sub>UI Overhaul · Chat System</sub></td>
    <td align="center"><strong>Mohammad Hamarsheh</strong><br/><sub>UI Design · Gemini 2 Integration · Database</sub></td>
    <td align="center"><strong>Mohammad Al-Masri</strong><br/><sub>Development</sub></td>
  </tr>
</table>

<br/>

---

<div align="center">

  **Built with ❤️ at Mälardalen University**

  <br/>

  [![Email](https://img.shields.io/badge/Contact-nbn24004%40student.mdu.se-blue?style=flat-square&logo=gmail&logoColor=white)](mailto:nbn24004@student.mdu.se)

nbn24004@student.mdu.se">Contact Me</a> •  
</div>