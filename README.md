# cv
Vous trouverez ici les informations professionelles me concernant

```mermaid
---
config:
  theme: redux
---
flowchart TB
    A(["Commencer"]) --> B{"Sélectionner difficulté"}
    B --> C["Easy"] & D["Medium"] & E["Hard"] & F["Expert"]
    C --> G["Montrer HUD"]
    D --> G
    E --> G
    F --> G
    G --> H["Countdown"]
    H --> I["Montrer cible"]
    I --> J["Cliquer"] & K["Temps écoulé"]
    J --> L["Temps terminé"]
    K --> L
    L --> M["Recommencer"]
    M --> A
