# Routines

**Feature ID:** BV-010
**Volume:** III — Product Specifications
**File:** 10-routines.md
**Status:** Draft
**Version:** 0.1.0
**Last Updated:** July 13, 2026
**Owner:** Coleen Ligasan

---

# 🌸 Overview

Routines allow users to organize products into structured beauty routines that reflect how they use products in real life.

Rather than functioning as a habit tracker, BloomVault's Routine feature focuses on planning, organization, and understanding. Users can build routines using products from their Library and arrange them in the order they intend to use them.

Routines help transform a collection of products into a practical beauty system.

---

# Purpose

Provide users with a way to organize saved products into meaningful routines.

Routines should help users:

* Visualize how products work together.
* Plan morning and evening routines.
* Create routines for specific goals or occasions.
* Document personal usage notes.
* Build confidence in their beauty decisions.

---

# Problem It Solves

As users save more products, it becomes difficult to remember:

* Which products belong together.
* The order products should be applied.
* Which routine a product is part of.
* Why certain products were selected.

Without a routine feature, products remain individual pieces of information rather than part of a complete beauty workflow.

Routines provide structure and context.

---

# Goals

Routines should:

* Feel simple and flexible.
* Support personal beauty workflows.
* Encourage thoughtful product organization.
* Reinforce learning and understanding.
* Integrate naturally with the Library.

BloomVault should help users design routines, not pressure them to complete routines.

---

# User Stories

### Create a Routine

**As a user, I want to create a routine so I can organize products in the order I use them.**

---

### Plan My Skincare

**As a user, I want to see how products fit together so I can build a complete routine.**

---

### Create Specialized Routines

**As a user, I want to create routines for specific goals, events, or skin concerns.**

---

### Add Personal Notes

**As a user, I want to attach notes to routine steps so I can remember important instructions.**

---

# Functional Requirements

The Routines feature shall allow users to:

* Create a routine.
* Edit a routine.
* Delete a routine.
* Add products from the Library.
* Remove products from a routine.
* Reorder products.
* Rename routines.
* Add optional notes to each step.
* View routine details.

---

# Business Rules

* Every routine belongs to a single user.
* Products must exist in the user's Library before being added to a routine.
* Products may belong to multiple routines.
* Routine notes are optional.
* Deleting a routine does not remove products from the Library.

---

# Routine Types

Users may create any routine they wish.

Examples include:

* 🌞 Morning Routine
* 🌙 Night Routine
* ✈️ Travel Routine
* 💒 Wedding Prep
* 🩷 Rosacea Recovery
* ☀️ Summer Routine
* ❄️ Winter Routine

BloomVault does not restrict routine categories.

---

# Routine Structure

A routine consists of:

* Routine name
* Optional description
* Ordered list of products
* Optional step notes
* Creation date
* Last updated date

---

# User Flow

Library

↓

Create Routine

↓

Select Products

↓

Arrange Order

↓

Add Optional Notes

↓

Save Routine

↓

View Routine

---

# Screen Relationships

Routines connect with:

* Library
* Product Details
* Collections
* Wishlist
* Compare

Routines represent one of the primary ways users organize products within their Library.

---

# UI Components

The Routine experience may include:

* Routine cards
* Routine details screen
* Product step list
* Drag-and-drop ordering
* Step notes
* Create Routine button
* Edit Routine action
* Empty State

The experience should feel calm and organized.

---

# User Interface Behavior

Routines should:

* Update immediately after edits.
* Preserve product order.
* Support intuitive reordering.
* Display notes clearly.
* Allow quick access to Product Details.

---

# States

Supported states include:

* Empty
* Loading
* Populated
* Editing
* Error
* Offline

---

# Empty States

When no routines exist:

*"Create your first routine to organize products into a personalized beauty workflow."*

---

# Error Handling

Examples include:

* Failed routine creation.
* Failed routine update.
* Failed product assignment.
* Network interruption.
* Synchronization issues.

Users should receive clear feedback and recovery options.

---

# Edge Cases

Routines should gracefully support:

* Large routines.
* Duplicate products.
* Empty routines.
* Offline changes.
* Deleted products.

---

# Accessibility

Routines should support:

* Screen readers.
* Dynamic text sizes.
* Accessible drag-and-drop interactions.
* Logical navigation order.
* Comfortable touch targets.

---

# Analytics Events

Potential analytics events include:

* Routine Created
* Routine Updated
* Routine Deleted
* Product Added to Routine
* Product Removed from Routine
* Routine Viewed

Analytics should support product improvements while respecting user privacy.

---

# Database Impact

Routines store user-created organizational data and maintain relationships between users and products.

Each routine contains ordered product references and optional user notes.

Detailed schema definitions are documented within the Technical Architecture volume.

---

# API Requirements

Routines require functionality for:

* Create Routine
* Update Routine
* Delete Routine
* Retrieve Routines
* Add Product to Routine
* Remove Product from Routine
* Reorder Routine Steps

Implementation details are documented separately.

---

# Security & Permissions

Users may only access and manage their own routines.

All routine data should be protected through authentication and Row Level Security (RLS).

---

# Performance Considerations

Routines should:

* Load quickly.
* Synchronize efficiently.
* Preserve ordering reliably.
* Scale with growing libraries.

---

# Acceptance Criteria

The feature is complete when users can:

* Create routines.
* Add Library products to routines.
* Reorder routine steps.
* Add optional notes.
* Edit and delete routines.
* Access routines across devices.

---

# Future Enhancements

Potential future improvements include:

* Routine reminders.
* Routine scheduling.
* Routine completion tracking.
* AI-generated routines.
* Ingredient conflict detection.
* Routine effectiveness insights.
* Seasonal routine suggestions.

---

# Product Decisions

BloomVault treats routines as organizational tools rather than habit trackers.

The purpose of routines is to help users understand how products fit together and to provide structure for their beauty journey. Routines should support learning, planning, and personalization without creating pressure through streaks, completion goals, or productivity metrics.

The Library remains the foundation of every routine, reinforcing BloomVault's identity as a personal beauty knowledge library.

---

> **BloomVault**

> *Your Personal Beauty Library.*
