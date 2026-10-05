# Gromozeka

<p align="center">
  <img src="assets/images/gromozeka.png" width="480" alt="Gromozeka holding six books" />
</p>

Gromozeka is a local-first knowledge synthesis tool that turns books, articles, documentation, and other materials into a unified, verifiable document. It combines overlapping knowledge while preserving important details, differing perspectives, contradictions, and links to the original sources.

```mermaid
flowchart LR
    sources@{ shape: docs, label: "Books, articles<br/>and documentation" }
    processing("AI-assisted processing<br/>Extract and compare")
    synthesis{{"Knowledge synthesis<br/>Merge and preserve<br/>differences"}}
    output@{ shape: doc, label: "Unified document<br/>with source references" }

    sources --> processing --> synthesis --> output
    output -. "Traceable to originals" .-> sources

    classDef source fill:#eff6ff,stroke:#3b82f6,color:#1e3a8a
    classDef ai fill:#f5f3ff,stroke:#8b5cf6,color:#4c1d95
    classDef result fill:#ecfdf5,stroke:#10b981,color:#064e3b
    class sources source
    class processing,synthesis ai
    class output result
```
