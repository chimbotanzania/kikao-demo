# KIKAO — Interactive UI Prototype
### *Meet With The Lost Ones*

A fully responsive, front-end-only HTML prototype for **KIKAO**, an AI-powered reunification platform. Built for client, investor & stakeholder demos — no backend, no build step, no dependencies. Just open `index.html`.

---

## ▶️ How to run

**Option A — double-click:** open `index.html` in any modern browser.

**Option B — local server** (recommended, avoids any browser file:// quirks):

```bash
npx serve .          # then open http://localhost:3000
# or
python -m http.server 8000
```

---

## 🗺️ Pages (18)

| Page | File | Highlights |
|------|------|-----------|
| Landing | `index.html` | Hero, features, stats, screenshots, testimonials, pricing, FAQ, footer |
| Login | `login.html` | Zauthy branding · Email / Phone / OTP / Google / Apple |
| Dashboard | `dashboard.html` | AI matches, alerts, recent searches, notifications, quick actions |
| Search People | `search.html` | Name + photo search, AI suggestions, filters, history, skeletons |
| AI Matches | `ai-matches.html` | Confidence bars & badges, category filters |
| Interactive Map | `map.html` | Pins, satellite toggle, radius, share/copy/navigate |
| Missing Child Alert | `child-alert.html` | Amber alert, clothing, nearby map, report sighting |
| Lost Person Profile | `profile-lost.html` | Photos, timeline, last-seen map, story, contact |
| SOS Emergency | `sos.html` | Live SOS button, trusted contacts, emergency timeline |
| Reunion Stories | `stories.html` | Social feed: photos, likes, comments, shares |
| KIKAO Vault | `vault.html` | Albums, photos, videos, documents + secure sharing |
| Album Sharing | `album-share.html` | Private / Selected / Family / Trusted, expiring links |
| Family Vault | `family-vault.html` | Members, family tree, shared memories |
| Messaging | `messages.html` | Conversations, images, voice notes, location, requests |
| Notifications | `notifications.html` | Match / alert / SOS / social / vault, filterable |
| Premium | `premium.html` | Plans, monthly/yearly toggle, comparison table |
| User Profile | `profile.html` | Cover, avatar, bio, timeline, privacy, contacts |
| Admin Dashboard | `admin.html` | KPIs, charts, AI usage, storage, moderation queue |

### v2 modules (Client Demo update)

| Page | File | Highlights |
|------|------|-----------|
| Missing Persons | `cases.html` | Command centre: active cases, sightings, charts, live map, poster generator |
| Global Search | `global-search.html` | Search by name, school, village, region, photo & voice; AI similarity scores |
| Trust Before Contact | `trust-journey.html` | 7-step journey keeping the user in control of personal data |
| Safe Meeting | `safe-meeting.html` | Countdown, route, weather, parking, transport, "Start Safe Meeting" |
| Live Audio Rooms | `audio-rooms.html` | Social audio: categories, speakers, raise hand, become speaker |
| Video Meeting | `video-meeting.html` | Participant grid, controls, chat, waiting room, recording, screen share |
| Reunion Planner | `reunion-planner.html` | RSVP, guest list, timeline, budget, checklist, seating, countdown |
| Reunion Groups | `groups.html` | Feed, chat, events, polls, albums, members, AI-assisted planning |
| Family Tree | `family-tree.html` | Interactive multi-generation tree, click for profile preview |
| Trust & Safety | `trust-score.html` | Trust score gauge, verification indicators, safety tips |
| Digital Legacy | `legacy.html` | Legacy contacts, albums, inheritance settings, family access |
| Privacy & Consent | `privacy.html` | Consent controls, AI transparency, data export & deletion |
| Device Preview | `mobile-preview.html` | Interactive iPhone / Android / tablet / desktop mockups |

### Global additions
- **Floating AI Assistant** — on every signed-in page (bottom-right): proactive suggestions, chat, contextual deep-links.
- **Consent Wizard** — shown on signup (and from Privacy page): choose which optional features to enable.
- **"Demo preview" badge** — persistent reminder that all data is fictional.
- Landing page gained **Safety First, Privacy & Consent, NGO & Volunteer Partnerships, Trusted by Families** sections.
- Vault gained **Children, School Memories, Business, Legal Documents** albums, **Recent Uploads**, and an **Invitation Only** permission.
- Premium gained **Larger Video Meetings, Advanced Family Tree, Digital Legacy, Priority Support**.

---

## 📁 Structure

```
KIKAO/
├── index.html ... admin.html      # 18 linked pages
├── README.md
└── assets/
    ├── css/styles.css             # Design system (glassmorphism, light/dark, responsive)
    ├── js/app.js                  # Shared shell, icons, theme, toasts, modals, counters
    ├── js/media.js                # Self-contained SVG avatar & photo generator
    └── img/logo.svg, logo-mark.svg
```

## ✨ Built in

- **Light / Dark mode** — toggle in the top bar (persists via localStorage)
- **Responsive** — mobile, tablet & desktop; sidebar collapses to a drawer
- **Glassmorphism** design, animated counters, scroll reveals, loading skeletons, FABs, toasts, modal dialogs
- **Reusable components** — one shared CSS + JS framework powers every page
- **100% offline** — all avatars/photos are generated as inline SVG; no external image, font CDN fallback, or API calls required to function

## 📝 Notes for stakeholders

All data is **fictional sample data**. AI match scores are presented as *possibilities, not certainties* throughout. This is a visual prototype: buttons simulate behaviour with toasts and modals — there is no real authentication, storage, or matching engine behind it yet.

---
*© 2026 KIKAO · Prototype for demonstration purposes.*
