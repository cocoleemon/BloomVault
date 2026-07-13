# 🌸 Screen Inventory

> *"Every screen should have a clear purpose. If a screen exists without adding meaningful value, it shouldn't exist."*

---

# Introduction

The Screen Inventory provides a complete overview of every screen included in BloomVault Version 1.

Each screen exists to support the application's core philosophy of helping users research, organize, understand, and confidently navigate beauty products.

Rather than maximizing the number of screens, BloomVault focuses on creating a cohesive and connected experience.

---

# Authentication

### Sign In

Purpose:

Allow existing users to securely access their BloomVault account.

---

### Sign Up

Purpose:

Allow new users to create a BloomVault account.

---

### Forgot Password

Purpose:

Help users recover access to their account.

---

# Main Navigation

BloomVault Version 1 includes four primary destinations.

| Screen | Purpose |
|---------|---------|
| 📚 Library | Personal beauty library and organization |
| 🔍 Discover | Explore and discover products |
| 🔎 Search | Search the product catalog |
| 👤 Me | Account, preferences, and settings |

---

# Library

### Library Home

Purpose:

Display all products saved by the user.

---

### Collections

Purpose:

Organize products into custom collections.

---

### Collection Details

Purpose:

View and manage products within a collection.

---

### Wishlist

Purpose:

View products saved for future consideration.

---

### Routines

Purpose:

View all skincare routines.

---

### Routine Details

Purpose:

Create, edit, and manage routines.

---

# Product Experience

### Product Details

Purpose:

Serve as the central hub for researching a product.

Users can:

- View product information
- Explore ingredients
- Browse the brand
- Compare products
- Add to collections
- Add to Wishlist
- Add to routines
- Write personal notes

---

### Product Comparison

Purpose:

Compare products side by side before making a decision.

---

### Ingredient Explorer

Purpose:

Help users understand ingredients and discover related products.

---

### Brand

Purpose:

Browse all products from a specific brand.

---

# Discover

### Discover Home

Purpose:

Introduce users to products outside their personal Library.

Possible sections include:

- Featured Products
- Trending Products
- New Products
- Browse by Category

---

# Search

### Search

Purpose:

Search for products within BloomVault.

Includes:

- Search bar
- Search results
- Recent searches
- Suggested searches

---

# Me

### Me

Purpose:

Provide access to personal account information, preferences, and settings.

Possible sections include:

- Account
- Preferences
- Settings
- Help & Support
- About BloomVault

---

# Supporting Screens

### Empty States

Purpose:

Guide users when no content is available.

Examples:

- Empty Library
- Empty Wishlist
- Empty Collections
- Empty Routines

---

### Error States

Purpose:

Clearly communicate unexpected issues while helping users recover.

---

### Loading States

Purpose:

Provide visual feedback while data is loading.

---

# Future Screens

The following screens are intentionally excluded from Version 1 but may be introduced in future releases:

- AI Beauty Assistant
- Barcode Scanner
- Price Tracking
- Product Timeline
- Smart Recommendations
- Notifications
- Beauty Journal

These ideas are documented separately within Future UX Ideas.

---

# Screen Relationships

Most screens connect through Product Details.

```text
Library
      │
Discover
      │
Search
      │
      ▼
Product Details
      │
 ┌────┼─────────────┐
 │    │             │
 ▼    ▼             ▼
Ingredient      Brand      Compare
      │
      ▼
Library Actions
      │
 ┌────┼─────────────┐
 │    │             │
 ▼    ▼             ▼
Collections Wishlist Routines
```

This architecture allows users to move naturally between learning and organization without unnecessary navigation.

---

# Screen Inventory Summary

BloomVault Version 1 intentionally includes a focused set of screens that support research, organization, learning, and confident decision-making.

Every screen has a clearly defined purpose and contributes to the overall experience of building a personal beauty library.

---

> **BloomVault**

> *Your Personal Beauty Library.*