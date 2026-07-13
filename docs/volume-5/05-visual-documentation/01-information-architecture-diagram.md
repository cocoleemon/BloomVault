# 🌸 Information Architecture Diagram

```mermaid
flowchart TD

A[Authentication]

A --> B[Library]
A --> C[Discover]
A --> D[Search]
A --> E[Me]

B --> F[Product Details]
C --> F
D --> F

F --> G[Ingredient Explorer]
F --> H[Brand]
F --> I[Compare]

F --> J[Collections]
F --> K[Wishlist]
F --> L[Routines]
F --> M[Personal Notes]
```