# Fiocchi Popcorn Website Flowchart

## Simple User Journey

```mermaid
graph TD
    A[User Visit] --> B{Login?}
    B -->|Yes| C[Authenticate]
    B -->|No| D[Browse]

    C --> E{Role?}
    E -->|Customer| F[Home]
    E -->|Admin| G[Dashboard]

    D --> H[View Products]
    H --> I{Buy?}
    I -->|Yes| J[Add to Cart]
    I -->|No| K[Flavor Lab]

    J --> L[Checkout]
    K --> M[Vote]
    M --> H

    L --> N[Order]
    F --> H
    G --> O[Analytics]
```

## Mobile Flow

```mermaid
graph TB
    A[Mobile User] --> B[Menu]
    B --> C{Option}
    C -->|Home| D[Homepage]
    C -->|Collection| E[Products]
    C -->|Flavor Lab| F[Voting]
    C -->|Login| G[Auth]

    D --> H[Browse]
    E --> I[Filter]
    F --> J[Vote]
    G --> K{Role}
```

## Purchase Flow

```mermaid
graph LR
    A[Browse] --> B[Add Cart]
    B --> C[Checkout]
    C --> D[Payment]
    D --> E[Confirm]
    E --> F[Receive]
```

## Key Features

- Clean, simplified flows
- Focus on main user paths
- Mobile-friendly navigation
- Clear decision points
- Minimal but complete coverage