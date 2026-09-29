# Hyperframes Composition Brief: InRent

## Objective
A 20s vertical (1080x1920) cinematic-polished product film for **InRent**, a student-
accommodation marketplace for Botswana. The phone running the real app is the hero; the film
walks the real flow: Browse verified rentals → Request to book → "Booking request sent!".

## Output
- Composition dir: `brag-output/` (this project) · Render: `brag-output/brag.mp4`
- Format: vertical 9:16 — 1080x1920 · Duration: 20s

## Source Material
- Project: `inrent_flutter` (Flutter). Screens: `marketplace_screen`, `property_detail_screen`,
  `booking_confirmation_screen`, `welcome_screen`. Palette: `core/constants/app_colors.dart`.
- Copy that must appear verbatim (from the app):
  - "Search near your campus" (search field intent), "P2,500/mo", "Verified", "1 bed"
  - "per month", "Book a viewing", "Request to book"
  - "Booking request sent!", "The landlord will respond within 24 hours.",
    "Awaiting landlord", "Find your perfect student home."
- Real asset: `assets/img/logo.png` (teal house+person mark + inRent wordmark) — use in outro.

## Creative Direction
- Tone: cinematic + polished blend — calm, premium consumer film; warm friendly marketplace feel.
- 5 scenes, unhurried holds, soft slides, one clean success beat. Light palette, lots of air.
- Hook: "Student housing in Botswana — without the guesswork." Outro: the real logo + "Find
  your perfect student home." + "Verified rentals near your campus · Botswana 🇧🇼".
- Avoid generic SaaS language, abstract filler, and redesigning the app's look.

## Visual Identity (light theme, from the app)
- Teal #00BFA5 (dark #00897B, light #4DD0C4, surface #E0F7F4) · bg #F8F9FA · white cards ·
  border #E5E7EB · text #1A1A2E / #6B7280 / #9CA3AF · amber chip #FFF7E0/#92400E · Pula "P2,500".
- System sans, bold display. The app UI is recreated inside a clean phone frame.

## Storyboard
Contract = `brag-output/brag-plan.md`. Scenes:
1. Hook 3.3s — teal wash + mark + line.
2. Browse 4.7s — phone: search + 2 verified cards slide in one by one.
3. Book 4.7s — phone: property detail + simulated tap on "Request to book".
4. Confirmed 4.0s — teal check + "Booking request sent!" + details card.
5. Outro 3.3s — real logo + "Find your perfect student home."

## Audio
- Music: `assets/music/happy-beats-business-moves-vol-11-by-ende-dot-app.mp3` (~115 BPM), vol ~0.30,
  fade in 0.5s / out under outro. Cue preset at `assets/music/cues/...vol-11...json`.
- Strong-cue targets: ~3.70s phone reveal, ~5.8/6.9s card arrivals (beat grid), ~8.96s tap,
  ~12.65s success check, ~17.91s logo. Lock 1–2; readability wins.
- SFX (light, app-store): `interface/drop_001`+`drop_002` (cards), `ui/click1` (tap),
  `impact/impactSoft_medium_000` (success). Vol 0.5–0.65.
- Subtle audio-reactive teal glow if trivial; else document skip. Local relative paths only.
- Gate: `npx hyperframes check` must pass before render.
