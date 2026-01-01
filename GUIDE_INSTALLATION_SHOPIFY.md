# 📥 Guide d'Installation du Thème sur Shopify

## ⚠️ Important : GitHub ne peut pas être utilisé directement

Shopify **ne peut pas importer un thème directement depuis GitHub**. Vous avez plusieurs options :

---

## 🎯 Option 1 : Télécharger depuis GitHub et créer un ZIP (Recommandé)

### Étape 1 : Télécharger depuis GitHub

1. Allez sur : https://github.com/adil-bennani-corps/THEME_MRtournevis
2. Cliquez sur le bouton vert **"Code"**
3. Sélectionnez **"Download ZIP"**
4. Enregistrez le fichier ZIP sur votre ordinateur

### Étape 2 : Extraire et préparer

1. **Extrayez le ZIP** dans un dossier (ex: `THEME_MRtournevis-main`)
2. **Vérifiez la structure** : Le dossier doit contenir tous les fichiers (layout/, fichiers .liquid, .json, etc.)
3. **Important** : Assurez-vous que le dossier `layout/` contient `theme.liquid`

### Étape 3 : Créer un nouveau ZIP (sans le dossier parent)

**⚠️ CRITIQUE** : Ne pas créer le ZIP du dossier parent, mais du contenu !

1. **Ouvrez le dossier** `THEME_MRtournevis-main` (ou le nom du dossier extrait)
2. **Sélectionnez TOUS les fichiers** à l'intérieur (Ctrl+A)
   - Vous devez voir : `layout/`, `config/`, tous les fichiers .liquid, .json, etc.
   - **PAS** le dossier parent lui-même
3. **Clic-droit** → "Envoyer vers" → "Dossier compressé (ZIP)"
4. Nommez-le : `Theme_mrTournevis.zip`

### Étape 4 : Télécharger sur Shopify

1. Connectez-vous à votre **Shopify Admin**
2. Allez dans **En ligne > Thèmes**
3. Cliquez sur **"Ajouter un thème"** → **"Télécharger un fichier"**
4. Sélectionnez votre fichier ZIP
5. Attendez que le thème soit installé

---

## 🎯 Option 2 : Utiliser Shopify CLI (Pour développeurs)

Si vous avez Shopify CLI installé :

```bash
# 1. Cloner le dépôt (si pas déjà fait)
git clone https://github.com/adil-bennani-corps/THEME_MRtournevis.git
cd THEME_MRtournevis

# 2. Se connecter à Shopify
shopify theme dev

# Ou pour pousser le thème
shopify theme push
```

**Note** : Shopify CLI nécessite une configuration préalable.

---

## 🎯 Option 3 : Cloner Git localement et créer un ZIP

Si vous avez Git installé localement :

```bash
# 1. Cloner le dépôt
git clone https://github.com/adil-bennani-corps/THEME_MRtournevis.git
cd THEME_MRtournevis

# 2. Créer un ZIP (Windows PowerShell)
Compress-Archive -Path * -DestinationPath ../Theme_mrTournevis.zip -Force

# 3. Télécharger le ZIP sur Shopify (voir Option 1, Étape 4)
```

---

## ✅ Vérification Après Installation

Une fois le thème installé sur Shopify, vérifiez :

1. **Dans l'éditeur de thème** :
   - Allez sur la **homepage**
   - Vérifiez que les sections se chargent
   - Vérifiez qu'il n'y a plus d'erreur 404

2. **Structure du thème** :
   - Le thème doit contenir **des centaines de fichiers** (pas seulement 2-3)
   - Vérifiez la présence des dossiers : `layout/`, `sections/`, `templates/`, `assets/`

---

## 🚨 Problèmes Courants

### Erreur "La branche n'est pas un thème valide"

Cette erreur apparaît si vous essayez d'importer directement depuis GitHub. **Solution** : Utilisez l'Option 1 (télécharger ZIP depuis GitHub).

### Le thème ne contient que 2-3 fichiers après installation

**Cause** : Le ZIP a été créé incorrectement (dossier parent au lieu du contenu).  
**Solution** : Vérifiez l'Étape 3 de l'Option 1 - vous devez créer le ZIP du **contenu** du dossier, pas du dossier lui-même.

### Page 404 après installation

**Cause** : Le thème est incomplet ou `index.json` référence des sections qui n'existent pas.  
**Solution** : 
- Vérifiez que tous les fichiers sont présents dans le ZIP
- Vérifiez que `layout/theme.liquid` existe
- Vérifiez que les sections référencées existent

---

## 📋 Checklist d'Installation

- [ ] J'ai téléchargé le ZIP depuis GitHub
- [ ] J'ai extrait le ZIP
- [ ] J'ai créé un nouveau ZIP avec le **contenu** du dossier (pas le dossier parent)
- [ ] Le ZIP contient `layout/theme.liquid`
- [ ] Le ZIP contient des centaines de fichiers
- [ ] J'ai téléchargé le ZIP sur Shopify
- [ ] Le thème s'est installé sans erreur
- [ ] La homepage se charge correctement

---

## 💡 Astuce

**Pour éviter les problèmes** :
- Toujours créer le ZIP du **contenu** du dossier (tous les fichiers à la racine)
- Vérifier que `layout/theme.liquid` est présent
- Vérifier la taille du ZIP (devrait être de plusieurs Mo)

---

**Bonne installation ! 🚀**

