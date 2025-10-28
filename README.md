# Cyber Audit Dashboard

> Application web interactive bilingue (FR/EN) pour réaliser des audits de cybersécurité sur sites industriels

[![License: MIT](https://img.shields.io/badge/License-MIT-blue.svg)](https://opensource.org/licenses/MIT)
[![GitHub stars](https://img.shields.io/github/stars/K3E9X/cyber-audit-dashboard?style=social)](https://github.com/K3E9X/cyber-audit-dashboard)
[![GitHub forks](https://img.shields.io/github/forks/K3E9X/cyber-audit-dashboard?style=social)](https://github.com/K3E9X/cyber-audit-dashboard/fork)

## 🌟 Démo en ligne

**[Lancer l'application](https://k3e9x.github.io/cyber-audit-dashboard/)**

## ✨ Nouveautés v2.0

### 🗄️ Gestion avancée de l'historique
- **Base de données locale (IndexedDB)** : Stockage illimité d'audits
- **Recherche instantanée** : Trouvez vos audits par nom, site ou auditeur
- **Filtrage intelligent** : Par statut (Brouillon, En cours, Terminé, Validé)
- **Tri multi-critères** : Par date, nom ou progression
- **Statistiques globales** : Tableau de bord de tous vos audits

### 🔄 Comparaison d'audits
- **Vue côte à côte** : Comparez deux audits simultanément
- **Analyse des différences** : Identifiez rapidement les changements
- **Statistiques comparatives** : Évolution des conformités entre audits

### 🌐 Système bilingue FR/EN
- **Traduction complète** : 100% de l'interface en français et anglais
- **27 checkpoints traduits** : Titres, descriptions et preuves
- **Changement instantané** : Bascule de langue sans perte de données
- **Préférence sauvegardée** : La langue choisie est mémorisée

### 📥 Import/Export avancé
- **Export global JSON** : Exportez tous vos audits en un clic
- **Import JSON** : Importez des audits depuis un fichier
- **Actions de remédiation** : Champ dédié pour les recommandations

## 🎯 Fonctionnalités principales

### Dashboard interactif
- **Statistiques en temps réel** : Visualisation instantanée de l'état d'avancement
- **4 cartes statistiques** : Progression globale, conformes, non-conformes, partiels
- **Progression par catégorie** : Suivi détaillé des 5 catégories

### Système de sauvegarde multi-niveaux
- **Sauvegarde individuelle** : Chaque audit est enregistré séparément
- **Statuts d'audit** : Brouillon → En cours → Terminé → Validé
- **Métadonnées complètes** : Site, date, auditeur, responsable sécurité
- **Dates de création/modification** : Suivi temporel automatique

### Interface moderne et adaptative
- **Mode sombre/clair** : Confort visuel adapté à votre environnement
- **Responsive design** : Fonctionne sur desktop, tablette et mobile
- **Sidebar navigation** : Navigation fluide entre pages
- **Toasts de notification** : Feedback visuel pour chaque action
- **Modales de confirmation** : Sécurité pour les actions critiques

### Optimisé pour le terrain
- **Utilisation hors-ligne** : Fonctionne sans connexion internet
- **État vide intuitif** : Guide l'utilisateur lors de la première utilisation
- **Commentaires détaillés** : Zone de texte pour observations
- **Actions de remédiation** : Recommandations par checkpoint

## 📋 Points de contrôle couverts

L'application couvre **27 points de contrôle** répartis en **5 catégories** :

| Catégorie | Points | Description |
|-----------|--------|-------------|
| **Gouvernance** | 1 | Pilotage de la cybersécurité |
| **Ressources** | 9 | Cartographie SI, réseau, sauvegarde, PCA/PRA |
| **Contrôle d'accès** | 9 | Comptes, authentification, privilèges, journalisation |
| **Actifs** | 6 | Correctifs, sécurité postes/serveurs, données |
| **Physique** | 2 | Contrôles d'accès physiques |

### Détails par checkpoint
- **ID unique** : Identification claire (GOU-01, RES-01, etc.)
- **Titre et description** : Objectif du contrôle
- **Preuves à vérifier** : Liste de documents/éléments à contrôler
- **4 statuts possibles** : Conforme, Non conforme, Partiel, N/A
- **Champs de commentaires** : Observations détaillées
- **Actions de remédiation** : Recommandations d'amélioration

## 🚀 Utilisation

### Démarrage rapide

#### Page "Nouvel Audit"
1. **Renseignez les informations** : Nom, site, date, auditeur, responsable
2. **Choisissez le statut** : Brouillon, En cours, Terminé, Validé
3. **Parcourez les checkpoints** : 5 catégories dépliables
4. **Cochez les statuts** : Conforme/Non conforme/Partiel/N/A
5. **Cochez les preuves** : Cases à cocher pour chaque élément
6. **Ajoutez des commentaires** : Observations détaillées
7. **Notez les actions** : Recommandations de remédiation
8. **Sauvegardez** : Enregistrement dans l'historique

#### Page "Historique"
1. **Vue d'ensemble** : 5 cartes statistiques (Total, Brouillon, En cours, Terminé, Validé)
2. **Recherche** : Barre de recherche par nom/site/auditeur
3. **Filtres** : Par statut et critères de tri
4. **Actions** : Ouvrir, Supprimer chaque audit
5. **Export global** : Téléchargez tous vos audits en JSON
6. **Import** : Importez des audits depuis un fichier

#### Page "Comparaison"
1. **Sélectionnez 2 audits** : Via les menus déroulants
2. **Lancez la comparaison** : Bouton "Comparer"
3. **Visualisez les différences** : Statistiques + tableau détaillé
4. **Identifiez les changements** : Checkpoints différents en surbrillance

### Workflow recommandé

```
1. Préparation
   └─ Créer un nouvel audit (statut: Brouillon)
   └─ Renseigner les informations générales
   └─ Choisir la langue (FR/EN)

2. Audit sur site
   └─ Passer le statut en "En cours"
   └─ Parcourir les 27 points de contrôle
   └─ Cocher les preuves vérifiées
   └─ Ajouter observations et recommandations
   └─ Sauvegarder régulièrement

3. Analyse
   └─ Consulter le dashboard (progression globale)
   └─ Identifier les non-conformités
   └─ Comparer avec un audit précédent

4. Finalisation
   └─ Passer le statut en "Terminé"
   └─ Relecture et validation
   └─ Passer en "Validé"

5. Archivage
   └─ Export JSON individuel ou global
   └─ Sauvegarde externe
```

## 🛠️ Installation locale

### Option 1 : Utilisation directe
Ouvrez simplement `index.html` dans votre navigateur. Aucune installation requise !

### Option 2 : Serveur local
```bash
# Cloner le repository
git clone https://github.com/K3E9X/cyber-audit-dashboard.git

# Accéder au dossier
cd cyber-audit-dashboard

# Lancer un serveur local (Python 3)
python -m http.server 8000

# Ouvrir dans le navigateur
# http://localhost:8000
```

### Option 3 : Via GitHub Pages
L'application est déjà déployée et accessible directement en ligne !

## 💾 Format des données

### Export JSON d'un audit individuel
```json
{
  "id": 1,
  "name": "Audit Site Paris Q4 2024",
  "site": "Site de production Paris",
  "auditDate": "2025-10-28",
  "auditor": "Jean Dupont",
  "responsible": "Marie Martin",
  "status": "completed",
  "createdAt": "2025-10-28T10:00:00.000Z",
  "updatedAt": "2025-10-28T15:30:00.000Z",
  "stats": {
    "total": 27,
    "completed": 27,
    "conforme": 18,
    "nonConforme": 5,
    "partiel": 3,
    "na": 1,
    "percentage": 100
  },
  "checkpoints": {
    "GOU-01": {
      "status": "conforme",
      "comment": "Contrats à jour, CR de comité disponibles",
      "action": "",
      "evidenceChecked": [0, 1, 2]
    },
    "RES-01": {
      "status": "partiel",
      "comment": "Cartographie existante mais nécessite mise à jour",
      "action": "Planifier une mise à jour trimestrielle de la cartographie",
      "evidenceChecked": [0, 1]
    }
  }
}
```

### Export JSON de tous les audits
Le bouton "Exporter Tout (JSON)" dans l'historique génère un tableau JSON contenant tous vos audits sauvegardés.

## 🎨 Personnalisation

### Thèmes
- **Mode clair/sombre** : Bouton 🌙/☀️ en haut à droite
- **Préférence sauvegardée** : Le thème est mémorisé dans localStorage
- **Variables CSS** : Toutes les couleurs sont personnalisables via les variables CSS

### Langue
- **FR/EN** : Bouton 🇫🇷/🇬🇧 en haut à droite
- **Traduction complète** : Interface, checkpoints, messages
- **Préférence sauvegardée** : La langue est mémorisée dans localStorage

### Modification des checkpoints
Pour ajouter ou modifier des points de contrôle, éditez l'objet `checkpoints` et `checkpointsTranslations` dans le JavaScript :

```javascript
const checkpoints = {
    gouvernance: [
        {
            id: 'GOU-01',
            title: 'Votre titre',
            desc: 'Description',
            evidence: ['Preuve 1', 'Preuve 2']
        }
    ]
};

// N'oubliez pas d'ajouter la traduction
const checkpointsTranslations = {
    fr: { /* ... */ },
    en: { /* ... */ }
};
```

## 🤝 Contribution

Les contributions sont les bienvenues ! Voici comment contribuer :

1. **Fork** le projet
2. **Créez** une branche pour votre fonctionnalité (`git checkout -b feature/AmazingFeature`)
3. **Committez** vos changements (`git commit -m 'Add some AmazingFeature'`)
4. **Poussez** vers la branche (`git push origin feature/AmazingFeature`)
5. **Ouvrez** une Pull Request

## 🗺️ Roadmap

### Réalisé ✅
- [x] Sauvegarde automatique (LocalStorage)
- [x] Mode sombre/clair
- [x] Export JSON individuel
- [x] Système d'historique complet (IndexedDB)
- [x] Recherche et filtrage d'audits
- [x] Comparaison entre deux audits
- [x] Import/Export JSON de l'historique
- [x] Traduction FR/EN complète

### En cours de développement 🚧
- [ ] Export PDF avancé avec jsPDF
- [ ] Export Excel avec graphiques
- [ ] Génération automatique de rapports

### Futur 🔮
- [ ] Templates personnalisables par secteur
- [ ] Mode collaboratif multi-utilisateurs
- [ ] API REST pour intégration externe
- [ ] Application mobile native (React Native)
- [ ] Tableaux de bord analytics avancés
- [ ] Import depuis Excel/CSV
- [ ] Système de tags et catégories personnalisées

## 🐛 Bugs connus

Consultez les [Issues](https://github.com/K3E9X/cyber-audit-dashboard/issues) pour voir les bugs connus et les fonctionnalités en cours de développement.

## 📄 Licence

Ce projet est sous licence MIT. Voir le fichier [LICENSE](LICENSE) pour plus de détails.

## 🔗 Liens connexes

- **[Guide d'audit basique](https://github.com/K3E9X/audit-cybersecurity-industriel)** - Version imprimable simple
- **[Documentation complète](./docs/user-guide.md)** - Guide utilisateur détaillé
- **[Changelog](./CHANGELOG.md)** - Historique des versions

## 🏗️ Stack technique

- **Frontend** : HTML5, CSS3 (Variables CSS), JavaScript (ES6+)
- **Stockage** : IndexedDB (pour l'historique), LocalStorage (pour les préférences)
- **Graphiques** : Chart.js
- **Export** :
  - JSON natif
  - Excel : SheetJS (xlsx)
  - PDF : jsPDF + html2canvas (en développement)
- **Architecture** : Single Page Application (SPA)
- **Aucune dépendance backend** : 100% client-side

## 👨‍💻 Auteur

**K3E9X**
- GitHub: [@K3E9X](https://github.com/K3E9X)

## 🙏 Remerciements

- [Chart.js](https://www.chartjs.org/) pour les graphiques
- [SheetJS](https://sheetjs.com/) pour l'export Excel
- [jsPDF](https://github.com/parallax/jsPDF) pour l'export PDF
- La communauté open-source

---

⭐ **Si ce projet vous est utile, n'oubliez pas de lui donner une étoile !**

💬 **Des questions ?** Ouvrez une [Issue](https://github.com/K3E9X/cyber-audit-dashboard/issues/new)

🤖 **Développé avec [Claude Code](https://claude.com/claude-code)**
