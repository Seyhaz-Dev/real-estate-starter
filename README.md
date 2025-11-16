# README

Status: Not started

# **Apple KH Real Estate — Real Estate Website**

A beginner-friendly **HTML + CSS + JavaScript** starter project for building a bilingual real estate website for Cambodian users.

Developers will work in small teams (Front-End Developers + Tech Lead) to design and implement a mobile-friendly property browsing experience.

---

## 📌 Project Overview

This project simulates a real-world real estate search website where users can look for properties to **rent** or **buy**.

The goal is to practice:

- HTML structure and semantic layout
- CSS styling, spacing, and responsive design
- JavaScript for basic interactivity
- Fetching and displaying data from JSON files
- Simple language switching (optional bonus feature)

You will extend the starter files to build pages such as:

- Home
- Property Listings
- Property Details
- Contact Page

---

## 👥 Team Roles

Each team includes two roles:

### **1. Front-End Developers**

- Build layout using HTML and CSS
- Implement responsive design
- Write JavaScript for filtering, interactivity, and data loading
- Communicate progress and collaborate with teammates

### **2. Tech Lead**

- Organize initial folder structure
- Guide developers

---

## 📁 Project Folder Structure

```
project/
├── index.html
├── pages
│   ├── about
│   │   ├── index.css
│   │   └── index.html
│   ├── agents
│   │   ├── index.css
│   │   └── index.html
│   ├── buy
│   │   ├── index.css
│   │   └── index.html
│   ├── contact
│   │   ├── index.css
│   │   └── index.html
│   └── rent
│       ├── index.css
│       └── index.html
├── public
│   ├── assets
│   │   └── images
│   │       ├── agents
│   │       └── properties
│   └── data
│       ├── agents.json
│       ├── langs.json
│       └── properties.json
├── scripts
│   ├── index.js
│   └── scroller.js
└── styles
    ├── components
    │   ├── card.css
    │   ├── card-top.css
    │   ├── general.css
    │   └── nav.css
    ├── main.css
    └── scroller.css
```

---

## 🌐 JSON Data Structure

Properties:

```json
[
  {
    "id": 1,
    "title": {
      "en": "Modern Apartment near AEON Mall",
      "km": "អាផាតមិនទំនើបនៅជិត AEON Mall"
    },
    "type": "apartment",
    "purpose": "rent",
    "price": 350,
    "currency": "USD",
    "location": {
      "city": "Phnom Penh",
      "district": "Chamkarmon",
      "address": "Street 271, Tonle Bassac"
    },
    "bedrooms": 2,
    "bathrooms": 1,
    "area": 65,
    "unit": "m²",
    "images": ["images/apartment1_1.jpg", "images/apartment1_2.jpg"],
    "features": ["Air Conditioning", "Balcony", "Parking"],
    "agency_id": 101,
    "posted_date": "2025-11-10",
    "available": true
  }
]

```

Language file (optional):

