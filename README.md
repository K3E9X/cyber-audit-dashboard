# cyber-audit-dashboard
Application web interactive pour audits de cybersécurité industriels
# Cyber Audit Dashboard

> Application web interactive pour réaliser des audits de cybersécurité sur sites industriels

[![License: MIT](https://img.shields.io/badge/License-MIT-blue.svg)](https://opensource.org/licenses/MIT)
[![GitHub stars](https://img.shields.io/github/stars/K3E9X/cyber-audit-dashboard?style=social)](https://github.com/K3E9X/cyber-audit-dashboard)
[![GitHub forks](https://img.shields.io/github/forks/K3E9X/cyber-audit-dashboard?style=social)](https://github.com/K3E9X/cyber-audit-dashboard/fork)

## Démo en ligne

**[Lancer l'application](https://k3e9x.github.io/cyber-audit-dashboard/)**


## Fonctionnalités

### Dashboard interactif
- **Statistiques en temps réel** : Visualisation instantanée de l'état d'avancement
- **Graphiques dynamiques** : Répartition des conformités avec Chart.js
- **Barre de progression** : Suivi visuel du pourcentage de complétion

### Sauvegarde intelligente
- **Auto-save** : Sauvegarde automatique toutes les 30 secondes
- **LocalStorage** : Aucune perte de données, même en fermant le navigateur
- **Export JSON** : Sauvegarde et partage de vos audits

### Recherche & Filtrage
- **Recherche instantanée** : Trouvez rapidement un point de contrôle
- **Filtres par statut** : Conformes, Non conformes, Partiels, Non vérifiés
- **Navigation intelligente** : Sidebar avec progression par catégorie

### Interface moderne
- **Mode sombre/clair** : Confort visuel adapté à votre environnement
- **Responsive design** : Fonctionne sur desktop, tablette et mobile
- **Animations fluides** : Expérience utilisateur soignée

### Optimisé pour le terrain
- **Utilisation hors-ligne** : Fonctionne sans connexion internet
- **Impression optimisée** : Format A4 prêt pour l'impression
- **Commentaires détaillés** : Zone de texte pour chaque point de contrôle

## Points de contrôle couverts

L'application couvre **27 points de contrôle** répartis en **5 catégories** :

| Catégorie | Points | Description |
|-----------|--------|-------------|
| **Gouvernance** | 1 | Gestion des risques et pilotage |
| **Ressources** | 9 | Cartographie, réseau, infrastructure |
| **Contrôle d'accès** | 9 | Gestion des comptes et authentification |
| **Actifs** | 6 | Sécurité des systèmes et postes |
| **Physique** | 2 | Contrôles d'accès physiques |

## Utilisation

### Démarrage rapide

1. **Ouvrez l'application** dans votre navigateur
2. **Remplissez les informations** de l'audit (site, date, auditeur)
3. **Parcourez les checkpoints** et cochez les statuts
4. **Ajoutez des commentaires** pour chaque point
5. **Sauvegardez** ou **exportez** votre audit

### Workflow recommandé

```
1. Préparation
   └─ Renseignez les informations générales

2. Audit sur site
   └─ Parcourez les 27 points de contrôle
   └─ Cochez les statuts (Conforme/Non conforme/Partiel)
   └─ Ajoutez vos observations

3. Analyse
   └─ Consultez le dashboard pour avoir une vue d'ensemble
   └─ Utilisez les filtres pour identifier les non-conformités

4. Export
   └─ Sauvegardez en JSON pour archivage
   └─ Imprimez pour signature et classement
```

## Installation locale

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


## Format des données

### Export JSON
```json
{
  "site": "Site de production Paris",
  "auditDate": "2025-10-10",
  "auditor": "Jean Dupont",
  "responsible": "Marie Martin",
  "checkpoints": {
    "GOU-01": {
      "status": "conforme",
      "comment": "Contrats à jour, CR de comité disponibles"
    },
    "RES-01": {
      "status": "partiel",
      "comment": "Cartographie existante mais nécessite mise à jour"
    }
  }
}
```

## Personnalisation

### Thèmes
L'application supporte automatiquement les modes clair et sombre. Le thème choisi est sauvegardé dans le localStorage.

### Modification des checkpoints
Pour ajouter ou modifier des points de contrôle, éditez l'objet `checkpoints` dans le JavaScript :

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
```

## Contribution

Les contributions sont les bienvenues ! Voici comment contribuer :

1. **Fork** le projet
2. **Créez** une branche pour votre fonctionnalité (`git checkout -b feature/AmazingFeature`)
3. **Committez** vos changements (`git commit -m 'Add some AmazingFeature'`)
4. **Poussez** vers la branche (`git push origin feature/AmazingFeature`)
5. **Ouvrez** une Pull Request

## Roadmap

- [ ] Import de fichiers JSON
- [ ] Export PDF avancé avec jsPDF
- [ ] Comparaison entre deux audits
- [ ] Templates personnalisables
- [ ] Mode collaboratif multi-utilisateurs
- [ ] API REST pour intégration externe
- [ ] Application mobile native
- [ ] Génération automatique de rapports

## Bugs connus

Consultez les [Issues](https://github.com/K3E9X/cyber-audit-dashboard/issues) pour voir les bugs connus et les fonctionnalités en cours de développement.

## Licence

Ce projet est sous licence MIT. Voir le fichier [LICENSE](LICENSE) pour plus de détails.

## 🔗 Liens connexes

- **[Guide d'audit basique](https://github.com/K3E9X/audit-cybersecurity-industriel)** - Version imprimable simple
- **[Documentation complète](./docs/user-guide.md)** - Guide utilisateur détaillé
- **[Changelog](./CHANGELOG.md)** - Historique des versions

## Auteur

**K3E9X**
- GitHub: [@K3E9X](https://github.com/K3E9X)

## Remerciements

- [Chart.js](https://www.chartjs.org/) pour les graphiques
- La communauté open-source

---

⭐ **Si ce projet vous est utile, n'oubliez pas de lui donner une étoile !**

💬 **Des questions ?** Ouvrez une [Issue](https://github.com/K3E9X/cyber-audit-dashboard/issues/new)
