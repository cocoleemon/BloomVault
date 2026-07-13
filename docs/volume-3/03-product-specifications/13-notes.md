# Personal Notes

Feature ID: BV-013
Volume: III — Product Specifications
File: 13-notes.md
Status: Draft
Version: 0.1.0
Last Updated: July 13, 2026
Owner: Coleen Ligasan

---

# 🌸 Overview

**Feature ID:** BV-013

Personal Notes allow users to record their own thoughts, observations, and experiences for individual beauty products.

Rather than relying on memory, users can build a personal record that grows alongside their beauty journey.

Every note belongs to a specific product, making BloomVault not only a product library, but also a library of personal experiences.

---

# Purpose

Personal Notes help users remember information that cannot be found on product labels or ingredient lists.

These notes transform products from simple catalog entries into meaningful personal references.

The goal is to support learning through experience.

---

# Problem It Solves

Beauty enthusiasts often remember products through personal experiences rather than specifications.

Examples include:

- "This irritated my skin."
- "Perfect under makeup."
- "Too heavy for daytime."
- "Repurchase!"
- "Works better during winter."

Without a dedicated place to store these thoughts, users rely on memory, screenshots, or external note-taking apps.

BloomVault keeps those experiences directly connected to the product they belong to.

---

# Goals

Personal Notes should:

- Preserve personal experiences.
- Help users remember why they saved a product.
- Support future purchasing decisions.
- Improve routine planning.
- Grow naturally over time.

---

# User Stories

### Record an Experience

**As a user, I want to write notes about a product so I can remember how it worked for me.**

---

### Revisit Previous Thoughts

**As a user, I want to review my previous notes before repurchasing or recommending a product.**

---

### Update My Experience

**As a user, I want to edit my notes over time as my opinions change.**

---

# Functional Requirements

Users shall be able to:

- Create a note for a product.
- Edit an existing note.
- Delete a note.
- View notes directly from Product Details.

Each product supports one continuously editable note.

---

# Business Rules

- Notes belong to individual products.
- A product can have only one note.
- Notes are private.
- Notes sync across devices.
- Notes remain available until deleted by the user.

---

# User Flow

```text
Product Details

↓

Personal Notes

↓

Write / Edit Note

↓

Save

↓

Return to Product Details
```

---

# Screen Relationships

Personal Notes connect with:

- Product Details
- Library
- Collections
- Wishlist
- Routines

Notes are always accessed through the Product Details page.

---

# User Interface

The Notes section appears within Product Details.

Possible actions include:

- Add Note
- Edit Note
- Delete Note

The interface should prioritize simplicity and readability.

---

# Empty State

When no note exists:

> *"Capture your thoughts about this product. Your future self will thank you."*

---

# Error Handling

Examples include:

- Failed save.
- Sync conflict.
- Offline changes.

BloomVault should automatically preserve drafts whenever possible.

---

# Accessibility

Notes should support:

- Screen readers
- Dynamic text sizes
- Keyboard accessibility
- Large touch targets

---

# Analytics

Potential analytics events:

- Note Created
- Note Updated
- Note Deleted

Analytics should improve product quality while respecting user privacy.

---

# Database Impact

Each note stores:

- Product ID
- User ID
- Note content
- Created date
- Last updated date

Each product may contain only one note per user.

---

# API Requirements

The Notes feature requires endpoints for:

- Create Note
- Retrieve Note
- Update Note
- Delete Note

---

# Security

Notes are private.

Only the owner may create, view, edit, or delete their notes.

---

# Performance

Notes should:

- Load instantly with Product Details.
- Auto-save drafts when appropriate.
- Synchronize efficiently across devices.

---

# Acceptance Criteria

The feature is complete when users can:

- Write notes for a product.
- Edit notes.
- Delete notes.
- View notes whenever they revisit the product.

---

# Future Enhancements

Potential future improvements include:

- Rich text formatting
- Photo attachments
- Voice notes
- Timeline of note edits
- AI-generated summaries of long notes

---

# Product Decisions

Personal Notes are intentionally simple.

BloomVault does not attempt to become a journaling application.

Instead, notes exist to capture meaningful observations that help users better understand products through their own experiences.

Every note should answer one question:

> **"What would my future self want to remember about this product?"**

---

> **BloomVault**

> *Your Personal Beauty Library.*