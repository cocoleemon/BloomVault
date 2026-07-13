# Compare

**Feature ID:** BV-009
**Volume:** III — Product Specifications
**File:** 09-compare.md
**Status:** Draft
**Version:** 0.1.0
**Last Updated:** July 13, 2026
**Owner:** Coleen Ligasan

---

# 🌸 Overview

Compare allows users to evaluate beauty products side by side, making it easier to understand similarities and differences before making a decision.

Rather than recommending a "better" product, BloomVault presents objective information in a clear, organized format so users can make informed decisions based on their own needs, preferences, and routines.

Comparison is designed to support learning—not persuasion.

---

# Purpose

Provide users with a simple and reliable way to compare products before purchasing or adding them to their routine.

Compare should help users:

* Understand product differences.
* Evaluate ingredients and formulations.
* Compare suitability for different skin types.
* Make more informed beauty decisions.
* Reduce decision fatigue.

---

# Problem It Solves

Beauty products often appear similar, making it difficult to understand how they actually differ.

Users frequently switch between multiple product pages, ingredient websites, social media posts, and notes to compare products manually.

This fragmented process makes research time-consuming and increases the likelihood of confusion or impulse purchases.

Compare brings relevant information together into one focused view.

---

# Goals

Compare should:

* Present information objectively.
* Make differences easy to understand.
* Reduce unnecessary research effort.
* Support thoughtful decision-making.
* Encourage learning instead of ranking.

BloomVault should never declare one product as universally better than another.

---

# User Stories

### Compare Two Products

**As a user, I want to compare two products side by side so I can better understand their differences.**

---

### Make Better Decisions

**As a user, I want clear comparisons so I can choose products that fit my needs rather than relying on marketing claims.**

---

### Compare My Research

**As a user, I want to compare products I've saved so I can decide which one best fits my routine.**

---

# Functional Requirements

Compare shall allow users to:

* Select two products.
* View products side by side.
* Compare product specifications.
* Compare ingredient highlights.
* Compare skin type suitability.
* Compare texture and finish (when available).
* View personal notes alongside compared products.
* Open Product Details from the comparison.

---

# Business Rules

* Users may compare two products at a time.
* Products do not need to belong to the user's Library.
* Comparison data should remain neutral.
* BloomVault should never rank products or recommend a winner.

---

# Comparison Categories

Comparison may include:

* Product image
* Product name
* Brand
* Category
* Size
* Price (if available)
* Key ingredients
* Full ingredient list
* Benefits
* Skin type suitability
* Texture
* Finish
* Fragrance
* Alcohol
* Product claims
* User notes

Only available information should be displayed.

---

# User Flow

Library, Discover, Search, or Product Details

↓

Select Compare

↓

Choose Second Product

↓

Comparison View

↓

Open Product Details or Return

---

# Screen Relationships

Compare connects with:

* Library
* Product Details
* Search
* Discover
* Collections
* Wishlist

---

# UI Components

The Compare screen may include:

* Two product panels
* Side-by-side comparison table
* Highlighted differences
* Personal notes section
* Swap products button
* Remove product action
* Empty State

The layout should prioritize readability on mobile devices.

---

# User Interface Behavior

Compare should:

* Highlight differences without implying superiority.
* Keep matching attributes visually aligned.
* Allow users to swap products easily.
* Load comparison data quickly.
* Preserve scroll position when appropriate.

---

# States

Supported states include:

* Empty
* Loading
* Comparing
* Error
* Offline

---

# Empty States

When no products have been selected:

*"Choose two products to see their similarities and differences side by side."*

---

# Error Handling

Examples include:

* Product unavailable.
* Failed comparison data.
* Network interruption.
* Missing product information.

Users should always receive clear feedback.

---

# Edge Cases

Compare should gracefully support:

* Products with incomplete information.
* Products from different categories.
* Duplicate product selection.
* Offline viewing of previously loaded comparisons.

---

# Accessibility

Compare should support:

* Screen readers.
* Dynamic text sizes.
* Accessible tables and labels.
* Logical reading order.
* High contrast where appropriate.

---

# Analytics Events

Potential analytics events include:

* Comparison Started
* Product Added to Comparison
* Product Removed from Comparison
* Comparison Viewed
* Comparison Shared (future)

---

# Database Impact

Comparison does not permanently store comparison results.

It retrieves product information dynamically and may reference the user's personal notes when available.

---

# API Requirements

Compare requires functionality for:

* Retrieve comparison data.
* Retrieve product attributes.
* Retrieve personal notes.
* Load comparison metadata.

Implementation details are documented separately.

---

# Security & Permissions

Users may only access their own notes and private data during comparisons.

Public product information should remain available to all users.

---

# Performance Considerations

Compare should:

* Load efficiently.
* Cache recently viewed comparisons.
* Optimize side-by-side rendering.
* Handle incomplete product data gracefully.

---

# Acceptance Criteria

The feature is complete when users can:

* Compare two products.
* Clearly understand similarities and differences.
* View their own notes within comparisons.
* Open Product Details from either product.
* Compare products without performance issues.

---

# Future Enhancements

Potential future improvements include:

* Compare up to three products.
* AI-generated comparison summaries.
* Highlight ingredient conflicts.
* Routine compatibility insights.
* Export comparison results.
* Share comparison links.

---

# Product Decisions

Comparison exists to educate rather than persuade.

BloomVault intentionally avoids ranking products or declaring winners. Instead, it provides organized information that empowers users to make decisions based on their own goals, skin concerns, and preferences.

Every comparison should leave users feeling more informed—not more influenced.

---

> **BloomVault**

> *Your Personal Beauty Library.*
