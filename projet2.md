# Mise à jour 2

## Principaux changements
* **Changements de la structure HTML et CSS** de base.
* **Mise en place du suivi de la souris** (`mousemove`) nécessaire pour détecter l'inactivité de l'utilisateur.
* **Affichage des coordonnées de positionnement** (feedback) via une **fenêtre contextuelle** (`popup`) qui apparaît après **2000 ms** (2 secondes).

---

## Contribution de l'IA et Assistance (presque la même qu'avant)
* **Outil utilisé :** Gemini
* **Défi :** La logique **JavaScript**.
* **Résultat :** J'ai sollicité l'aide de **Gemini** pour comprendre la logique de l'event 'setTimeOut', le même ami a ensuite revu le code et ajouté des commentaires pour clarifier chaque partie pour moi.

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