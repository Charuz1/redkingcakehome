Project Introduction: Redking Cake Nikaweratiya

1. Project Overview

Redking Cake Nikaweratiya is a modern, mobile-first, single-page custom cake ordering and showcase web application built for a premier local celebration bakery in Nikaweratiya, Sri Lanka.

The primary objective of this website is to convert visitors from Facebook and Instagram into confirmed cake orders by allowing customers to browse categorized cake designs, upload custom reference photos, choose pickup or delivery options, view bank transfer details for advance payments, and send a complete, pre-formatted order message directly to the bakery's WhatsApp (+94 76 280 0955).

2. Business Profile & Contact Details

Use these exact business details across all pages, footers, modals, and WhatsApp message templates:

Business Name: Redking Cake Nikaweratiya

Address: Samadarapitiya, Maho Road, Nikaweratiya 60470, Sri Lanka

Primary WhatsApp / Order Number: +94 76 280 0955 (WhatsApp API format: 94762800955)

Secondary Hotline: +94 77 225 2645

Operating Hours: Open 24 Hours, Monday – Sunday (Customers are advised to contact ahead for custom designs or same-day orders)

Social Media:

Facebook: Red King Cake Nikaweratiya

Instagram: @chathura_rasnayaka_redking

3. Product Offerings & Pricing Structure

The bakery specializes in bespoke celebration cakes and gift bundles:

Cake Categories:

Birthday Cakes (Buttercream, Ribbon, Fondant & Custom Theme Cakes)

Wedding & Anniversary (Multi-tier Wedding Cakes & Anniversary Specials)

Chocolate & Drip (Belgian Ganache Drip, Truffle & Hazelnut Cakes)

Gateau & Cupcakes (Black Forest Gateau, Red Velvet & Swirl Cupcake Boxes)

Combo & Gift Packs (Pot Cakes, Custom Mug Printing, Plush Teddy Bears & Gift Hampers)

Pricing Tiers & Promotional Packages:

Promotional Combo / Cake Packages: LKR 5,000 and LKR 7,000

Custom & Luxury Celebration Cakes: LKR 10,000+

Standard Weight Options: 500g, 1kg, 1.5kg, 2kg+

4. Visual Identity & "Antigravity" Design System

The UI follows a Modern Luxury Bakery aesthetic enhanced with subtle Antigravity levitation effects:

Color Palette:

Primary Background (Warm Ivory): #FFFBF7

Secondary Surface (Soft Cream): #FDF4EC

Brand Accent (Royal Crimson): #B91C1C (Hover/Dark: #991B1B)

Luxury Highlight (Champagne Gold): #D97706

Primary Text (Deep Espresso): #1F1614

WhatsApp Action Green: #059669 (Emerald-600)

Typography:

Display / Headings: Playfair Display (Google Fonts)

Body / UI / Forms: Plus Jakarta Sans (Google Fonts)

Antigravity UI Effects:

Smooth CSS @keyframes floating animations (translateY + subtle rotation) applied to the hero cake card, promo badges, and ambient background orbs.

Frosted glassmorphism (backdrop-filter: blur(14px)) on the sticky navigation bar, floating badges, and order cards.

Smooth card elevation (translateY(-8px)) on gallery hover interactions.

5. Technical Architecture & File Structure

The project is intentionally built with zero backend dependencies so it loads ultra-fast on mobile connections and can be hosted for free on GitHub Pages, Netlify, Vercel, or Cloudflare Pages.

redking-cake-nikaweratiya/
├── index.html          # Complete single-page application (HTML5, Tailwind CSS CDN, Custom CSS, Vanilla JS)
└── introduction.md     # Project specification & Antigravity agent guide


Frontend Stack: Semantic HTML5, Tailwind CSS (via CDN), Custom CSS3 Animations, and Vanilla JavaScript (ES6+).

Mobile-First Responsiveness: Optimized for 375px mobile viewports up to 1440px desktop displays, with touch-friendly inputs (>= 44px tap targets) and sticky live order summaries on desktop.

6. Core Functional Requirements

When modifying or extending this codebase, ensure all of the following features remain intact and functional:

Sticky Glassmorphic Header:

Displays the Redking Cake brand logo, quick section navigation links, mobile hamburger menu, and a direct "WhatsApp Us" button.

Hero Section:

Features a levitating hero cake showcase, floating promo badges, quick-select package pills (LKR 5,000, LKR 7,000, LKR 10,000+), and dual CTAs (Order Custom Cake & Explore Menu).

Interactive Categorized Cake Gallery:

Dynamic category filter tabs (All, Birthday Cakes, Wedding & Anniversary, Chocolate & Drip, Gateau & Cupcakes, Combo & Gift Packs).

Clicking "Order This Cake" automatically populates the Cake Category and Package in the order form below and smoothly scrolls to #order-form.

Custom Cake Order Form & Live Summary:

Customer Details: Customer Name, Phone Number, WhatsApp Number (with a "Same as Phone" auto-sync checkbox).

Cake Customization: Cake Category (Vargaya), Size/Package, and Name/Wording on Cake.

Schedule: Required Date (restricted to today or future dates) and Required Time.

Fulfillment: Radio toggle between Store Pickup (Maho Road, Nikaweratiya) and Home Delivery (dynamically reveals a required Delivery Location input field).

Custom Design Reference Upload: Drag-and-drop or file picker supporting JPG, PNG, and WEBP with an instant thumbnail preview, file size readout, and remove button.

Advance Payment Option: Radio toggle between "Confirm Price via WhatsApp First" and "Pay Advance via Bank Transfer" (reveals an expandable bank account card with a one-click Copy Account No. button and optional transfer reference field).

Real-Time Order Summary: Updates live as the user types or selects options.

WhatsApp Integration & Confirmation Modal:

Validates all required fields before submission.

Formats all order inputs into a clean, emoji-structured WhatsApp message and opens https://wa.me/94762800955?text=... in a new tab.

Displays a backup Confirmation Modal with a Copy Message button and a reminder to attach the uploaded reference photo or bank receipt in WhatsApp.

Location & Social Footer:

Displays the full Nikaweratiya address, clickable phone/WhatsApp links, 24/7 operating hours, social media buttons, and an embedded Google Map centered on Nikaweratiya (60470).

7. Instructions for Google Antigravity Agents

If you are an AI agent operating inside Google Antigravity IDE, follow these guidelines when executing user tasks:

Adding or Updating Cakes: Edit the cakeCatalog array inside the <script> section of index.html. Ensure every item includes id, title, category, formCategory, price, description, and a reliable image URL with an onerror fallback.

Updating Bank Account Details: Locate #bank-transfer-box in index.html to update the Bank Name, Account Holder Name, or #bank-account-number.

Preserving Single-File Portability: Unless the user explicitly requests a multi-file framework migration (e.g., React/Next.js), keep all styles and JavaScript self-contained within index.html so the site works immediately when opened in any browser.

Testing Checklist: After making edits, verify mobile layout (375px), category tab filtering, conditional delivery address validation, image upload preview, and WhatsApp URL encoding.