```json
{
  "en": {
    "nav": {
      "home": "Home",
      "listings": "Listings",
      "about": "About",
      "contact": "Contact"
    },

    "hero": {
      "title": "Find Your Next Home in Cambodia",
      "subtitle": "Affordable rooms, apartments, and houses for rent and sale.",
      "search": "Search Properties"
    },

    "filters": {
      "purpose": "Purpose",
      "purpose_rent": "Rent",
      "purpose_buy": "Buy",

      "type": "Type",
      "type_any": "Any type",
      "type_room": "Room",
      "type_apartment": "Apartment",
      "type_house": "House",

      "city": "City",
      "price_range": "Price Range"
    },

    "listing": {
      "featured_properties": "Featured Properties",
      "no_results": "No properties found.",
      "load_more": "Load More"
    },

    "property": {
      "details": "Property Details",
      "price": "Price",
      "per_month": "per month",
      "bedrooms": "Bedrooms",
      "bathrooms": "Bathrooms",
      "area": "Area",
      "contact_agency": "Contact Agency",
      "available": "Available",
      "not_available": "Not Available",
      "for_sale": "For Sale"
    },

    "contact": {
      "title": "Contact Us",
      "name": "Your Name",
      "email": "Your Email",
      "message": "Message",
      "send": "Send Message",
      "success": "Message sent successfully!"
    },

    "about": {
      "title": "About KH Realty",
      "mission": "We help Cambodians find affordable and comfortable places to live.",
      "agencies": "Our Partner Agencies"
    },

    "ui": {
      "language": "Language",
      "english": "English",
      "khmer": "Khmer",
      "back": "Back",
      "view_details": "View Details"
    },

    "footer": {
      "copyright": "© 2025 KH Realty. All rights reserved."
    }
  },

  "km": {
    "nav": {
      "home": "ទំព័រដើម",
      "listings": "ប្រភេទអចលនទ្រព្យ",
      "about": "អំពីពួកយើង",
      "contact": "ទំនាក់ទំនង"
    },

    "hero": {
      "title": "ស្វែងរកលំនៅដ្ឋានបន្ទាប់របស់អ្នកនៅកម្ពុជា",
      "subtitle": "បន្ទប់ អាផាតមិន និងផ្ទះ អាចជួល ឬទិញបានក្នុងតម្លៃសមរម្យ។",
      "search": "ស្វែងរកអចលនទ្រព្យ"
    },

    "filters": {
      "purpose": "គោលបំណង",
      "purpose_rent": "ជួល",
      "purpose_buy": "ទិញ",

      "type": "ប្រភេទ",
      "type_any": "គ្រប់ប្រភេទ",
      "type_room": "បន្ទប់",
      "type_apartment": "អាផាតមិន",
      "type_house": "ផ្ទះ",

      "city": "ខេត្ត/ទីក្រុង",
      "price_range": "ជួរតម្លៃ"
    },

    "listing": {
      "featured_properties": "អចលនទ្រព្យពិសេស",
      "no_results": "មិនមានអចលនទ្រព្យទេ។",
      "load_more": "បង្ហាញបន្ថែម"
    },

    "property": {
      "details": "ព័ត៌មានលម្អិតអចលនទ្រព្យ",
      "price": "តម្លៃ",
      "per_month": "ក្នុងមួយខែ",
      "bedrooms": "បន្ទប់គេង",
      "bathrooms": "បន្ទប់ទឹក",
      "area": "ផ្ទៃក្រឡា",
      "contact_agency": "ទាក់ទងក្រុមហ៊ុន",
      "available": "មាន",
      "not_available": "មិនមានទេ",
      "for_sale": "លក់"
    },

    "contact": {
      "title": "ទាក់ទងមកយើង",
      "name": "ឈ្មោះរបស់អ្នក",
      "email": "អ៊ីមែលរបស់អ្នក",
      "message": "សារ",
      "send": "ផ្ញើសារ",
      "success": "សាររបស់អ្នកបានផ្ញើរួចរាល់!"
    },

    "about": {
      "title": "អំពី KH Realty",
      "mission": "យើងជួយប្រជាជនកម្ពុជា ស្វែងរកកន្លែងរស់នៅមានតម្លៃសមរម្យ និងមានផាសុខភាព។",
      "agencies": "ក្រុមហ៊ុនដៃគូរបស់យើង"
    },

    "ui": {
      "language": "ភាសា",
      "english": "ភាសាអង់គ្លេស",
      "khmer": "ភាសាខ្មែរ",
      "back": "ត្រឡប់ក្រោយ",
      "view_details": "មើលព័ត៌មានលម្អិត"
    },

    "footer": {
      "copyright": "© 2025 KH Realty. រក្សាសិទ្ធិគ្រប់យ៉ាង។"
    }
  }
}

```

---

## 🌐 Optional Language Switching (Bonus Feature)

HTML:

```html
<h1 data-i18n="hero.title"></h1>
```

JS example:

```jsx
function setLanguage(lang) {
  document.querySelectorAll("[data-i18n]").forEach(el => {
    const key = el.dataset.i18n.split(".");
    let text = translations[lang];
    key.forEach(k => text = text[k]);
    el.textContent = text;
  });
}
```

Developers who want to go further can store the user’s choice in `localStorage`.

---

## 💡 Features You Will Build

### **Required**

- Clean HTML structure
- Responsive layouts (mobile-first)
- Property listing cards
- Simple filtering (e.g., rent/buy, type)
- Property details using ID query parameters
- Contact page with basic JS form validation

### **Optional Bonus Features (Nice to Have)**

- Language switching (Khmer/English)
- Remember selected language using `localStorage`
- Dark mode toggle

---

## 🧪 How to Run the Project

### Option 1 — Open the HTML files directly

Double-click on `index.html`.

### Option 2 — Recommended: Use Live Server in VS Code

1. Install “Live Server” extension
2. Right-click `index.html`
3. Click **Open with Live Server**

This enables auto-reload and is easier for development.

---

## 🎯 Learning Goals

By finishing this project, you will gain confidence in:

### HTML

- Semantic structure
- Forms
- Accessibility attributes

### CSS

- Flexbox & Grid
- Responsive layout
- Component-based styling
- Hover & animation basics

### JavaScript

- DOM manipulation
- JSON loading with `fetch()`
- Filtering UI
- Language switching (i18n)
- Event listeners

### Teamwork

- Collaboration in small teams
- Role responsibilities
- Presentation & communication skills

---

## 🎤 Final Presentation

Your team will present:

- What you built
- A short demo of your website
- What roles you took
- What challenges you solved
- What you learned about HTML, CSS, and JS