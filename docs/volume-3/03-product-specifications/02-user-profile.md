# Me

**Feature ID:** BV-002
**Volume:** III — Product Specifications
**File:** 02-me.md
**Status:** Draft
**Version:** 0.1.0
**Last Updated:** July 13, 2026
**Owner:** Coleen Ligasan

---

# 🌸 Overview

The Me stores personal preferences and account information that allow BloomVault to deliver a more personalized and relevant experience.

Unlike social media profiles, the Me is private and exists solely to support the user's beauty journey.

It helps BloomVault understand the user's preferences while giving users complete control over the information they choose to share.

---

# Purpose

Provide a central location where users can:

* Manage their account.
* Personalize their BloomVault experience.
* Store beauty preferences.
* Update profile information.
* Control privacy and notification settings.

The profile should feel helpful rather than overwhelming.

---

# Problem It Solves

Every person's beauty journey is unique.

Without personalization:

* Product recommendations become generic.
* Ingredient guidance may not be relevant.
* Future AI assistance lacks context.
* The experience feels less personal.

The User Profile provides optional context that helps BloomVault become a smarter beauty companion over time.

---

# Goals

The Me should:

* Keep personal information organized.
* Support meaningful personalization.
* Minimize onboarding friction.
* Respect user privacy.
* Grow alongside the user's evolving beauty journey.

---

# User Stories

### Account Management

**As a user, I want to manage my account information so I can keep my BloomVault profile up to date.**

---

### Personalization

**As a user, I want to store my beauty preferences so BloomVault can provide more relevant recommendations and insights.**

---

### Privacy

**As a privacy-conscious user, I want complete control over the information I choose to share.**

---

### Flexible Setup

**As a new user, I want to skip optional profile details and complete them later so I can start using BloomVault immediately.**

---

# Functional Requirements

The User Profile shall allow users to:

* View account information.
* Update display name.
* Change profile photo (optional).
* Update email address.
* Change password.
* Manage beauty preferences.
* Manage notification preferences.
* Sign out.

Future versions may also include account export and deletion.

---

# Beauty Profile

The Beauty Profile is an optional section that stores personal preferences to improve the BloomVault experience.

Possible fields include:

### Skin

* Skin Type
* Skin Concerns
* Sensitivity Level

### Hair

* Hair Type
* Hair Concerns

### Body

* Body Care Goals

### Makeup

* Makeup Style
* Preferred Finish

### Fragrance

* Favorite Fragrance Families

### Shopping

* Budget Preference
* Favorite Brands

All fields should remain optional and editable at any time.

---

# Business Rules

* Every user has exactly one profile.
* Beauty Profile information is optional.
* Users may update preferences at any time.
* Personal information remains private and is never publicly displayed.
* Profile changes should sync across devices.

---

# User Flow

Library

↓

Me

↓

View Account

↓

Edit Information

↓

Save Changes

↓

Return to Library

---

# Screen Relationships

The User Profile connects with:

* Authentication
* Library
* Settings
* Notifications
* Routines
* AI Beauty Librarian (Future)

---

# UI Components

The profile may include:

* Profile photo
* Display name
* Email address
* Beauty Profile section
* Notification settings
* Privacy settings
* Sign Out button

The layout should remain clean and easy to navigate.

---

# User Interface Behavior

The User Profile should:

* Save changes automatically where appropriate.
* Clearly indicate unsaved changes when manual confirmation is required.
* Provide immediate feedback after successful updates.
* Allow users to edit information without leaving the screen.

---

# States

Supported states include:

* Loading
* Viewing
* Editing
* Saving
* Success
* Error
* Offline

The editing experience should feel smooth and reassuring.

---

# Empty States

Optional profile fields should display friendly prompts encouraging users to personalize their experience without creating pressure.

For example:

*"Tell us a little about your skin to help BloomVault personalize future recommendations."*

---

# Error Handling

Examples include:

* Invalid email format.
* Email already in use.
* Failed profile update.
* Failed image upload.
* Network interruption.

Errors should clearly explain what happened and how users can recover.

---

# Edge Cases

The User Profile should gracefully support:

* Skipped onboarding.
* Incomplete Beauty Profiles.
* Profile updates while offline.
* Changing email addresses.
* Removing optional information.

---

# Accessibility

The User Profile should support:

* Screen readers.
* Dynamic text sizes.
* Large touch targets.
* Clear labels.
* Accessible forms.
* Logical navigation order.

---

# Analytics Events

Potential analytics events include:

* Profile Viewed
* Profile Updated
* Beauty Profile Completed
* Notification Preferences Changed
* Sign Out

Analytics should be used to improve the experience while respecting user privacy.

---

# Database Impact

The User Profile stores user-specific information including:

* Account details
* Beauty preferences
* Notification preferences
* Profile image reference

Database structure is defined in the Technical Architecture documentation.

---

# API Requirements

The User Profile requires functionality for:

* Retrieve profile
* Update profile
* Upload profile image
* Update preferences
* Update notification settings

Implementation details are defined separately.

---

# Security & Permissions

Users may only access and modify their own profile.

Sensitive account information should be protected through authentication, authorization, and Row Level Security (RLS).

---

# Performance Considerations

The User Profile should:

* Load quickly.
* Cache profile information where appropriate.
* Synchronize updates efficiently.
* Avoid unnecessary network requests.

---

# Acceptance Criteria

The feature is complete when users can:

* View their account information.
* Update profile details.
* Manage beauty preferences.
* Update notification settings.
* Synchronize profile changes across devices.
* Securely sign out.

---

# Future Enhancements

Potential future improvements include:

* Skin quiz
* Hair quiz
* Beauty goals
* Routine preferences
* AI-powered personalization
* Data export
* Account deletion
* Profile backup and restore

---

# Product Decisions

BloomVault intentionally treats the User Profile as a private personalization tool rather than a public identity.

The goal is not to create a social profile but to help BloomVault better understand each user's unique beauty journey.

All personalization should remain optional, allowing users to enjoy the app immediately while adding more context over time.

---

> **BloomVault**

> *Your Personal Beauty Library.*
