# Ingredient Explorer

**Feature ID:** BV-011  
**Volume:** III — Product Specifications  
**File:** 11-ingredient-explorer.md  
**Status:** Draft  
**Version:** 0.1.0  
**Last Updated:** July 13, 2026  
**Owner:** Coleen Ligasan

---

# 🌸 Overview

Ingredient Explorer helps users understand the ingredients found in beauty products through clear, approachable, and reliable explanations.

Rather than presenting scientific information without context, BloomVault explains what ingredients commonly do, who they may benefit, and where they appear throughout the user's personal Beauty Library.

Ingredient Explorer transforms ingredient lists from something intimidating into something meaningful.

---

# Purpose

Provide users with an easy way to learn about beauty ingredients while researching products.

Ingredient Explorer should help users:

- Understand what common ingredients do.
- Learn ingredient benefits in simple language.
- Discover which products contain a specific ingredient.
- Build confidence when reading ingredient lists.
- Support more informed beauty decisions.

---

# Problem It Solves

Ingredient lists are often long, technical, and difficult to understand.

Users frequently leave shopping apps to search Google, Reddit, or ingredient websites just to answer questions like:

- What is Niacinamide?
- Is Panthenol good for sensitive skin?
- Which of my products contain Centella?
- Should I avoid this ingredient?

This fragmented research experience interrupts learning and makes product evaluation more difficult.

Ingredient Explorer brings that knowledge directly into BloomVault.

---

# Goals

Ingredient Explorer should:

- Make ingredient research approachable.
- Explain concepts in everyday language.
- Connect ingredients to products.
- Encourage curiosity.
- Build beauty knowledge over time.

BloomVault should educate rather than overwhelm.

---

# User Stories

### Learn About Ingredients

**As a user, I want simple explanations so I can understand what ingredients actually do.**

---

### Find Products by Ingredient

**As a user, I want to see which products contain a specific ingredient so I can explore alternatives or compare formulations.**

---

### Understand My Library

**As a user, I want to know which ingredients appear across my saved products so I can better understand my routine.**

---

### Research While Browsing

**As a user, I want to tap any ingredient from a product page and immediately learn more about it without leaving the app.**

---

# Functional Requirements

Ingredient Explorer shall allow users to:

- Browse ingredients.
- Search ingredients by name.
- Open ingredient details.
- View ingredient descriptions.
- View common benefits.
- View common skin concerns addressed.
- View commonly paired ingredients.
- View considerations and usage notes.
- View products containing the ingredient.
- View products from the user's Library containing the ingredient.

---

# Business Rules

- Ingredient information is educational only.
- BloomVault does not provide medical advice.
- Ingredient information should remain neutral.
- No ingredient should be labeled as universally "good" or "bad."
- Product-specific formulations may behave differently from ingredient summaries.

---

# Ingredient Information

Each ingredient page may include:

- Ingredient name
- Alternative names (if applicable)
- Short description
- Primary functions
- Common benefits
- Suitable skin types
- Skin concerns commonly addressed
- Texture or formulation notes (when relevant)
- Commonly paired ingredients
- Things to be mindful of
- Related products

Content should prioritize clarity over scientific complexity.

---

# Product Integration

Ingredient Explorer should integrate naturally throughout BloomVault.

Users should be able to:

- Tap an ingredient from Product Details.
- Open Ingredient Explorer directly.
- View products in their Library containing that ingredient.
- Discover additional products containing the ingredient.

This creates a seamless learning experience without interrupting product research.

---

# User Flow

Product Details, Search, or Discover

↓

Tap Ingredient

↓

Ingredient Explorer

↓

Read Ingredient Information

↓

Browse Related Products

↓

Return to Product or Continue Exploring

---

# Screen Relationships

Ingredient Explorer connects with:

- Product Details
- Library
- Discover
- Search
- Compare

Ingredients become another way to navigate BloomVault's knowledge base.

---

# UI Components

Ingredient Explorer may include:

- Search bar
- Ingredient cards
- Ingredient summary
- Benefit badges
- Skin concern badges
- Products containing the ingredient
- Products in Your Library section
- Related ingredients

The interface should prioritize readability and learning.

---

# User Interface Behavior

Ingredient Explorer should:

- Load quickly.
- Support fast searching.
- Display information progressively.
- Encourage exploration through related ingredients.
- Provide quick access back to Product Details.

---

# States

Supported states include:

- Empty
- Loading
- Populated
- Searching
- Offline
- Error

Transitions should remain smooth and intuitive.

---

# Empty States

When no ingredients match a search:

*"We couldn't find that ingredient. Try another search or browse popular ingredients."*

---

# Error Handling

Examples include:

- Ingredient unavailable.
- Failed search.
- Network interruption.
- Missing ingredient information.

Users should always receive clear feedback.

---

# Edge Cases

Ingredient Explorer should gracefully support:

- Ingredients with multiple names.
- Products with incomplete ingredient lists.
- Missing descriptions.
- Offline viewing of cached ingredients.
- Ingredients appearing in many products.

---

# Accessibility

Ingredient Explorer should support:

- Screen readers.
- Dynamic text sizes.
- Accessible search.
- Logical navigation order.
- Clear heading hierarchy.

---

# Analytics Events

Potential analytics events include:

- Ingredient Viewed
- Ingredient Searched
- Product Opened from Ingredient
- Related Ingredient Selected

Analytics should improve the product while respecting user privacy.

---

# Database Impact

Ingredient Explorer stores a master ingredient catalog and maintains relationships between ingredients and products.

It also references products within the user's Library to provide personalized ingredient insights.

Detailed schema definitions are documented within the Technical Architecture volume.

---

# API Requirements

Ingredient Explorer requires functionality for:

- Retrieve ingredient list
- Search ingredients
- Retrieve ingredient details
- Retrieve products by ingredient
- Retrieve Library products containing ingredient
- Retrieve related ingredients

Implementation details are documented separately.

---

# Security & Permissions

Ingredient information is publicly accessible.

Personalized sections, such as "Products in Your Library," require user authentication and appropriate Row Level Security (RLS).

---

# Performance Considerations

Ingredient Explorer should:

- Load ingredient pages quickly.
- Cache frequently viewed ingredients.
- Support efficient searching.
- Handle ingredients associated with many products.

---

# Acceptance Criteria

The feature is complete when users can:

- Search ingredients.
- Read ingredient information.
- Open Ingredient Explorer from Product Details.
- View products containing the ingredient.
- View products in their own Library containing the ingredient.
- Navigate easily between ingredients and products.

---

# Future Enhancements

Potential future improvements include:

- AI-powered ingredient explanations.
- Ingredient interaction guidance.
- Ingredient compatibility insights.
- Trending ingredients.
- Personalized ingredient recommendations.
- Ingredient learning paths.
- Ingredient safety summaries.
- Barcode-to-ingredient navigation.

---

# Product Decisions

Ingredient Explorer exists to make beauty education approachable.

Rather than overwhelming users with scientific terminology, BloomVault presents ingredient information in a way that is practical, easy to understand, and directly connected to the products users are researching.

The goal is not to replace professional advice, but to help users build confidence through knowledge.

Ingredient Explorer reinforces BloomVault's philosophy that better beauty decisions begin with better understanding.

---

> **BloomVault**

> *Your Personal Beauty Library.*