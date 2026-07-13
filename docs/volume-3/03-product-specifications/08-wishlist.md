# Wishlist

**Feature ID:** BV-008
**Volume:** III — Product Specifications
**File:** 08-wishlist.md
**Status:** Draft
**Version:** 0.2.0
**Last Updated:** July 13, 2026
**Owner:** Coleen Ligasan

---

# 🌸 Overview

The Wishlist allows users to keep track of products they hope to purchase in the future.

Unlike the Library, which serves as a personal beauty knowledge library, the Wishlist represents purchase intent. It helps users organize products they are considering while continuing to research and compare them before making a decision.

Every Wishlist item may also include an optional **Purchase Intent**, allowing users to remember *why* they saved a product in the first place.

The Wishlist should feel intentional rather than transactional, supporting thoughtful purchasing habits instead of impulse buying.

---

# Purpose

Provide users with a dedicated space to manage products they are interested in purchasing.

The Wishlist should help users:

* Keep track of products they want to buy.
* Separate purchase intent from general research.
* Continue researching before purchasing.
* Capture the reason behind each future purchase.
* Make thoughtful buying decisions.

---

# Problem It Solves

Users often discover products they want to buy in the future but have no organized way to track them.

As a result, they may:

* Forget products they were interested in.
* Lose track of why they wanted a product.
* Repurchase products impulsively.
* Forget to wait for sales or restocks.
* Struggle to prioritize future purchases.

The Wishlist provides a structured way to manage future purchases while keeping products connected to the user's Beauty Library.

---

# Goals

The Wishlist should:

* Support intentional purchasing.
* Reduce forgotten products.
* Preserve the user's purchase intentions.
* Encourage continued research before buying.
* Integrate naturally with the Library.

Wishlist items should always feel like part of a larger beauty journey.

---

# User Stories

### Save for Later

**As a user, I want to save products I'm interested in so I can revisit them later.**

---

### Wait Before Buying

**As a user, I want to keep products on my Wishlist while I continue researching them before making a purchase.**

---

### Stay Organized

**As a user, I want to separate products I want to buy from products I'm simply researching.**

---

### Track Priorities

**As a user, I want to organize my Wishlist so I know which products I'm most excited to purchase next.**

---

### Remember My Intention

**As a user, I want to record why I'm waiting to purchase a product so I can remember my reasoning when I revisit it later.**

---

# Functional Requirements

The Wishlist shall allow users to:

* Add products to the Wishlist.
* Remove products from the Wishlist.
* View all Wishlist items.
* Search within the Wishlist.
* Sort Wishlist items.
* Open Product Details from the Wishlist.
* Assign an optional Purchase Intent.
* Edit a Purchase Intent.
* Remove a Purchase Intent.

Wishlisted products should always remain part of the user's Library.

---

# Business Rules

* Wishlist items belong to a single user.
* Products can exist in both the Library and the Wishlist.
* Removing a product from the Wishlist does not remove it from the Library.
* Products may only appear once in the Wishlist.
* Purchase Intent is optional.
* Each Wishlist item may have one Purchase Intent.
* Users may edit or remove the Purchase Intent at any time.

---

# Purchase Intent

Purchase Intent captures the user's reason for saving a product.

This transforms the Wishlist from a simple shopping list into a decision-making tool that supports thoughtful purchasing habits.

Suggested Purchase Intent values include:

* 💸 Waiting for Sale
* ⏳ Waiting for Payday
* 🔬 Still Researching
* 🧴 Finish Current Product
* 🎁 Gift Idea
* ✈️ Buy Abroad
* 🌈 Need Shade Match
* 📦 Waiting for Restock
* ✏️ Custom

Future versions may allow users to create fully customizable Purchase Intents.

---

# User Flow

Library or Product Details

↓

Add to Wishlist

↓

(Optional) Select Purchase Intent

↓

Wishlist

↓

Browse Wishlist

↓

Open Product Details

↓

Purchase or Remove from Wishlist

---

# Screen Relationships

