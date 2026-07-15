# 🌸 File Storage

> *"Images preserve the beauty that words alone cannot capture."*

---

# Introduction

BloomVault uses Supabase Storage to manage images and other files required throughout the platform.

Rather than storing binary files directly in the database, BloomVault stores file references while the actual files are securely managed within cloud storage.

This approach improves performance, scalability, and maintainability.

---

# Purpose

The File Storage architecture aims to:

- Store media efficiently.
- Reduce database size.
- Protect uploaded files.
- Support scalable storage.
- Organize assets consistently.

---

# Storage Provider

BloomVault uses:

- Supabase Storage

Supabase Storage provides secure, scalable object storage integrated with authentication and access policies.

---

# Storage Domains

Storage is organized into three primary domains.

## 🌍 Beauty Catalog

Shared media available to all users.

Examples include:

- Product Images
- Brand Logos
- Category Images (future)
- Ingredient Icons (future)

---

## 📚 Personal Library

Private user-owned media.

Future examples include:

- Custom Collection Covers
- Routine Photos
- Personal Beauty Shelf Photos
- Other user-uploaded assets

Access is restricted to the owning user through security policies.

---

## ⚙️ Platform

Shared application assets.

Examples include:

- Application illustrations
- Empty state graphics
- Default avatars
- Promotional assets

These support the overall user experience without belonging to individual users.

---

# Storage Organization

Example storage structure:

```text
catalog/
├── products/
├── brands/

library/
├── collections/
├── uploads/

platform/
├── assets/
├── illustrations/
```

This organization mirrors BloomVault's domain-driven architecture.

---

# File References

The database stores references to files rather than the files themselves.

Example:

- Product image URL
- Brand logo URL
- Collection cover URL

This separation keeps the database lightweight and improves storage efficiency.

---

# Security

Storage security includes:

- Authenticated access
- Row Level Security integration
- Bucket access policies
- Signed URLs where appropriate

Private user files should never be publicly accessible unless explicitly shared in future platform features.

---

# Performance

The storage system should prioritize:

- Optimized image delivery
- Efficient file retrieval
- Scalable storage growth
- Minimal bandwidth usage

Images should be appropriately sized for mobile devices to improve loading performance.

---

# Future Growth

The storage architecture supports future capabilities including:

- Multiple product images
- User-generated media
- AI-generated visuals
- Product comparison galleries
- Image optimization
- Content Delivery Network (CDN) enhancements

These additions can be introduced without changing the overall storage organization.

---

# Design Decisions

BloomVault separates media storage from relational data.

By storing files within Supabase Storage and keeping only references in the database, the platform remains scalable while preserving a clean and efficient database structure.

The storage organization mirrors the platform's knowledge domains, creating consistency across the entire architecture.

---

# File Storage Summary

The File Storage architecture provides a secure and scalable foundation for managing BloomVault's media assets.

Through domain-based organization and cloud storage, BloomVault delivers efficient media management while supporting future growth and richer user experiences.

---

> **Beautiful knowledge deserves beautiful presentation.**

> **BloomVault**

> *Your Personal Beauty Library.*