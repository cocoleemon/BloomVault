# Wishlist

**Feature ID:** BV-008
**Volume:** III — Product Specifications
**File:** 08-wishlist.md
**Status:** Draft
**Version:** 0.1.0
**Last Updated:** July 13, 2026
**Owner:** Coleen Ligasan

---

# 🌸 Overview

The Wishlist allows users to keep track of products they hope to purchase in the future.

Unlike the Library, which serves as a personal beauty knowledge library, the Wishlist represents purchase intent. It helps users organize products they are considering while continuing to research and compare them before making a decision.

The Wishlist should feel intentional rather than transactional, supporting thoughtful purchasing habits instead of impulse buying.

---

# Purpose

Provide users with a dedicated space to manage products they are interested in purchasing.

The Wishlist should help users:

* Keep track of products they want to buy.
* Separate purchase intent from general research.
* Revisit products before purchasing.
* Make thoughtful buying decisions.

---

# Problem It Solves

Users often discover products they want to buy in the future but have no organized way to track them.

As a result, they may:

* Forget products they were interested in.
* Repurchase products impulsively.
* Lose track of products while waiting for sales.
* Struggle to prioritize future purchases.

The Wishlist provides a structured way to manage future purchases while keeping products connected to the user's Beauty Library.

---

# Goals

The Wishlist should:

* Support intentional purchasing.
* Reduce forgotten products.
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

# Functional Requirements

The Wishlist shall allow users to:

* Add products to the Wishlist.
* Remove products from the Wishlist.
* View all wishlisted products.
* Search within the Wishlist.
* Sort Wishlist items.
* Open Product Details from the Wishlist.

Wishlisted products should remain part of the user's Library.

---

# Business Rules

* Wishlist items belong to a single user.
* Products can exist in both the Library and the Wishlist.
* Removing a product from the Wishlist does not remove it from the Library.
* Products may only appear once in the Wishlist.

---

# User Flow

Library or Product Details

↓

Add to Wishlist

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
* Remove from Wishlist action
* Empty State

The layout should remain clean and focused.

---

# User Interface Behavior

The Wishlist should:

* Update immediately after adding or removing products.
* Preserve sorting preferences.
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

Analytics should support product improvements while respecting user privacy.

---

# Database Impact

The Wishlist stores user-specific purchase intent and references products already saved in the user's Library.

Detailed relationships are defined within the Technical Architecture documentation.

---

# API Requirements

Wishlist requires functionality for:

* Add to Wishlist
* Remove from Wishlist
* Retrieve Wishlist
* Search Wishlist
* Sort Wishlist

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

---

# Acceptance Criteria

The feature is complete when users can:

* Add products to the Wishlist.
* Remove products from the Wishlist.
* Search and sort Wishlist items.
* Open Product Details from the Wishlist.
* Maintain Wishlist data across devices.

---

# Future Enhancements

Potential future improvements include:

* Wishlist priorities.
* Purchase status tracking.
* Price tracking.
* Sale notifications.
* Restock notifications.
* Purchase reminders.
* Wishlist reasons (e.g., Waiting for Sale, Still Researching).
* Budget planning.

---

# Product Decisions

The Wishlist represents purchase intention rather than product discovery.

Every wishlisted product should already exist within the user's Beauty Library, reinforcing BloomVault's philosophy that meaningful beauty decisions begin with research.

The Wishlist is designed to support intentional purchasing habits by helping users revisit products, continue learning, and buy with confidence when the time is right.

---

> **BloomVault**

> *Your Personal Beauty Library.*