Wishlist connects with:

* Library
* Product Details
* Compare
* Collections
* Discover

Wishlist extends the user's Beauty Library by representing future purchase intentions.

---

# UI Components

The Wishlist may include:

* Wishlist grid or list
* Search bar
* Sort options
* Product cards
* Purchase Intent badge
* Remove from Wishlist action
* Empty State

The layout should remain clean, organized, and easy to scan.

---

# User Interface Behavior

The Wishlist should:

* Update immediately after adding or removing products.
* Preserve sorting preferences.
* Display Purchase Intent badges when available.
* Allow quick access to Product Details.
* Make managing future purchases effortless.

---

# States

Supported states include:

* Empty
* Loading
* Populated
* Searching
* Offline
* Error

Transitions should remain smooth and predictable.

---

# Empty States

When no products have been added, BloomVault should encourage thoughtful exploration.

Example:

*"Products you're considering will appear here. Add items to your Wishlist while you continue researching them."*

---

# Error Handling

Examples include:

* Failed Wishlist update.
* Failed Purchase Intent update.
* Network interruption.
* Duplicate additions.
* Synchronization issues.

Users should always understand what happened and how to recover.

---

# Edge Cases

The Wishlist should gracefully support:

* Large Wishlists.
* Offline changes.
* Deleted products.
* Duplicate save attempts.
* Missing Purchase Intent.
* Slow network conditions.

---

# Accessibility

The Wishlist should support:

* Screen readers.
* Dynamic text sizes.
* Accessible buttons.
* Logical navigation order.
* Comfortable touch targets.

---

# Analytics Events

Potential analytics events include:

* Product Wishlisted
* Product Removed from Wishlist
* Wishlist Opened
* Wishlist Searched
* Wishlist Sorted
* Purchase Intent Selected
* Purchase Intent Updated
* Purchase Intent Removed

Analytics should support product improvements while respecting user privacy.

---

# Database Impact

The Wishlist stores user-specific purchase intentions while referencing products already saved in the user's Library.

Each Wishlist item may optionally store a Purchase Intent that captures the user's current buying intention.

Detailed schema definitions are documented within the Technical Architecture volume.

---

# API Requirements

Wishlist requires functionality for:

* Add to Wishlist
* Remove from Wishlist
* Retrieve Wishlist
* Search Wishlist
* Sort Wishlist
* Assign Purchase Intent
* Update Purchase Intent
* Remove Purchase Intent

Implementation details are documented separately.

---

# Security & Permissions

Users may only access and manage their own Wishlist.

All Wishlist data should be protected through authentication and Row Level Security (RLS).

---

# Performance Considerations

The Wishlist should:

* Load quickly.
* Synchronize efficiently.
* Cache recent updates.
* Scale alongside growing libraries.

Purchase Intent updates should feel immediate and responsive.

---

# Acceptance Criteria

The feature is complete when users can:

* Add products to the Wishlist.
* Remove products from the Wishlist.
* Assign, edit, and remove Purchase Intent.
* Search and sort Wishlist items.
* Open Product Details from the Wishlist.
* Maintain Wishlist data across devices.

---

# Future Enhancements

Potential future improvements include:

* Multiple Purchase Intents.
* AI-suggested Purchase Intent.
* Price tracking.
* Sale notifications.
* Restock notifications.
* Purchase reminders.
* Budget planning.
* Custom icons for Purchase Intent.
* Automatic grouping by Purchase Intent.

---

# Product Decisions

The Wishlist represents purchase intention rather than product discovery.

Every wishlisted product should already exist within the user's Beauty Library, reinforcing BloomVault's philosophy that meaningful beauty decisions begin with research.

Purchase Intent is intentionally lightweight but meaningful. By allowing users to record *why* they are waiting before purchasing, BloomVault supports mindful buying habits and preserves the context behind every Wishlist item.

The Wishlist is designed to encourage thoughtful purchasing—not impulse buying.

---

> **BloomVault**

> *Your Personal Beauty Library.*
