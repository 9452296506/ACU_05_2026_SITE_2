# Bionetic — Landing Page

---

## 🇵🇱 Wersja polska

### Opis projektu

Statyczna strona docelowa (landing page) marki **Bionetic** — biokompleks do
pielęgnacji włosów, sprzedawany na rynku łotewskim.

Strona w całości w języku łotewskim. Treść, ceny i adresy dostosowane do
rynku Łotwy (Origo, Ryga).

### Specyfikacja techniczna

| Element             | Wartość                                                    |
|---------------------|------------------------------------------------------------|
| Język interfejsu    | Łotewski (`lang="lv"`)                                     |
| Stos technologiczny | HTML5, CSS3 (custom properties, Grid, Flexbox), vanilla JS |
| Typografia          | Fraunces (serif) + DM Sans (sans)                          |
| Paleta              | Sage green (`#3f5240`) + Clay terracotta (`#c97b63`)       |
| Ikony               | Font Awesome 6.5.1 (CDN)                                   |
| Wymagania serwera   | Brak — statyczne pliki                                     |

### Funkcjonalność

- Sticky header z efektem scroll
- Menu mobilne (szuflada boczna)
- Koszyk z trwałym `localStorage` (`bionetic_cart_v2`)
- Modal wyszukiwania z filtrowaniem
- Modal konta (logowanie / rejestracja, demo)
- Akordeon FAQ
- Pełnoekranowe polityki (Privacy, Terms, Delivery, Refund) z routingiem URL (`?page=...`)
- Walidacja formularza kontaktowego (JS)
- Formularz newslettera
- Baner cookie z trwałą zgodą (`bionetic_cookie_ok_v2`)
- Sekcja porównawcza (Salon vs Bionetic)
- Sekcja "4 tygodnie z produktem"

### SEO

- Meta description, canonical, OpenGraph
- JSON-LD `LocalBusiness` z adresem Origo
- Semantyczny HTML, atrybuty `alt` na obrazach
- `theme-color` dla mobilnych przeglądarek

### Struktura katalogu

```
├── index.html
├── css/
│   ├── base.css         (tokeny, reset, typografia, przyciski)
│   ├── components.css   (header, footer, modal, drawer, formularze, polityki)
│   └── sections.css     (hero, trust, produkt, benefity, składniki, how,
│                         founder, compare, reviews, experience, faq,
│                         contact, newsletter, responsive)
└── js/
    ├── cart.js          (koszyk + publiczne API window.BioneticCart)
    ├── ui.js            (header, menu, modale, FAQ, polityki, cookies, Esc)
    └── main.js          (search, walidacja kontaktu, newsletter, konto demo)
```

### Uruchomienie lokalne

To statyczna strona — wystarczy otworzyć `index.html` w przeglądarce lub
serwować dowolnym serwerem statycznym


### Responsywność

Punkty graniczne: **1024 px**, **768 px**, **480 px**. Strona została
zweryfikowana na typowych szerokościach mobile (360 px+), tablet i desktop.

### Status projektu

✅ **Wersja 1.0.0 — gotowa do wdrożenia produkcyjnego.**

### Polityka repozytorium

Niniejsze repozytorium publiczne zawiera **wyłącznie dokumentację oraz
zrzuty ekranu** mające potwierdzić wykonanie zlecenia (do celów rozliczeniowych
i podatkowych JDG).

Kompletny kod źródłowy znajduje się w **prywatnym repozytorium**, do którego
zleceniodawca otrzymuje bezpośredni dostęp w ramach przekazania projektu.
Szczegóły — w pliku `DELIVERY.md`.

---

## 🇬🇧 English version

### Project overview

A static landing page for the **Bionetic** brand — a biocomplex for hair care,
sold on the Latvian market. Variant **2** is an alternative visual treatment of
the same brand: a different color palette, different section layout and
different typography than variant 1.

The page is fully in Latvian. All content, prices and addresses are tailored
to the Latvian market (Origo, Riga).

### Technical specification

| Item             | Value                                                          |
|------------------|----------------------------------------------------------------|
| Interface lang   | Latvian (`lang="lv"`)                                          |
| Stack            | HTML5, CSS3 (custom properties, Grid, Flexbox), vanilla JS     |
| Typography       | Fraunces (serif) + DM Sans (sans)                              |
| Palette          | Sage green (`#3f5240`) + Clay terracotta (`#c97b63`)           |
| Icons            | Font Awesome 6.5.1 (CDN)                                       |
| Server reqs      | None — static files                                            |

### Functionality

- Sticky header with scroll behavior
- Mobile menu (slide-out drawer)
- Cart persisted in `localStorage` (`bionetic_cart_v2`)
- Search modal with filtering
- Account modal (login / register, demo)
- FAQ accordion
- Fullscreen policy overlays (Privacy, Terms, Delivery, Refund) with URL routing (`?page=...`)
- Contact form validation (JS)
- Newsletter form
- Cookie banner with persistent consent (`bionetic_cookie_ok_v2`)
- Comparison section (Salon vs Bionetic)
- "4-week experience" section

### SEO

- Meta description, canonical, OpenGraph
- JSON-LD `LocalBusiness` with Origo address
- Semantic HTML, `alt` on all images
- `theme-color` for mobile browsers

### Directory structure

```
site2/
├── index.html
├── css/
│   ├── base.css         (tokens, reset, typography, buttons)
│   ├── components.css   (header, footer, modal, drawer, forms, policy)
│   └── sections.css     (hero, trust, product, benefits, ingredients, how,
│                         founder, compare, reviews, experience, faq,
│                         contact, newsletter, responsive)
└── js/
    ├── cart.js          (cart + public window.BioneticCart API)
    ├── ui.js            (header, menu, modals, FAQ, policies, cookies, Esc)
    └── main.js          (search, contact validation, newsletter, account demo)
```

### Running locally

This is a static page — open `index.html` directly or serve it with any
static server


### Responsiveness

Breakpoints: **1024 px**, **768 px**, **480 px**. Verified across typical
mobile (360 px+), tablet and desktop widths.

### Project status

✅ **Version 1.0.0 — production ready.**

### Repository policy

This public repository contains **only documentation and screenshots** that
prove the work was completed (used for invoicing and tax-reporting purposes
of the contractor's sole-proprietorship).

The complete source code lives in a **private repository** to which the client
receives direct access as part of project delivery. See `DELIVERY.md` for
details.
