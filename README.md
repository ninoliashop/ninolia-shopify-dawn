# 🎀 Ninolia Premium Theme - Shopify Dawn

## 📋 Vue d'ensemble

Ninolia est un thème Shopify Dawn entièrement personnalisé pour une boutique bébé premium, doux et minimaliste. Conçu pour convertir et rassurer les parents.

### 🎨 Palette de Couleurs

- **Crème** : `#F7F3EE` - Couleur primaire (fond)
- **Beige** : `#DCCCB8` - Couleur secondaire (accents)
- **Terracotta** : `#C98F75` - Accent (boutons, CTA)
- **Gris Foncé** : `#2D2D2D` - Texte principal
- **Gris Muted** : `#6F6A63` - Texte secondaire

## 📁 Structure des Fichiers

```
niniolia-shopify-dawn/
├── config/
│   └── settings_schema.json          # Configuration des couleurs et typographie
├── sections/
│   ├── hero.liquid                   # Hero avec titre, sous-titre, bouton, image
│   ├── trust-badge.liquid            # Bandeau de confiance (4 icônes)
│   ├── featured-collection.liquid    # Collection produits mise en avant
│   ├── benefits.liquid               # Pourquoi Ninolia (3 bénéfices)
│   ├── image-text.liquid             # Section image + texte
│   ├── testimonials.liquid           # Avis clients (3 témoignages)
│   ├── blog-section.liquid           # Blog conseils parents
│   ├── newsletter.liquid             # Newsletter
│   └── footer.liquid                 # Footer organisé
├── assets/
│   └── ninolia-theme.css             # Styles CSS personnalisés (variables CSS)
├── snippets/
│   └── color-palette.liquid          # Palette de couleurs réutilisable
└── README.md                         # Ce fichier
```

## 🚀 Fonctionnalités

### 1. **Hero Section** (`hero.liquid`)
- Titre et sous-titre personnalisables
- Bouton CTA avec lien configurable
- Image lifestyle responsive
- Gradient dégradé premium en arrière-plan

### 2. **Bandeau de Confiance** (`trust-badge.liquid`)
- 4 icônes éditables (✓, 🌿, 🚚, ❤️)
- Texte personnalisable pour chaque badge
- Responsive sur mobile (2 colonnes)

### 3. **Collection Produits** (`featured-collection.liquid`)
- Affichage des produits d'une collection Shopify
- Grille 4 colonnes (3 sur tablette, 2 sur mobile)
- Effet hover avec élévation
- Affichage du prix

### 4. **Bénéfices** (`benefits.liquid`)
- 3 sections avec icônes, titre et texte
- Fond beige tendre
- Effet hover subtle
- Entièrement personnalisable

### 5. **Image + Texte** (`image-text.liquid`)
- Disposition côte à côte sur desktop
- Image responsive
- Bouton CTA personnalisable
- Parfait pour la page "Notre Histoire"

### 6. **Avis Clients** (`testimonials.liquid`)
- 3 cartes de témoignages
- Étoiles 5/5
- Noms et titres des auteurs
- Animation hover

### 7. **Blog** (`blog-section.liquid`)
- Affichage des 3 derniers articles
- Image, catégorie, titre, extrait
- Lien "Lire la suite"
- Responsive 3 colonnes → 1 colonne mobile

### 8. **Newsletter** (`newsletter.liquid`)
- Gradient terracotta/beige attrayant
- Formulaire email épuré
- Bouton d'abonnement
- Responsive

### 9. **Footer** (`footer.liquid`)
- 4 colonnes (À propos, Boutique, Service client, Informations)
- Liens réseaux sociaux
- Bas de page avec copyrights
- Responsive 2 colonnes mobile

## 📱 Responsive Design

✅ **Desktop** : Optimisé pour écrans 1200px+  
✅ **Tablette** : Grilles adaptées 768px-1024px  
✅ **Mobile** : Grilles 1-2 colonnes, texte optimisé  

## 🎯 Optimisation Conversion

- ✅ CTA clairs et visibles (couleur terracotta)
- ✅ Trust badges pour rassurer
- ✅ Avis clients en évidence
- ✅ Newsletter stratégiquement placée
- ✅ Animations subtiles (pas d'excès)
- ✅ Textes rassurants et professionnels
- ✅ Hiérarchie visuelle claire

## 🛠️ Installation

1. **Cloner le repository**
   ```bash
   git clone https://github.com/ninoliashop/ninolia-shopify-dawn.git
   ```

2. **Configuration Shopify CLI** (optionnel)
   ```bash
   shopify theme pull
   ```

3. **Personnalisation**
   - Remplacer les images par vos photos
   - Adapter les textes à votre marque
   - Configurer les collections Shopify
   - Activer votre blog Shopify

4. **Publication**
   - Tester localement ou sur un thème de test
   - Publier sur Shopify

## 📊 Sections et Ordre Recommandé

1. **Hero** → Appel à l'action initial
2. **Trust Badges** → Rassurer immédiatement
3. **Featured Collection** → Produits phares
4. **Benefits** → Différenciation Ninolia
5. **Image + Texte** → Storytelling
6. **Testimonials** → Preuve sociale
7. **Blog** → Engagement et SEO
8. **Newsletter** → Lead generation
9. **Footer** → Navigation secondaire

## 🎨 Variables CSS Disponibles

Dans `assets/ninolia-theme.css` :

```css
--color-primary: #F7F3EE;    /* Crème */
--color-secondary: #DCCCB8;  /* Beige */
--color-accent: #C98F75;     /* Terracotta */
--color-dark: #2D2D2D;       /* Gris Foncé */
--color-muted: #6F6A63;      /* Gris Muted */
--spacing-xs: 0.5rem;        /* Petits espacements */
--spacing-sm: 1rem;
--spacing-md: 1.5rem;
--spacing-lg: 2rem;
--spacing-xl: 3rem;
--spacing-2xl: 4rem;
--border-radius: 12px;       /* Coins arrondis */
```

## 🔧 Personnalisation

### Modifier les couleurs :
1. Aller dans `config/settings_schema.json`
2. Modifier les valeurs hex des couleurs
3. Les variables CSS se mettront à jour automatiquement

### Ajouter/modifier les sections :
1. Éditer les fichiers `.liquid` dans `/sections`
2. Modifier les `settings` du `{% schema %}`
3. Les options apparaîtront dans l'éditeur Shopify

## 📞 Support

Pour toute question ou problème :
- Ouvrir une issue sur GitHub
- Contacter : support@ninolia.com

## 📄 Licence

Thème Ninolia © 2024. Tous droits réservés.

---

**Version** : 1.0.0  
**Dernière mise à jour** : Juin 2024  
**Compatibilité** : Shopify Dawn v5.0+
