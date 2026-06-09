# Guide d'Installation Ninolia Theme

## 📦 Prérequis

- Shopify Store actif
- Thème Shopify Dawn (gratuit)
- Accès admin Shopify
- Collections produits créées
- Blog créé (pour section blog)

## 🚀 Installation Étape par Étape

### Étape 1: Clone le Repository

```bash
cd votre-dossier-shopify
git clone https://github.com/ninoliashop/ninolia-shopify-dawn.git
```

### Étape 2: Configuration Shopify CLI (Optionnel mais Recommandé)

```bash
# Installer Shopify CLI
brew install shopify-cli

# Se connecter
shopify login --store ninolia.myshopify.com

# Synchroniser le thème
shopify theme push --development
```

### Étape 3: Intégration Manuelle dans Shopify

Si vous préférez ne pas utiliser CLI :

1. Aller à **Ventes en Ligne > Thèmes**
2. Cliquer **"Ajouter un thème"** → **"Importer de ZIP"**
3. Télécharger le repository en ZIP
4. Sélectionner et importer
5. Personnaliser dans l'éditeur de thème

## 🎨 Personnalisation

### 1. Importer Images

- Hero image (1920x1080px recommandé)
- Image section "Image + Texte"
- Images produits dans collections
- Avatar auteur testimonials

### 2. Configurer Collections

Dans `sections/featured-collection.liquid` :
1. Sélectionner collection à afficher
2. Configurer nombre produits
3. Tester responsive

### 3. Activer Blog

Dans `sections/blog-section.liquid` :
1. Créer blog dans Shopify (Articles)
2. Ajouter 3+ articles avec images
3. Sélectionner blog dans éditeur

### 4. Personnaliser Textes

- Héros: titre, sous-titre
- Trust badges: icônes (emoji ou HTML)
- Bénéfices: titres et descriptions
- FAQ: questions/réponses
- Footer: infos entreprise

### 5. Tester Tous les Appareils

✅ Desktop (1920px+)  
✅ Tablet (768px-1024px)  
✅ Mobile (320px-480px)  

## 🔧 Fichiers Importants à Modifier

### `config/settings_schema.json`
Couleurs principales de la boutique

### `assets/ninolia-theme.css`
Styles CSS globaux

### `sections/*.liquid`
Contenu des sections

### `snippets/color-palette.liquid`
Palette réutilisable

## 📱 Optimisation Mobile

- Tous les grilles adaptées (4 col → 3 → 2 → 1)
- Textes redimensionnés automatiquement
- Boutons fullwidth sur mobile
- Espacements réduits

## 🔍 SEO Checklist

- [ ] Meta titles optimisés
- [ ] Meta descriptions < 160 car
- [ ] Alt text sur images
- [ ] Headings hiérarchisés (H1-H3)
- [ ] URLs courtes et descriptives
- [ ] Sitemap généré
- [ ] Schema markup ajouter (optional)

## 💳 Configuration Paiement

1. Aller à **Paramètres > Paiements**
2. Configurer Stripe/PayPal
3. Définir devise (€ EUR)
4. Tester paiement

## 📊 Analytics & Conversion

### Google Analytics
```html
<!-- Ajouter dans theme.liquid HEAD -->
<!-- Google Analytics 4 -->
```

### Google Tag Manager
```
<!-- Ajouter GTM container -->
```

## 🚀 Checklist Avant Lancement

- [ ] Toutes images hautes résolution
- [ ] Liens internes actifs
- [ ] Formulaire newsletter testé
- [ ] Métadonnées complètes
- [ ] Favicon ajouté
- [ ] Logo téléchargé
- [ ] Téléphone/email mis à jour
- [ ] Politique de confidentialité créée
- [ ] Conditions générales créées
- [ ] Robots.txt optimisé
- [ ] SSL/HTTPS actif
- [ ] Mobile test réussi

## 🆘 Troubleshooting

### Sections ne s'affichent pas
- Vérifier que les fichiers `.liquid` sont dans `/sections`
- Rafraîchir l'éditeur de thème
- Vérifier console pour erreurs

### Couleurs ne s'appliquent pas
- Vérifier `settings_schema.json`
- Vérifier CSS en cascade
- Vider cache navigateur

### Images ne se chargent pas
- Vérifier chemins `{{ image_url }}`
- Vérifier permissions fichiers
- Tester sur autre navigateur

### Mobile ne s'affiche pas bien
- Vérifier media queries dans CSS
- Utiliser Chrome DevTools
- Tester sur vraie appareil

## 📞 Support

Pour questions :
- Email: support@ninolia.com
- GitHub Issues: [repo]
- Documentation: README.md

## 📚 Ressources Utiles

- [Shopify Theme Development](https://shopify.dev/themes)
- [Liquid Documentation](https://shopify.dev/api/liquid)
- [Shopify CLI Reference](https://shopify.dev/cli)
- [Accessibility Guidelines](https://www.shopify.com/partners/blog/web-accessibility)

## 🔄 Mise à Jour Future

Pour mettre à jour le thème :

```bash
git pull origin main
shopify theme push
```

---

**Version**: 1.0.0  
**Dernière mise à jour**: Juin 2024  
**Support**: Ninolia Team
