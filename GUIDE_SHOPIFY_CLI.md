# 🚀 Guide Shopify CLI - Installation et Utilisation

## ✅ État des Prérequis

Tous les prérequis sont installés :

- ✅ **Node.js** : v24.12.0 (requis : 20.10+) 
- ✅ **npm** : 11.6.2
- ✅ **Git** : 2.52.0 (requis : 2.28.0+)
- ✅ **Shopify CLI** : Installé via npm

---

## 📋 Résumé de l'Installation

Shopify CLI a été installé avec la commande :
```bash
npm install -g @shopify/cli @shopify/theme
```

**Note** : Le package `@shopify/theme` est maintenant déprécié car il est inclus dans `@shopify/cli` depuis la version 3.59.0. C'est normal de voir cet avertissement.

---

## 🎯 Utilisation de Shopify CLI

### Option 1 : Développement Local (Recommandé)

Pour développer et voir les changements en temps réel :

```bash
# Dans le dossier du thème
cd C:\Users\benzr\Downloads\Theme_mrTournevis

# Lancer le serveur de développement
shopify theme dev
```

Cette commande va :
1. Vous demander de vous connecter à votre boutique Shopify
2. Créer un thème de développement
3. Synchroniser les fichiers en temps réel
4. Ouvrir un aperçu dans votre navigateur

### Option 2 : Push Direct du Thème

Pour uploader le thème directement :

```bash
# Dans le dossier du thème
cd C:\Users\benzr\Downloads\Theme_mrTournevis

# Pousser le thème
shopify theme push
```

Cette commande va :
1. Vous demander de vous connecter à votre boutique
2. Vous demander quel thème modifier (ou créer un nouveau)
3. Uploader tous les fichiers

### Option 3 : Pull (Télécharger depuis Shopify)

Pour télécharger un thème depuis Shopify :

```bash
shopify theme pull
```

---

## 🔐 Première Connexion

La première fois que vous utilisez Shopify CLI :

1. **Exécutez une commande** (ex: `shopify theme dev`)
2. **Shopify CLI va ouvrir votre navigateur**
3. **Connectez-vous** à votre compte Shopify
4. **Autorisez** Shopify CLI à accéder à votre boutique
5. **Sélectionnez votre boutique** si vous en avez plusieurs

---

## 📝 Commandes Utiles

### Voir l'aide
```bash
shopify theme --help
```

### Lister les thèmes
```bash
shopify theme list
```

### Ouvrir l'éditeur de thème
```bash
shopify theme open
```

### Vérifier les fichiers
```bash
shopify theme check
```

---

## ⚠️ Notes Importantes

1. **Git** : Shopify CLI utilise Git pour suivre les changements. Assurez-vous que votre dépôt est à jour :
   ```bash
   git pull origin main
   ```

2. **Fichiers à ne pas uploader** : Shopify CLI respecte `.gitignore`. Les fichiers temporaires ne seront pas uploadés.

3. **Thème de développement** : `shopify theme dev` crée automatiquement un thème de développement séparé de votre thème live. C'est parfait pour tester !

4. **Synchronisation** : Les changements sont synchronisés en temps réel. Sauvegardez vos fichiers et ils apparaîtront sur Shopify.

---

## 🆚 Comparaison avec la Méthode ZIP

| Méthode | Avantages | Inconvénients |
|---------|-----------|---------------|
| **Shopify CLI** | - Synchronisation temps réel<br>- Développement local<br>- Pas besoin de ZIP | - Nécessite installation<br>- Nécessite connexion |
| **ZIP Manuel** | - Simple<br>- Pas d'installation requise | - Pas de synchronisation<br>- Doit recréer le ZIP à chaque fois |

**Recommandation** : Utilisez Shopify CLI pour le développement, et le ZIP pour des installations ponctuelles.

---

## 🚀 Prochaines Étapes

1. **Testez Shopify CLI** :
   ```bash
   cd C:\Users\benzr\Downloads\Theme_mrTournevis
   shopify theme dev
   ```

2. **Ou push directement** :
   ```bash
   shopify theme push
   ```

3. **Commitez vos changements sur GitHub** après chaque modification importante :
   ```bash
   git add .
   git commit -m "Description des modifications"
   git push origin main
   ```

---

**Shopify CLI est maintenant prêt à être utilisé ! 🎉**

