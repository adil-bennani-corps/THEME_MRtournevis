# 🔧 Guide de Dépannage - Page 404

## 🎯 Problème

Vous voyez une page 404 dans l'éditeur de thème Shopify après avoir téléchargé le thème.

## ✅ Solution Immédiate

### Étape 1 : Accéder à la Homepage

1. Dans l'éditeur de thème Shopify (là où vous voyez la page 404)
2. Regardez le menu de **gauche**
3. Cliquez sur **"Pages"** ou **"Page d'accueil"** ou **"Home"**
4. Sélectionnez **"Accueil"** (ou la page principale)

➡️ **Cela devrait afficher la homepage au lieu de la 404**

---

### Étape 2 : Si la homepage ne se charge toujours pas

Si même la homepage affiche une erreur, il y a peut-être un problème avec les sections que nous avons créées.

**Solution temporaire :** Restaurer une homepage fonctionnelle

1. Dans l'éditeur de thème, sur la page d'accueil
2. Cliquez sur chaque section problématique
3. Cliquez sur les **"..."** (trois points) → **"Désactiver"** ou **"Supprimer"**
4. Utilisez les sections existantes du thème pour le moment

---

### Étape 3 : Créer les pages manquantes

La page 404 peut aussi apparaître si vous essayez d'accéder à des pages qui n'existent pas encore :

**Dans Shopify Admin** (pas dans l'éditeur) :
1. Allez dans **En ligne > Pages**
2. Créez une nouvelle page :
   - **Titre** : "Services"
   - **Modèle de page** : `page.services`
   - Cliquez sur **"Enregistrer"** puis **"Publier"**
3. Répétez pour "Rendez-vous" avec le modèle `page.appointment`

---

## 🔍 Vérifications Détaillées

### Vérifier que les sections sont disponibles

Dans l'éditeur de thème, sur la homepage :
1. Cliquez sur **"Ajouter une section"** ou regardez le menu des sections
2. Cherchez dans la liste :
   - "Homepage Hero Dual"
   - "Homepage Activities"
   - "Services Hero"
   - "Services Grid"
   - etc.

**Si ces sections n'apparaissent pas :**
- Il y a peut-être une erreur de syntaxe dans les fichiers `.liquid`
- Shopify ne peut pas charger ces sections
- Vous devrez peut-être re-télécharger le thème

### Vérifier les erreurs de console

1. Appuyez sur **F12** (outils de développement)
2. Ouvrez l'onglet **"Console"**
3. Regardez s'il y a des erreurs en rouge
4. Notez ces erreurs pour les corriger

---

## 🚨 Si rien ne fonctionne

### Option 1 : Utiliser l'ancienne homepage temporairement

Si vous avez une sauvegarde de l'ancien `index.json`, vous pouvez :
1. Re-télécharger le thème depuis Shopify
2. Modifier `index.json` pour utiliser les anciennes sections
3. Re-télécharger le thème modifié

### Option 2 : Désactiver les nouvelles sections

Dans l'éditeur de thème :
1. Sur la homepage, trouvez les sections "Homepage Hero Dual" et "Homepage Activities"
2. Cliquez dessus → **"..."** → **"Désactiver"**
3. Utilisez les sections existantes du thème (comme "Image Banner")

### Option 3 : Contacter le support

Si rien ne fonctionne, il se peut qu'il y ait une erreur dans les fichiers que nous avons créés. Dans ce cas, il faudra vérifier chaque fichier `.liquid` pour des erreurs de syntaxe.

---

## ✅ Checklist Rapide

- [ ] J'ai cliqué sur "Pages" → "Accueil" dans l'éditeur de thème
- [ ] La homepage se charge maintenant (ou affiche une autre erreur)
- [ ] Les sections "Homepage Hero Dual" apparaissent dans la liste des sections disponibles
- [ ] J'ai créé les pages "Services" et "Rendez-vous" dans Shopify Admin
- [ ] Je ne vois plus de page 404 sur la homepage

---

## 📞 Prochaines Étapes

Une fois que la homepage fonctionne :
1. ✅ Ajoutez les nouvelles sections une par une
2. ✅ Testez chaque section
3. ✅ Créez les pages Services et Rendez-vous
4. ✅ Configurez le menu

**Bon courage ! 🚀**

