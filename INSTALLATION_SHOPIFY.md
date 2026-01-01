# 📥 Guide d'Installation sur Shopify

## ❌ Problème

L'erreur **"La branche n'est pas un thème valide"** apparaît car Shopify ne peut **pas** installer un thème directement depuis GitHub.

## ✅ Solution : Télécharger depuis GitHub puis Uploader

### Méthode 1 : Télécharger le ZIP depuis GitHub (Recommandé)

1. **Allez sur GitHub** :
   - Ouvrez : https://github.com/adil-bennani-corps/THEME_MRtournevis
   - Cliquez sur le bouton vert **"Code"**
   - Sélectionnez **"Download ZIP"**
   - Le fichier `THEME_MRtournevis-main.zip` sera téléchargé

2. **Extrayez le ZIP** :
   - Double-cliquez sur le fichier ZIP
   - Extrayez le contenu dans un dossier (par exemple `THEME_MRtournevis-main`)

3. **Créez un nouveau ZIP du contenu** :
   - Ouvrez le dossier extrait `THEME_MRtournevis-main`
   - **Sélectionnez TOUS les fichiers** (Ctrl + A)
   - Clic-droit → "Envoyer vers" → "Dossier compressé (au format zip)"
   - Nommez-le : `THEME_MRtournevis_SHOPIFY.zip`

4. **Téléchargez sur Shopify** :
   - Allez dans Shopify Admin
   - **Thèmes** → **Ajouter un thème** → **Télécharger un fichier**
   - Sélectionnez votre fichier ZIP
   - Le thème sera installé !

### Méthode 2 : Utiliser Shopify CLI (Avancé)

Si vous avez Shopify CLI installé :

```bash
# 1. Cloner le dépôt
git clone https://github.com/adil-bennani-corps/THEME_MRtournevis.git
cd THEME_MRtournevis

# 2. Se connecter à Shopify
shopify theme dev

# 3. Ou push directement
shopify theme push
```

## ⚠️ Points Importants

- ❌ Shopify **ne peut pas** se connecter directement à GitHub
- ✅ Il faut **télécharger le ZIP** et l'uploader manuellement
- ✅ Assurez-vous que le ZIP contient **tous les fichiers** (pas juste le dossier parent)

## 🔍 Vérification

Après installation, vérifiez que le thème contient :
- `layout/theme.liquid`
- Beaucoup de fichiers `.liquid` (sections)
- Beaucoup de fichiers `.json` (templates)
- Le dossier `config/`

Si vous ne voyez que 2-3 fichiers, le ZIP n'a pas été créé correctement.

---

**La méthode GitHub → Download ZIP → Upload sur Shopify est la plus simple ! 🚀**

