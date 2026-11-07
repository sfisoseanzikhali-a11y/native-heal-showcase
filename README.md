# Native Heal — Healing & Wellness Marketplace

> **Showcase repository.** The source code is private (client project). This page describes the platform and my role in building it. A live walkthrough is available on request — see [Contact](#contact).

🌐 **Live at [nativeheal.co.za](https://nativeheal.co.za)**

Native Heal is a South African marketplace that connects people with healing and wellness practitioners. I took over an incomplete codebase as the **software developer** and built it into a live production platform.

---

## At a glance

| | |
|---|---|
| **Role** | Software Developer (via Zikhali Solutions) |
| **Timeline** | 2026 – present |
| **Users** | 50 practitioners · 200 users |
| **Frontend** | React + Vite, TypeScript (single-page app) |
| **Backend & data** | Supabase (PostgreSQL, Edge Functions), SQL |
| **Integrations** | Daily.co video consultations, Paystack payments, Twilio, Google Maps (Places, Geocoding) |
| **Security** | Role- and approval-based access control, CSP and security headers, locked-down CORS |
| **Hosting** | Vercel |

---

## What I built

### Taking over an unfinished codebase
I inherited a partially built project, got it running, learned its structure and built out the platform's features and UI to reach a production launch.

### Backend and database
I built and integrated backend APIs and wrote SQL directly against the Supabase/PostgreSQL database, including working with JSONB data for practitioner profiles.

### Security and access control
I strengthened platform security with authentication and role- and approval-based access control, so each type of user can only see and do what their role allows.

### Video consultations
Clients can hold live video consultations with practitioners directly on the platform, built on Daily.co.

### Integrations
I integrated Paystack for payments, Twilio for messaging, and Google Maps for address autocomplete and geocoding. Sensitive server-side logic runs in Supabase Edge Functions, so secret keys never reach the browser.

### Production hardening
- **Content-Security-Policy and security headers** configured on Vercel.
- **CORS locked down** so Edge Functions only accept requests from the production domain.
- **Browser-exposed API keys restricted** by HTTP referrer and to only the APIs in use, with billing alerts as a backstop.

### SEO for a single-page app
Single-page apps are hard for search engines to read. I added middleware that serves pre-rendered snapshots to crawlers and proxies a generated sitemap, so practitioner pages can be indexed.

### Debugging production issues
I diagnosed and fixed JSONB serialisation bugs that were breaking profile updates — tracing the problem from the UI through the API to how data was being stored.

### Release workflow
I own the Git branching and release process, including recovering production after an accidental merge to main.

---

## Features

<!-- Fill in the main features, for example: -->
- Live video consultations between clients and practitioners
- [Practitioner profiles and listings]
- [Search / browse by service or location]
- [Practitioner sign-up and admin approval]
- [Admin dashboard]

---

## Screenshots

<img width="1892" height="972" alt="image" src="https://github.com/user-attachments/assets/eb79f60a-e233-4459-8414-d5727209ee17" />


---

## What I'm working on next

- Automated test coverage for authentication, access control and profile updates
- 

---

## Contact

The source code is private. I'm happy to give a live walkthrough of the platform and how it's built.

**Sifiso Zikhali** · [sfisoseanzikhali@gmail.com](mailto:sfisoseanzikhali@gmail.com) · [LinkedIn](https://linkedin.com/in/sifiso-zikhali-5b1660230)
