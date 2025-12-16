# Mise à jour 1 (Initialisation)

## Principaux changements
* **Implémentation de la structure HTML et CSS** de base du jeu.
* **Mise en place du suivi de la souris** (`mousemove`) nécessaire pour détecter l'inactivité de l'utilisateur.
* **Affichage des coordonnées de positionnement** (à des fins de débogage initial).

---

## Contribution de l'IA et Assistance
* **Outil utilisé :** Gemini
* **Défi :** La logique **JavaScript** a nécessité une assistance.
* **Résultat :** J'ai sollicité l'aide de **Gemini** et d'un **collaborateur** (ami) pour comprendre la structure et les concepts de base nécessaires au suivi de la souris et à la mise en œuvre de la logique de jeu.

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