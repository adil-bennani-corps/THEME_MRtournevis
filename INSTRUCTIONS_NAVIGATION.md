# Instructions pour configurer le menu de navigation

## 📋 Configuration du menu dans Shopify

Pour mettre en place la nouvelle structure de navigation, suivez ces étapes :

### 1. Accéder à la configuration des menus

1. Connectez-vous à votre admin Shopify
2. Allez dans **En ligne > Navigation**
3. Modifiez le menu principal (généralement nommé "Menu principal" ou "Main menu")

### 2. Structure du menu recommandée

Créez la structure suivante :

```
Accueil
├── / (lien vers la homepage)

Services de réparation
├── /pages/services (lien vers la page Services)

Boutique
├── iPhone
│   └── /collections/iphone
├── Samsung
│   └── /collections/samsung
├── Informatique
│   └── /collections/chargeurs (ou la collection appropriée)
├── Accessoires
│   └── /collections/accessoires
└── Tous les produits
    └── /collections/all

Rendez-vous
├── /pages/appointment

Contact
├── /pages/contact
```

### 3. Notes importantes

- Le lien **"Services de réparation"** sera automatiquement mis en avant visuellement grâce au CSS
- Assurez-vous que l'URL du lien Services pointe vers `/pages/services`
- Le lien "Rendez-vous" doit pointer vers `/pages/appointment`
- Le menu "Boutique" doit être configuré comme un menu déroulant avec les sous-catégories

### 4. Configuration dans le thème

Le fichier `header.liquid` utilise automatiquement le menu configuré dans **Réglages du thème > Navigation**. Assurez-vous que la section Header utilise le bon menu dans les paramètres.

### 5. Vérification

Après configuration :
- Vérifiez que tous les liens fonctionnent correctement
- Testez sur mobile (menu burger)
- Le lien "Services de réparation" devrait apparaître en rouge et légèrement souligné

---

**Note** : Si vous souhaitez ajouter un badge "Nouveau" sur le lien Services, vous pouvez utiliser le CSS fourni dans `custom-mrtournevis.css` (classe `.nav-highlight`).

