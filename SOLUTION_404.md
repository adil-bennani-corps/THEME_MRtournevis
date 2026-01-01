# 🔧 Solution pour la page 404

## 🔍 Diagnostic

Vous voyez une page 404 dans l'éditeur de thème Shopify. Voici les causes possibles et solutions :

## ✅ Solutions à essayer

### 1. Vérifier que vous êtes sur la bonne page

Dans l'éditeur de thème Shopify :
- **Cliquez sur "Accueil"** dans le menu de gauche pour voir la homepage
- La page 404 apparaît si vous essayez d'accéder à une page qui n'existe pas encore (comme `/pages/services`)

### 2. Les pages doivent être créées dans Shopify Admin

Les templates que nous avons créés (`page.services.json`, `page.appointment.json`) sont des **modèles de pages**, mais les **pages elles-mêmes** doivent être créées dans Shopify Admin :

1. Allez dans **En ligne > Pages** (dans Shopify Admin, pas dans l'éditeur de thème)
2. Créez une nouvelle page :
   - **Titre** : "Services"
   - **Modèle** : `page.services`
   - **Publiez** la page
3. Répétez pour "Rendez-vous" avec le modèle `page.appointment`

### 3. Vérifier la homepage

Pour voir la homepage dans l'éditeur :
1. Dans l'éditeur de thème, cliquez sur **"Pages"** dans le menu de gauche
2. Sélectionnez **"Accueil"** (ou "Home")
3. Vous devriez voir la page d'accueil avec les nouvelles sections

### 4. Si la homepage ne se charge pas

Si même la homepage affiche une erreur, il peut y avoir un problème avec les sections. Vérifiez :

1. **Dans l'éditeur de thème** :
   - Allez sur la page d'accueil
   - Cliquez sur **"Ajouter une section"** ou **"Sections"**
   - Vérifiez si vous voyez "Homepage Hero Dual" et "Homepage Activities" dans la liste
   - Si elles n'apparaissent pas, il y a peut-être une erreur dans les fichiers

2. **Vérifier les erreurs dans la console** :
   - Appuyez sur F12 pour ouvrir les outils de développement
   - Regardez l'onglet "Console" pour voir s'il y a des erreurs JavaScript

## 🔄 Solution rapide : Utiliser l'ancienne homepage temporairement

Si vous voulez que le site fonctionne immédiatement, vous pouvez temporairement restaurer l'ancien `index.json` :

1. Dans l'éditeur de thème Shopify
2. Allez sur la homepage
3. Vous pouvez désactiver les nouvelles sections et utiliser les anciennes sections

## ✅ Vérification étape par étape

1. **Vérifiez que vous êtes sur la homepage** :
   - Dans l'éditeur, menu gauche → Pages → Accueil

2. **Vérifiez que les sections sont disponibles** :
   - Menu gauche → Sections (ou "Ajouter une section")
   - Cherchez "Homepage Hero Dual" et "Homepage Activities"

3. **Si les sections n'apparaissent pas** :
   - Il y a peut-être une erreur de syntaxe dans les fichiers .liquid
   - Vérifiez les logs dans Shopify (si disponibles)

4. **Créez les pages manquantes** :
   - Les pages "/pages/services" et "/pages/appointment" n'existent pas encore
   - Vous devez les créer dans Shopify Admin → Pages

## 📝 Résumé

La page 404 est **normale** si :
- ✅ Vous essayez d'accéder à `/pages/services` avant de créer la page
- ✅ Vous essayez d'accéder à `/pages/appointment` avant de créer la page

**Action immédiate** :
1. Dans l'éditeur de thème, cliquez sur **"Pages"** → **"Accueil"** pour voir la homepage
2. Créez les pages manquantes dans Shopify Admin → Pages

