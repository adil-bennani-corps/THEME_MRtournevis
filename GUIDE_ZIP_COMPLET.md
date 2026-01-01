# 📦 Guide : Créer un ZIP Complet pour Shopify

## 🚨 Problème Identifié

Le thème sur Shopify ne contient que :
- `config/settings_schema.json`
- `layout/theme.liquid`

**Mais vous avez 375 fichiers localement !** Le ZIP n'a pas inclus tous les fichiers.

## ✅ Solution : Créer un ZIP Complet

### Méthode 1 : Windows Explorer (Recommandé)

1. **Ouvrez le dossier** `Theme_mrTournevis` dans l'Explorateur Windows
2. **Sélectionnez TOUT** :
   - Appuyez sur `Ctrl + A` (sélectionner tout)
   - OU cliquez-droit dans le dossier → "Sélectionner tout"
3. **Créez le ZIP** :
   - Clic-droit sur les fichiers sélectionnés
   - Choisissez "Envoyer vers" → "Dossier compressé (au format zip)"
   - OU "Compresser vers ZIP"
4. **Nommez le fichier** : `Theme_mrTournevis_COMPLET.zip`
5. **Vérifiez** : Le ZIP devrait faire plusieurs Mo (pas quelques Ko !)

### Méthode 2 : PowerShell (Alternative)

1. Ouvrez PowerShell dans le dossier parent
2. Exécutez :
```powershell
cd "C:\Users\benzr\Downloads"
Compress-Archive -Path "Theme_mrTournevis\*" -DestinationPath "Theme_mrTournevis_COMPLET.zip" -Force
```

## ⚠️ Points Importants

### ✅ À Faire
- ✅ Sélectionner TOUS les fichiers et dossiers
- ✅ Inclure les fichiers à la racine
- ✅ Inclure le dossier `layout/`
- ✅ Inclure le dossier `config/` (s'il existe)
- ✅ Inclure TOUS les fichiers .liquid
- ✅ Inclure TOUS les fichiers .json
- ✅ Inclure TOUS les fichiers .css, .js, .svg, etc.

### ❌ À Éviter
- ❌ Ne pas sélectionner seulement quelques fichiers
- ❌ Ne pas créer le ZIP depuis l'intérieur d'un sous-dossier
- ❌ Ne pas exclure les fichiers cachés (si vous en voyez)

## 📋 Vérification Avant Téléchargement

Avant de télécharger sur Shopify, vérifiez que le ZIP contient :

### Dossiers (si présents)
- [ ] `layout/` avec `theme.liquid`
- [ ] `config/` avec `settings_schema.json`

### Fichiers à la racine (beaucoup !)
- [ ] Beaucoup de fichiers `.liquid` (sections)
- [ ] Beaucoup de fichiers `.json` (templates)
- [ ] Beaucoup de fichiers `.css`, `.js`, `.svg`
- [ ] `settings_schema.json` (si pas dans config/)
- [ ] `settings_data.json`
- [ ] Etc.

**Le ZIP devrait contenir environ 375 fichiers !**

## 🚀 Après Création du ZIP

1. **Vérifiez la taille** : Le ZIP devrait faire plusieurs Mo (au moins 1-2 Mo minimum)
2. **Téléchargez sur Shopify** :
   - Allez dans Shopify Admin
   - Thèmes → Ajouter un thème → Télécharger un fichier
   - Sélectionnez votre ZIP
3. **Vérifiez après téléchargement** :
   - Le thème devrait avoir des centaines de fichiers
   - Pas seulement 2 fichiers !

## 🔍 Comment Vérifier le Contenu du ZIP

1. **Ouvrez le ZIP** (double-clic dans Windows)
2. **Comptez les fichiers** : Vous devriez voir beaucoup de fichiers
3. **Cherchez** :
   - Des fichiers `.liquid` (beaucoup !)
   - Des fichiers `.json` (beaucoup !)
   - Des fichiers `.css`, `.js`, etc.

---

**Une fois le ZIP complet créé et téléchargé, le thème devrait fonctionner ! 🎉**

