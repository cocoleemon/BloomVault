# 🌸 Information Architecture

> *"Good architecture helps users find what they need. Great architecture helps users discover what they didn't know they were looking for."*

---

# Introduction

BloomVault is designed around a simple principle:

Everything begins with a product.

Rather than treating every feature as an isolated destination, BloomVault connects products, ingredients, brands, collections, routines, and personal organization into one seamless experience.

Users should never feel lost while exploring.

Every screen should naturally lead to another meaningful destination.

---

# Architecture Principles

The information architecture of BloomVault follows these principles:

- Product-centered navigation
- Simple and predictable structure
- Connected experiences
- Progressive discovery
- Minimal navigation depth
- Personal organization first

Every screen should help users continue exploring rather than forcing them to start over.

---

# High-Level Architecture

```text
Authentication
│
├── Sign In
├── Sign Up
└── Forgot Password

↓

Home

├── Library
├── Discover
├── Search
└── Me
```

---

# Primary Navigation

BloomVault Version 1 contains four primary destinations.

```text
Home

├── 📚 Library
├── 🔍 Discover
├── 🔎 Search
└── 👤 Me
```

These destinations provide access to every core feature within the application.

---

# Library

The Library is the user's personal beauty space.

```text
Library

├── All Products
├── Collections
├── Wishlist
├── Routines
└── Product Details
```

The Library contains only products that belong to the user.

---

# Discover

Discover encourages exploration beyond the user's own library.

```text
Discover

├── Featured Products
├── Trending Products
├── New Products
├── Browse Categories
└── Product Details
```

Discover introduces users to products they may wish to research.

---

# Search

Search provides direct access to BloomVault's product catalog.

```text
Search

├── Product Results
├── Recent Searches
├── Suggested Searches
└── Product Details
```

Search is optimized for quickly finding products rather than browsing.

---

# Product Details

Every product page becomes the central hub of the BloomVault experience.

```text
Product Details

├── Product Information
├── Ingredients
├── Brand
├── Compare
├── Collections
├── Wishlist
├── Notes
└── Routines
```

Almost every feature within BloomVault connects through Product Details.

---

# Ingredient Explorer

Ingredient Explorer is accessed from Product Details.

```text
Ingredient

├── Description
├── Benefits
├── Skin Concerns
├── Related Ingredients
├── Products Containing Ingredient
└── Products in Your Library
```

Ingredients become another pathway for product discovery and learning.

---

# Brand

Brands provide another way to browse products.

```text
Brand

├── Product Catalog
├── Categories
├── Products in Your Library
└── Products in Wishlist
```

Brand pages focus on product exploration rather than company information.

---

# Collections

Collections organize products into meaningful groups.

```text
Collections

├── Collection List
├── Collection Details
├── Add Products
└── Edit Collection
```

Collections are completely user-defined.

---

# Wishlist

Wishlist stores products users are interested in purchasing or researching later.

```text
Wishlist

├── Wishlist Items
├── Product Details
└── Move to Collection
```

Wishlist remains separate from the user's owned products.

---

# Product Comparison

Comparison allows users to evaluate products side by side.

```text
Comparison

├── Product A
├── Product B
├── Ingredients
├── Benefits
├── Notes
└── Differences
```

Comparison supports informed decision-making before purchase.

---

# Routines

Routines help users organize products into skincare routines.

```text
Routines

├── Morning
├── Evening
├── Custom Routine
└── Routine Details
```

BloomVault provides routine planning rather than habit tracking.

---

# Profile

Profile contains user preferences and account settings.

```text
Profile

├── Personal Information
├── Preferences
├── Account Settings
└── Help
```

---

# Connected Architecture

BloomVault is designed as a connected knowledge system.

```text
                📦 Product
                     │
      ┌──────────────┼──────────────┐
      │              │              │
🌿 Ingredient     🏷️ Brand      ⚖️ Compare
      │              │              │
      └──────────────┼──────────────┘
                     │
               📚 Library
                     │
      ┌──────────────┼──────────────┐
      │              │              │
🗂️ Collections   💖 Wishlist   ✨ Routines
```

This architecture allows users to move naturally between related information without becoming lost.

---

# Navigation Philosophy

BloomVault minimizes unnecessary navigation.

Users should rarely need more than two or three taps to reach related information.

Every Product Details page acts as a gateway to deeper exploration.

---

# Future Expansion

The architecture intentionally supports future features such as:

- AI Beauty Assistant
- Barcode Scanner
- Price Tracking
- Smart Recommendations
- Product Timeline

These additions can connect directly to the existing product-centered architecture without requiring major structural changes.

---

# Information Architecture Summary

BloomVault organizes beauty research around products rather than isolated features.

Products connect users to ingredients, brands, collections, comparisons, routines, and personal knowledge, creating a seamless research experience that grows more valuable over time.

Every screen exists to support curiosity, learning, and organization.

---

> **BloomVault**

> *Your Personal Beauty Library.*