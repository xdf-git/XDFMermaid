```mermaid
flowchart LR
    subgraph Token_Lifecycle["Carbon Credit Token Lifecycle"]
        A[Issuer / Project] --> B[Token Issuance on Polymath ST-20]
        B --> C[Token represents multiple tons of CO₂]
        C --> D[Partitions per Project or Vintage]
        D --> E[Investor / Holder Wallet]
        E --> F[Partial Transfer or Use]
        F --> G[Partial Burn / Retirement]
        G --> H[Blockchain Events Log - Redeemed/Retired]
    end
    subgraph Metadata["Metadata & Audit"]
        D --> I[Project ID, Vintage, Certificates Hash]
        G --> I
        H --> I
    end

