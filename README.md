# CoverUp 📚

A multi-user study progress tracker built to help PSC aspirants organize subjects, track subtopics, and monitor syllabus completion.

## Features
- Subject-wise study tracking
- Subtopic progress tracking
- Page-based progress
- Overall and subject-level progress indicators
- Multi-user data storage with Supabase
- Android app built with Capacitor

## Project layout
- `www/` — app web interface (HTML, CSS, JavaScript)
- `android/` — Capacitor Android project
- `capacitor.config.json` — Capacitor configuration

## Requirements
- Node.js and npm
- Android Studio and Android SDK (for building the Android app)

## Setup
1. Clone this repository.
2. Run `npm install` in the project root.
3. Open `www/app.js` and configure your Supabase project URL and publishable/anon key if required. Never add Supabase service-role/secret keys.
4. Run `npx cap sync android`.
5. Open the Android project with Android Studio using the `android/` folder and build/run the app.

## Security note
Supabase client-side keys are not a substitute for database security. Configure Row Level Security (RLS) policies on all user-data tables so users can access only their own records. Review the policies before using this app with real users.

## License
MIT license (see `LICENSE`).
