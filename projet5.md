# Mise à jour 5

* **Implémentation d'un chronomètre et d'un score (HUD) :** Le joueur dispose maintenant de 60 secondes pour accumuler le maximum de points possible.
* **Ajout des écrans de contrôle :** Mise en place des écrans d'initialisation et de fin de partie, affichant notamment le score final.
* **Intégration des boutons d'action :** Ajout des boutons pour **Démarrer** la partie et **Recommencer** le jeu.

## Contribution de l'IA et Assistance (presque la même qu'avant)
* **Outil utilisé :** Gemini
* **Défi :** La logique **JavaScript**, surtout pour faire le jeu recommencer.

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