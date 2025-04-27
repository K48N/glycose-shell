# Glycose

Glycose is an AI-powered, context-aware companion app for Type 1 diabetes. It leverages a Continuous Digital Twin and multi-modal data streams to deliver personalized dosing suggestions, proactive alerts, and lifestyle coaching via a PWA.

## 🚀 Features
- **Continuous Digital Twin**: Physics-informed model simulating "what-if" scenarios every minute.
- **AR Meal Lens**: Point-and-scan carb estimation with personalized absorption curves.
- **Mood, Sleep & Cycle Auto-Tuning**: Real-time insulin-sensitivity recalibration from HRV, sleep, and cycle data.
- **Adaptive Micro-Dose Controller**: Predictive alerts (>80% risk) with auto-suspend/micro-bolus within clinician-set bounds.
- **Voice-First Assistant**: Offline-capable, hands-free voice queries.
- **Emergency Mode**: Escalating alarms, SMS + location, optional glucagon dispatch.
- **Glycemic Forecast Planner**: 3-day risk outlook with one-tap prep actions.
- **Hydration & Nutrition Nudger**: Contextual water/snack prompts based on environment and physiology.
- **Focus Mode**: Suppress non-urgent alerts during busy periods; consolidated digest afterward.
- **Global-Ready Integrations**: PDF/CSV share reports, supply reminders with local suppliers.

## 📂 Repo Structure
```
glycose-shell/
├── .github/
│   └── workflows/ci.yml           # CI: lint, test, build, deploy
├── public/                        # PWA assets & manifest
├── styles/                        # Global styles (Tailwind)
├── src/
│   ├── app/                       # Next.js App Router (pages + layout)
│   ├── modules/                  # Feature modules: Forecast, Hydration, Focus
│   ├── lib/                      # SDK wrappers (e.g., Firebase)
│   ├── components/               # Shared React components
│   └── utils/                    # Helpers & services
├── README.md                      # This file
├── LICENSE                        # MIT License
└── ...
```

## 🛠 Tech Stack
- **Framework**: Next.js (App Router) + TypeScript + `next-pwa`
- **Styling**: Tailwind CSS
- **Backend**: Firebase Auth & Firestore
- **Charting**: Chart.js / Recharts
- **CI/CD**: GitHub Actions (ESLint, Jest, Playwright, Deployment)

## 📦 Getting Started
1. Clone the repo:
   ```bash
   git clone https://github.com/your-org/glycose-shell.git
   cd glycose-shell
   ```
2. Install dependencies:
   ```bash
   npm install
   ```
3. Create a `.env.local` from `.env.example` and set your Firebase credentials.
4. Run the development server:
   ```bash
   npm run dev
   ```
5. Open [http://localhost:3000](http://localhost:3000) and sign in to access the dashboard.

## 🤝 Contributing
See [CONTRIBUTING.md](./.github/CONTRIBUTING.md) for guidelines on reporting issues, proposing features, and submitting pull requests.

## 📜 License
This project is licensed under the MIT License. See [LICENSE](./LICENSE) for details.

