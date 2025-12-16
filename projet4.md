# Mise à jour 4

**Amélioration du concept de jeu :** Le point ne s'affiche plus immédiatement sur les coordonnées de la souris, mais apparaît désormais à une position aléatoire après la période d'inactivité (délai) de l'utilisateur.
* **Mise en œuvre d'une boucle de jeu :** Le système est configuré pour relancer un nouveau point immédiatement après un succès ou un échec.
* **Refonte et nettoyage du code :** Le code a été optimisé, les variables et les fonctions ont été renommées pour une meilleure lisibilité et le fichier a été nettoyé des lignes inutiles.

---

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