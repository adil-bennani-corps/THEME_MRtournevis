# 🛠️ Thème Shopify - Mr. Tournevis

Thème Shopify personnalisé pour Mr. Tournevis avec refonte complète mettant en avant les services de réparation et la boutique d'accessoires.

## 📋 Description

Ce thème a été créé pour mettre en avant les deux activités principales de Mr. Tournevis :
- ✅ **Services de réparation professionnelle** (smartphones, tablettes, PC, consoles)
- ✅ **Vente d'accessoires originaux**

## 🎯 Fonctionnalités

### Pages Créées
- **Homepage** : Nouveau hero avec 2 activités et section "Nos Activités"
- **Page Services** (`/pages/services`) : Page complète avec tous les services de réparation
- **Page Rendez-vous** (`/pages/appointment`) : Formulaire de prise de rendez-vous pour interventions à domicile

### Sections Personnalisées
- `homepage-hero-dual.liquid` - Hero homepage avec 2 CTAs
- `homepage-activities.liquid` - Section "Nos Activités"
- `services-hero.liquid` - Hero de la page Services
- `services-grid.liquid` - Grille des 4 services
- `services-testimonials.liquid` - Témoignages clients
- `services-locations.liquid` - Adresses des magasins
- `services-cta-appointment.liquid` - CTA rendez-vous
- `appointment-form.liquid` - Formulaire de rendez-vous

### Design System
- CSS custom complet (`custom-mrtournevis.css`)
- Palette de couleurs cohérente (rouge #DC2626)
- Typographie Inter (Google Fonts)
- Responsive design (mobile, tablette, desktop)

## 🚀 Installation

### Méthode 1 : Depuis GitHub (Recommandé)

1. **Téléchargez le thème** :
   ```bash
   git clone https://github.com/adil-bennani-corps/THEME_MRtournevis.git
   ```

2. **Créez un ZIP** du dossier téléchargé

3. **Téléchargez sur Shopify** :
   - Admin Shopify → Thèmes → Ajouter un thème → Télécharger un fichier
   - Sélectionnez le ZIP

### Méthode 2 : Via Shopify CLI

```bash
shopify theme push
```

## 📁 Structure du Thème

```
THEME_MRtournevis/
├── layout/
│   └── theme.liquid (layout principal)
├── sections/ (toutes les sections)
│   ├── services-hero.liquid
│   ├── homepage-hero-dual.liquid
│   └── ...
├── templates/ (tous les templates)
│   ├── index.json (homepage)
│   ├── page.services.json
│   ├── page.appointment.json
│   └── ...
├── assets/ (CSS, JS, images)
│   ├── custom-mrtournevis.css
│   └── ...
└── config/
    └── settings_schema.json
```

## ⚙️ Configuration

### 1. Créer les Pages dans Shopify Admin

1. **Page Services** :
   - En ligne > Pages → Nouvelle page
   - Titre : "Services"
   - Modèle : `page.services`
   - Publier

2. **Page Rendez-vous** :
   - Nouvelle page
   - Titre : "Rendez-vous"
   - Modèle : `page.appointment`
   - Publier

### 2. Configurer le Menu

Voir `INSTRUCTIONS_NAVIGATION.md` pour la configuration complète du menu.

Structure recommandée :
- Accueil
- Services de réparation → `/pages/services`
- Boutique (dropdown)
- Rendez-vous → `/pages/appointment`
- Contact

## 🎨 Personnalisation

Toutes les sections sont éditables depuis l'éditeur de thème Shopify :
- Textes et titres
- Images
- Couleurs
- Espacements

## 📝 Contraintes Respectées

- ✅ **Aucun prix** affiché pour les services de réparation
- ✅ RDV uniquement pour **interventions à domicile**
- ✅ Produits gardent leurs **prix affichés**
- ✅ Wording **"accessoires originaux"** (pas "premium")
- ✅ **Diagnostic gratuit** mis en avant

## 📚 Documentation

- `INSTRUCTIONS_NAVIGATION.md` - Guide pour configurer le menu
- `RECAP_MODIFICATIONS.md` - Récapitulatif des modifications
- `CHECKLIST_VALIDATION.md` - Checklist de validation complète
- `RESUME_FINAL.md` - Résumé final du projet

## 🔧 Développement

### Workflow Git

```bash
# Récupérer les dernières modifications
git pull origin main

# Ajouter vos modifications
git add .
git commit -m "Description des modifications"

# Envoyer vers GitHub
git push origin main
```

### Structure des Commits

Les commits doivent être descriptifs :
- `feat:` pour les nouvelles fonctionnalités
- `fix:` pour les corrections de bugs
- `style:` pour les modifications de style
- `docs:` pour la documentation

## 📞 Support

Pour toute question ou problème, référez-vous à la documentation dans le dossier ou créez une issue sur GitHub.

## 📄 Licence

Ce thème est propriétaire à Mr. Tournevis.

---

**Dernière mise à jour** : Janvier 2025

