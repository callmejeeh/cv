# Mise à jour 3

## Principaux changements
* **Changements de la structure HTML et CSS** de base.
* **Mise en place du suivi de la souris** et premiers conceptions du jeu.
* **Affichage d'un cible cliquable** qu'apparaît après 2000ms que la souris a été arreté

---

## Contribution de l'IA et Assistance (presque la même qu'avant)
* **Outil utilisé :** Gemini
* **Défi :** La logique **JavaScript**.

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