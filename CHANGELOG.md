# Changelog — Bionetic Landing (Wariant 2)

> Format zgodny z [Keep a Changelog](https://keepachangelog.com/) ·
> projekt stosuje [Semantic Versioning](https://semver.org/).

---

## 🇵🇱 Wersja polska

### [1.0.1] — 2026-05-13

#### Zmienione
- **Refaktoryzacja struktury plików.** Zawartość `<style>` i `<script>`
  z `index.html` została wyodrębniona do osobnych modułów w katalogach
  `css/` i `js/`, zgodnie z układem wariantu 1.
- `index.html` zawiera teraz wyłącznie znaczniki HTML oraz odwołania do
  zewnętrznych plików.
- Style podzielone na trzy pliki: `base.css` (tokeny, reset, typografia,
  przyciski), `components.css` (header, footer, modale, formularze, polityki)
  i `sections.css` (sekcje strony + responsywność).
- JavaScript podzielony na trzy moduły IIFE: `cart.js` (koszyk + publiczne API
  `window.BioneticCart`), `ui.js` (UI globalne) i `main.js` (logika sekcji).

#### Naprawione
- Drobne literówki językowe — kilka łańcuchów w litewskim wariancie
  zastąpiono poprawnymi formami łotewskimi (`Krepšelis tuščias` →
  `Grozs ir tukšs`, `Iš viso` → `Kopā`, `Apmokėti` → `Apmaksāt`,
  `Prisijungti/Registruotis` → `Pieslēgties/Reģistrēties`,
  `Nieko nerasta` → `Nekas nav atrasts`, `Demo paskyra` → `Demo konts`).

### [1.0.0] — 2026-05-13

#### Dodane
- Pierwsza wersja wariantu 2 strony marki Bionetic.
- Pełna treść w języku łotewskim, dostosowana do rynku Łotwy.
- Alternatywna paleta (sage green + clay terracotta) i typografia
  (Fraunces + DM Sans) — wyraźnie odróżniająca wariant 2 od wariantu 1.
- Sekcje: ogłoszenie, header z wycentrowanym logo, hero (editorial split),
  pasek zaufania, karta produktu, benefity (4 kafelki), spotlight składników
  (alternujące rzędy), "Jak stosować" (4 kroki), historia założycielki,
  tabela porównawcza salon/dom, ściana opinii, doświadczenie 4 tygodni,
  FAQ, kontakt, newsletter, footer.
- Koszyk z trwałym `localStorage` (klucz `bionetic_cart_v2`).
- Modal wyszukiwania + modal konta (logowanie / rejestracja demo).
- Pełnoekranowe polityki (Privacy, Terms, Delivery, Refund) z routingiem
  URL (`?page=...`) oraz obsługą historii przeglądarki.
- Banner cookie z trwałą zgodą (`bionetic_cookie_ok_v2`).
- Walidacja JS dla formularza kontaktowego.
- SEO: meta description, canonical, OpenGraph, JSON-LD `LocalBusiness`
  z adresem Origo, Ryga.
- Responsywność: punkty graniczne 1024 / 768 / 480 px, testowane od 360 px.
- Dokumentacja `README.md`, `CHANGELOG.md`, `DELIVERY.md` (PL + EN).

---

## 🇬🇧 English version

### [1.0.1] — 2026-05-13

#### Changed
- **File structure refactoring.** Inline `<style>` and `<script>` content from
  `index.html` was extracted into separate modules under `css/` and `js/`
  directories, matching the variant-1 layout.
- `index.html` now contains only markup and references to external files.
- Styles split into three files: `base.css` (tokens, reset, typography,
  buttons), `components.css` (header, footer, modals, forms, policies),
  and `sections.css` (page sections + responsive).
- JavaScript split into three IIFE modules: `cart.js` (cart + public
  `window.BioneticCart` API), `ui.js` (global UI), and `main.js`
  (section logic).

#### Fixed
- Minor copy fixes — a few Lithuanian strings were replaced with proper Latvian
  forms (`Krepšelis tuščias` → `Grozs ir tukšs`, `Iš viso` → `Kopā`,
  `Apmokėti` → `Apmaksāt`, `Prisijungti/Registruotis` →
  `Pieslēgties/Reģistrēties`, `Nieko nerasta` → `Nekas nav atrasts`,
  `Demo paskyra` → `Demo konts`).

### [1.0.0] — 2026-05-13

#### Added
- Initial release of variant 2 of the Bionetic brand page.
- Full content in Latvian, localized for the Latvian market.
- Alternative palette (sage green + clay terracotta) and typography
  (Fraunces + DM Sans) — clearly distinguishing variant 2 from variant 1.
- Sections: announcement bar, header with centered logo, hero (editorial
  split), trust strip, product card, benefits (4-tile grid), ingredient
  spotlight (alternating rows), "How to use" (4 steps), founder story,
  salon-vs-home comparison table, testimonials wall, 4-week experience,
  FAQ, contact, newsletter, footer.
- Cart persisted in `localStorage` (`bionetic_cart_v2`).
- Search modal + account modal (demo login / register).
- Fullscreen policy overlays (Privacy, Terms, Delivery, Refund) with URL
  routing (`?page=...`) and browser-history support.
- Cookie banner with persistent consent (`bionetic_cookie_ok_v2`).
- JS validation on the contact form.
- SEO: meta description, canonical, OpenGraph, JSON-LD `LocalBusiness` with
  the Origo, Riga address.
- Responsiveness: breakpoints at 1024 / 768 / 480 px, verified from 360 px.
- Documentation `README.md`, `CHANGELOG.md`, `DELIVERY.md` (PL + EN).
