# ✅ Vérification des Prérequis pour Shopify CLI

## 📋 Prérequis Nécessaires

Pour utiliser Shopify CLI, vous avez besoin de :

1. **Node.js** : version 20.10 ou supérieure
2. **Gestionnaire de paquets Node.js** : npm, Yarn 1.x, ou pnpm
3. **Git** : version 2.28.0 ou supérieure

---

## 🔍 Vérification Automatique

Les commandes ci-dessous vérifient l'installation de chaque outil.

### Node.js
```bash
node --version
```

### npm (gestionnaire de paquets Node.js)
```bash
npm --version
```

### Git
```bash
git --version
```

### Shopify CLI (si déjà installé)
```bash
shopify version
```

---

## 📥 Installation si Manquant

### Installer Shopify CLI

Si Shopify CLI n'est pas installé :

```bash
npm install -g @shopify/cli @shopify/theme
```

Ou avec yarn :
```bash
yarn global add @shopify/cli @shopify/theme
```

Ou avec pnpm :
```bash
pnpm add -g @shopify/cli @shopify/theme
```

---

## ✅ Résultat Attendu

Si tout est installé correctement, vous devriez voir :
- ✅ Node.js : `v20.10.0` ou supérieur
- ✅ npm : `10.x.x` ou supérieur (ou Yarn/pnpm)
- ✅ Git : `2.28.0` ou supérieur
- ✅ Shopify CLI : `3.x.x` ou supérieur (si installé)

---

## 🚀 Utilisation de Shopify CLI

Une fois tout installé, vous pouvez :

```bash
# Se connecter à votre boutique Shopify
shopify theme dev

# Ou pousser le thème directement
shopify theme push
```

---

**Note** : Si vous préférez, vous pouvez toujours utiliser la méthode ZIP manuelle (voir `METHODE_SIMPLE_INSTALLATION.md`).

