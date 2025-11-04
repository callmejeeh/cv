# Projet de Codage
## Projet inspiré par le site Pointer Pointer

### Objectif
Le site **Pointer Pointer** a été conçu comme une expérience web ludique et interactive, dont le but est de surprendre et d’amuser l’utilisateur. Son principe est simple : peu importe où l’on place le curseur sur l’écran, une photographie apparaît montrant une personne qui semble pointer exactement vers ce point. L’objectif principal est donc de créer une illusion d’interaction humaine entre l’utilisateur et la collection d’images, tout en démontrant les possibilités créatives du web moderne en matière d’interactivité et d’expérience utilisateur.

### Technologies utilisées
**HTML**, **CSS** et **JavaScript** pour la partie front-end.  
- **HTML** structure la page et définit les éléments nécessaires à l’affichage des images.  
- **CSS** gère la mise en page, les transitions et l’aspect visuel épuré du site.  
- **JavaScript** détecte en temps réel la position du curseur et déclenche la recherche d’une image appropriée.  

Du côté du **serveur**, une base de données d’images préalablement analysées (où l’on a identifié la position du doigt pointé) est utilisée pour renvoyer l’image la plus adaptée en fonction des coordonnées du pointeur. Ce traitement peut être réalisé grâce à un langage côté serveur comme **PHP** ou **Node.js**, couplé à un algorithme de correspondance d’images.

### Fonctionnement
Le fonctionnement repose sur la détection des coordonnées du curseur (X et Y) sur la fenêtre du navigateur.  

1. Lorsque l’utilisateur déplace son pointeur ou clique sur un point de l’écran, le site envoie ces coordonnées au serveur.  
2. Le serveur recherche dans sa base de données une photo dont la personne semble pointer vers ce point précis, à l’aide d’un repérage prédéfini de la direction du doigt.  
3. Une fois l’image trouvée, elle est renvoyée au navigateur et affichée à l’écran, créant ainsi l’illusion que la personne sur la photo pointe vers le curseur de l’utilisateur.
