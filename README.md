# Simple Node Portfolio - Application Web Statique avec Node.js et Express
![Animation Portfolio Web en Node.js](https://i.giphy.com/media/v1.Y2lkPTc5MGI3NjExZHVldWtlbjZ1Z2h3bG9tN2p6M2t3bG83c2I0eHgyeXRtZHB4eWhjYSZlcD12MV9pbnRlcm5hbF9naWZfYnlfaWQmY3Q9Zw/3o7TKnN6HfARXHcly8/giphy.gif)
[![Licence GitHub](https://img.shields.io/github/license/angoularaphael/simple-node-portfolio?style=flat-square)](https://github.com/angoularaphael/simple-node-portfolio/blob/main/LICENSE)
[![Étoiles GitHub](https://img.shields.io/github/stars/angoularaphael/simple-node-portfolio?style=flat-square)](https://github.com/angoularaphael/simple-node-portfolio/stargazers)
[![Forks GitHub](https://img.shields.io/github/forks/angoularaphael/simple-node-portfolio?style=flat-square)](https://github.com/angoularaphael/simple-node-portfolio/network)
[![Problèmes GitHub](https://img.shields.io/github/issues/angoularaphael/simple-node-portfolio?style=flat-square)](https://github.com/angoularaphael/simple-node-portfolio/issues)
[![Badge Visiteurs](https://visitor-badge.laobi.icu/badge?page_id=angoularaphael.simple-node-portfolio&format=true)](https://github.com/angoularaphael/simple-node-portfolio)
## Description
Simple Node Portfolio est une application web open-source développée en Node.js avec Express, servant un site statique pour un portfolio personnel. Elle inclut des pages HTML/CSS/JS basiques avec un serveur Node pour gérer les routes et servir les fichiers statiques. Idéale pour démontrer des compétences en développement web back-end léger, intégration front-end, et déploiement. Parfaite pour les débutants en Node.js cherchant à créer un site responsive et dynamique.
![Animation Site Portfolio Dynamique](https://cdn.dribbble.com/users/1162077/screenshots/3848921/programmer.gif)
## Fonctionnalités
- **Serveur Express** : Gestion des routes et service de fichiers statiques.
- **Pages Statiques** : Portfolio avec sections Accueil, Projets, Contact (HTML/CSS/JS).
- **Responsive Design** : Utilisation de CSS pour une adaptation mobile/desktop.
- **Intégration JS** : Scripts simples pour interactions (ex. : formulaire de contact basique).
- **Déploiement Facile** : Prêt pour Heroku, Vercel ou GitHub Pages (statique seulement).
## Démo
Voici comment fonctionne un peu cette application.
![Animation Démo Portfolio en Node.js](https://www.smartsheet.com/sites/default/files/4_Inventory-Stock-Control-animation_1.gif)
## Installation
Pour démarrer avec Simple Node Portfolio :
1. Clonez le dépôt :
   ```
   git clone https://github.com/angoularaphael/simple-node-portfolio.git
   ```
2. Installez les dépendances :
   ```
   npm install
   ```
3. Lancez le serveur :
   ```
   node server.js
   ```
4. Ouvrez http://localhost:3000 dans votre navigateur.
**Note** : Assurez-vous d'avoir Node.js installé (version 14 ou supérieure recommandée pour une compatibilité optimale avec Express).
## Utilisation
- Accédez au site via le navigateur après lancement du serveur.
- Personnalisez le contenu : Modifiez les fichiers dans le dossier `public/` (index.html, style.css, script.js).
- Ajoutez des routes : Éditez `server.js` pour de nouvelles pages ou API.
Exemple de code Node.js basique pour le serveur (extrait de `server.js`) :
```javascript
const express = require('express');
const path = require('path');
const app = express();
const PORT = 3000;

app.use(express.static(path.join(__dirname, 'public')));

app.get('/', (req, res) => {
  res.sendFile(path.join(__dirname, 'public', 'index.html'));
});

app.listen(PORT, () => {
  console.log(`Serveur lancé sur http://localhost:${PORT}`);
});
```
## Contribution
Les contributions sont les bienvenues ! Suivez ces étapes :
1. Forkez le dépôt.
2. Créez une nouvelle branche : `git checkout -b feature/votre-fonctionnalite`.
3. Commitez vos changements : `git commit -m 'Ajout d'une nouvelle fonctionnalité'`.
4. Poussez la branche : `git push origin feature/votre-fonctionnalite`.
5. Ouvrez une Pull Request.
Consultez [CONTRIBUTING.md](CONTRIBUTING.md) pour plus de détails (créez ce fichier si nécessaire).
## Licence
Ce projet est sous licence MIT - voir le fichier [LICENSE](LICENSE) pour plus de détails.
## Contact
- Mainteneur : @angoularaphael
- GitHub : [angoularaphael](https://github.com/angoularaphael)
- Email : germainraphaelangoulaonambele@gmail.com
---
