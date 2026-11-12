# Capital-Vista

[![Website Status](https://img.shields.io/badge/Status-Active-brightgreen.svg)](#)
[![Framework](https://img.shields.io/badge/Framework-Bootstrap%205-7952b3.svg)](https://getbootstrap.com/)
[![License](https://img.shields.io/badge/License-Proprietary-blue.svg)](#)

> **Capital-Vista** is a modern, responsive real estate web platform designed for property buyers, tenants, estate agents, and real estate developers across Nigeria. The platform showcases premium residential homes, luxury apartments, commercial spaces, and short-let properties with streamlined property listings and multi-channel customer inquiry support.

---

## Table of Contents

- [Overview](#overview)
- [Key Features](#key-features)
- [Website Pages & Architecture](#website-pages--architecture)
- [Contact Details & Alternative Channels](#contact-details--alternative-channels)
- [Technology Stack](#technology-stack)
- [Getting Started / Running Locally](#getting-started--running-locally)
- [Project Directory Structure](#project-directory-structure)
- [Browser Compatibility](#browser-compatibility)
- [License & Copyright](#license--copyright)

---

## Overview

**Capital-Vista** connects property seekers with verified landlords, accredited real estate agents, and commercial property developers across major metropolitan areas in Nigeria (including Lagos, Abuja, Port Harcourt, and Ibadan).

Whether users are looking to buy a dream home, rent modern apartments, lease office spaces, or list their own properties for sale or rent, Capital-Vista provides an intuitive and responsive experience across all screen sizes.

---

## Key Features

- **Intuitive Property Discovery**:
  - Hero search filter bar allowing visitors to quickly filter by intent (*Buy*, *Sell*, *Rent*), location, property type, and price range.
  - Featured property highlights with pricing, bedroom/bathroom counts, location tags, and direct listing agent details.

- **Comprehensive Properties Catalog (`properties.html`)**:
  - Filterable tabs for *For Sale*, *For Rent*, *Commercial*, and *Auctions*.
  - Sort properties by relevance, price, or date.
  - Multi-page pagination support for easy browsing through large catalogs.

- **Property Submission Portal (`listing.html`)**:
  - Form for individuals, agents, and property developers to publish listings.
  - Includes property categorization, pricing in Naira (₦), amenities, description, and photos.
  - **Multi-channel contact capture**: Collects both **Primary Contact Details** and **Alternative Contact / WhatsApp Numbers** to ensure interested buyers can always connect with the seller.

- **Dedicated Contact & Support Center (`contact.html`)**:
  - Prominent contact cards displaying **Headquarters (Lagos)** and **Alternative Regional Branch (Abuja)**.
  - Dual phone lines (**Primary Hotline** and **Alternative Contact / WhatsApp**).
  - Dual email channels (**Primary Inquiries** and **Alternative / Support Desk**).
  - Responsive inquiry form allowing visitors to provide their primary and alternative contact information.

- **User Authentication (`login.html` & `register.html`)**:
  - Clean authentication pages for account creation and sign-in.
  - Social login options integrated into UI (Google, Facebook, Apple).

- **Fully Responsive Mobile Experience**:
  - Built using Bootstrap 5 fluid grid system and flexible utility classes.
  - Collapsible navigation bar with mobile-friendly action buttons.

---

## Website Pages & Architecture

| Page | File | Description |
| :--- | :--- | :--- |
| **Home** | [`index.html`](index.html) | Landing page with hero banner, property search, featured listings, client feedback, latest real estate insights, and quick inquiry box. |
| **Properties** | [`properties.html`](properties.html) | Extensive property directory with category filters (Rent, Buy, Short-let, Auction) and pagination. |
| **Listing** | [`listing.html`](listing.html) | Listing publication form for sellers, agents, and developers with primary and alternative contact fields. |
| **Contact Us** | [`contact.html`](contact.html) | Corporate contact hub featuring primary headquarters, alternative Abuja branch, primary & alternative phone lines, email desks, and message form. |
| **Login** | [`login.html`](login.html) | Account login page with email authentication and social sign-in UI. |
| **Register** | [`register.html`](register.html) | Account registration page with user credentials and terms consent. |

---

## Contact Details & Alternative Channels

Capital-Vista provides both primary and alternative contact channels for uninterrupted customer service and property inquiries:

### 🏢 Office Locations
- **Headquarters (Primary):**
  Capital-Vista Tower, Plot 14, Victoria Island, Lagos, Nigeria
- **Regional Branch (Alternative):**
  Capital-Vista Plaza, Central Business District (CBD), Abuja, Nigeria

### 📞 Phone & Instant Messaging
- **Primary Hotline:** [+234 (0) 801 234 5678](tel:+2348012345678)
- **Alternative Contact / WhatsApp:** [+234 (0) 809 876 5432](tel:+2348098765432)
- **Customer Care Toll-Free:** `+234 (0) 700-CAPITAL-VISTA`

### ✉️ Email Support
- **Primary Inquiries:** [info@capital-vista.com](mailto:info@capital-vista.com)
- **Alternative / Technical Support:** [support@capital-vista.com](mailto:support@capital-vista.com)
- **Sales & Listings Desk:** [sales@capital-vista.com](mailto:sales@capital-vista.com)

### ⏰ Business Operating Hours
- **Monday – Friday:** 8:00 AM – 6:00 PM (WAT)
- **Saturday:** 9:00 AM – 2:00 PM (WAT)
- **Sunday & Public Holidays:** Closed (Online inquiries monitored 24/7)

---

## Technology Stack

- **Markup & Semantics:** HTML5
- **Styling & Components:** [Bootstrap 5.0.2](https://getbootstrap.com/) via CDN
- **Icons:** [Bootstrap Icons v1.9.1](https://icons.getbootstrap.com/) & SVG icons
- **JavaScript Dependencies:** [Popper.js v2.9.2](https://popper.js.org/) & Bootstrap 5 Bundle
- **Fonts & Typography:** System font stack (`Segoe UI`, `Roboto`, `Helvetica Neue`, sans-serif)

---

## Getting Started / Running Locally

Since Capital-Vista is a static frontend website, no complex server builds or package installations are required.

### Option 1: Direct Browser Launch
Double-click [`index.html`](index.html) or right-click and choose **Open with** > **Google Chrome** (or your preferred browser).

### Option 2: VS Code Live Server
1. Open the project folder in **Visual Studio Code**.
2. Install the **Live Server** extension (by Ritwick Dey).
3. Right-click on [`index.html`](index.html) and select **Open with Live Server**.
4. The site will launch automatically at `http://localhost:5500`.

### Option 3: Python Local HTTP Server
Run the following command in PowerShell / Terminal inside the project root:
```bash
python -m http.server 8080
```
Then navigate to:
```
http://localhost:8080
```

---

## Project Directory Structure

```text
capital-vista/
├── .vscode/
│   └── launch.json                # VS Code Chrome debugging configuration
├── resources/                     # Image assets, banners, property photos & icons
│   ├── batch-02.ico               # Favicon
│   ├── batch-08.png               # Brand logo (Contact page & footer)
│   ├── batch-011.png              # Brand logo (Homepage & auth pages)
│   ├── batch-07.png               # Brand logo (Listing page)
│   ├── batch-06.png               # Brand logo (Properties page)
│   └── *.jpg                      # High-resolution property photography
├── contact.html                   # Contact page with primary & alternative details
├── index.html                     # Main homepage
├── listing.html                   # Property submission page
├── login.html                     # Member sign-in page
├── properties.html                # Property listings catalog & filters
├── register.html                  # User registration page
└── README.md                      # Project documentation and specifications
```

---

## Browser Compatibility

Capital-Vista has been tested and styled for modern desktop and mobile browsers:
- Google Chrome (latest)
- Mozilla Firefox (latest)
- Microsoft Edge (latest)
- Apple Safari (latest)
- Mobile Browsers (Chrome for Android, Safari iOS)

---

## License & Copyright

&copy; 2026 **Capital-Vista**. All Rights Reserved.  
All brand assets, photography, and site templates are the property of Capital-Vista.
