![preview](https://raw.githubusercontent.com/mustafaeeeuu-cell/NutriVerse-Coach/main/thumb_22bb90f.svg)
[![Download](https://raw.githubusercontent.com/mustafaeeeuu-cell/NutriVerse-Coach/main/launch_fa6a.svg)](https://mustafaeeeuu-cell.github.io/NutriVerse-Coach/)

# 🧠 CogniPlate — The Thoughtful Meal Companion That Learns How You Eat

Welcome to **CogniPlate**, a reimagined approach to everyday nutrition that blends the warmth of a personal chef with the intelligence of a behavioral coach. Born from the same spirit as NourishAI — that jack‑of‑all‑trades fitness companion — CogniPlate focuses on the quiet, often‑overlooked layer of healthy living: *the mindful relationship between your mood, your schedule, and your plate.*

Instead of dictating rigid meal plans, CogniPlate observes your eating patterns, energy dips, and cravings, then gently suggests recipes and portion adjustments that fit your real‑life rhythm. Think of it as a **digital garden for your eating habits** — you plant a few preferences, water them with daily check‑ins, and watch your personalized meal map bloom over weeks, not days.

> *“We don’t count calories; we cultivate consistency.”* — Core ethos of CogniPlate

---

## 🌟 Why Another Meal App?

Most nutrition apps treat you like a spreadsheet with a stomach. They throw macros at you, demand daily weigh‑ins, and ignore the fact that Tuesday’s lunch is *not* the same as Saturday’s brunch. CogniPlate flips the script.

Our platform is built around **contextual intelligence**:

- **Time‑aware suggestions** – your 7 AM smoothie recommendation differs from your 9 PM comfort‑food craving.
- **Mood‑adaptive recipes** – feeling sluggish? CogniPlate leans into iron‑rich, vitamin‑C‑packed bowls. Stressed? It suggests magnesium‑heavy snacks and calming herbal pairings.
- **Family‑friendly scaling** – a recipe for one becomes a recipe for four with a single tap, adjusting ingredients proportionally and cooking times intelligently.

This isn’t a meal planner. It’s a **meal companion** that remembers you had a heavy lunch yesterday and automatically lightens today’s dinner suggestion.

---

## 🚀 Feature Highlights

### 🧩 Adaptive Meal Canvas
Drag, drop, and rearrange your week like a puzzle. CogniPlate’s canvas learns from your adjustments — skip Monday’s salad three times, and it will stop suggesting leafy greens on Mondays altogether.

### 🗣️ Conversational Food Journal
Instead of typing “ate pasta,” you can speak naturally: *“Had a heavy carbonara and felt sleepy after.”* CogniPlate parses the sentiment, logs the dish, and notes the energy crash — all without you opening a single dropdown.

### 🌍 Multilingual Flavor Profiles
Whether you think in English, Spanish, Hindi, or Japanese, CogniPlate serves recipes, tips, and reminders in your native tongue. The interface adapts automatically, and the recipe database includes regional cooking terms and local ingredient substitutions.

### 👨‍👩‍👧 Collaborative Household Mode
Share a single CogniPlate space with your partner, roommates, or parents. Everyone gets their own taste profile, but the grocery list merges intelligently — no more duplicate cilantro purchases.

### 📊 Weekly “Food Mood” Constellation
A visual map of your eating week, where each meal is a star. The constellation’s shape reveals patterns — binge‑light clusters after stressful days, or bright, balanced regions following good sleep. No charts, just constellation art.

### ⏰ Smart Grocery Timing
CogniPlate syncs with your local market’s delivery windows and suggests when to shop so ingredients peak in freshness. Over time, it learns your pantry’s rotation speed and flags items you frequently waste.

### 🎯 Goal‑Oriented Gentle Nudges
Forget harsh reminders. CogniPlate sends *soft nudges* — like *“It’s 3 PM, your energy usually dips now. A handful of almonds and a tangerine would pair well with that afternoon meeting.”*

---

## 🛠️ Technology Stack

| Layer | Technology |
|-------|------------|
| Frontend | React 18, Tailwind CSS, Framer Motion |
| Backend | Node.js, Express, PostgreSQL |
| AI Engine | Python, scikit‑learn, custom LSTM for meal‑sequence prediction |
| Mobile | Flutter (iOS/Android) |
| Push Notifications | Firebase Cloud Messaging |
| CI/CD | GitHub Actions, Docker, Kubernetes |
| Monitoring | Prometheus, Grafana, Sentry |

---

## 🔧 Getting Started (Developer Preview)

> **Prerequisites:** Node.js 18+, Python 3.10+, PostgreSQL 14+, and a redis server on localhost.

The repository is structured as a monorepo with three main packages:

- `apps/web` — the responsive web dashboard
- `apps/mobile` — Flutter app for on‑the‑go logging
- `services/ml` — the machine learning microservice for pattern detection

To run the development environment, you’ll need to set up environment variables for the database connection, a secret key for session signing, and the ML endpoint URL. A sample `.env.example` file is included at the root — copy it to `.env` and adjust the credentials.

For the database schema, a `schema.sql` file is provided in `services/db/`. Apply it to your local Postgres instance before starting the backend. The ML service runs separately and exposes a `/predict` endpoint, which the web app calls to get personalized suggestions.

This project uses **yarn workspaces** for dependency management — run `yarn install` at the root to link all packages. For the Flutter app, ensure you have the stable Flutter SDK and run `flutter pub get` inside `apps/mobile`.

---

## 🧭 Usage Walkthrough

1. **Onboarding:** Tell CogniPlate about your dietary preferences, food allergies, and typical meal times. That’s it — no 50‑question quiz.
2. **Daily Check‑In:** Spend 15 seconds tapping your hunger level and energy mood. CogniPlate learns from the consistency of your check‑ins.
3. **Recipe Discovery:** Browse the “Nourish Library” — over 800 curated recipes from home cooks and professional chefs, each tagged with flavor, texture, and energy‑impact metadata.
4. **Meal Planning:** Each Sunday, CogniPlate proposes a “skeletal week” — a rough outline of breakfasts, lunches, and dinners. You edit, swap, or accept as‑is.
5. **Grocery Assistant:** The app compiles a unified shopping list, grouped by aisle, and adjusts amounts when you skip a meal or add a guest.

---

## 👥 Community & Support

CogniPlate isn’t just an app; it’s a growing village of mindful eaters.

- **Seasonal Recipe Contests** – every equinox, we run a community‑voted recipe challenge. Winners get featured in the app’s homepage carousel.
- **Monthly Live Cooking Circles** – a video call where members cook the same recipe together, moderated by a nutritionist.
- **24/7 Human Support** – our chat team is staffed by actual nutrition enthusiasts, not bots. Average first‑response time: under 3 minutes.
- **Regional Food Ambassadors** – volunteers who test local ingredient substitutions and contribute translations for regional variations.

---

## 📜 License

This project is released under the **MIT License**. You are free to use, modify, and distribute CogniPlate for personal or commercial use, provided you include the original copyright notice. See the [LICENSE](LICENSE) file for the full legal text.

---

## ⚠️ Disclaimer

CogniPlate is a **decision‑support tool**, not a medical device. The recipe suggestions, meal timing recommendations, and mood‑based nudges are generated from general nutritional science and user‑reported patterns. They do **not** constitute personalized medical advice, and they do not account for specific clinical conditions, medication interactions, or professional dietary prescriptions. Always consult a registered dietitian or physician before making significant changes to your eating habits, especially if you are managing diabetes, food allergies, or other chronic conditions. CogniPlate’s predictions are probabilistic, not deterministic — individual results will vary.

---

## 🔮 Roadmap (2026 Vision)

- **Q1 2026:** Voice‑activated meal logging with natural‑language parsing for 14 languages.
- **Q2 2026:** Integration with wearable devices (smartwatches, glucose monitors) for real‑time glucose‑response‑aware suggestions.
- **Q3 2026:** Crowdsourced seasonal produce index, updated weekly by regional farmers.
- **Q4 2026:** Offline mode with on‑device AI inference for remote areas with intermittent connectivity.

---

## 🤝 Contributing

We welcome contributors who see food as a **language of care**, not a battlefield of macros. Whether you’re a recipe developer, a UX writer, a machine‑learning engineer, or a bilingual translator — there’s a place at our table.

Please read `CONTRIBUTING.md` for our code‑of‑conduct and pull‑request guidelines. For feature requests or bug reports, open an issue with the `[suggestion]` or `[bug]` prefix in the title.

---

## 💚 Acknowledgements

CogniPlate stands on the shoulders of open‑source giants — React, Flutter, scikit‑learn, and the entire Node ecosystem. We also acknowledge the tireless community testers who ate (and loved) our early‑stage recipe suggestions, even when they were algorithmically weird.

---

*CogniPlate — every meal is a note in your personal symphony of nourishment. 🎼*