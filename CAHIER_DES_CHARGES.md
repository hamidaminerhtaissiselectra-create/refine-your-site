# 📋 CAHIER DES CHARGES COMPLET — Répar'Action Volets

**Dernière mise à jour** : 6 mars 2026  
**Version** : 4.0  
**Statut** : ✅ Production

---

## 1. IDENTITÉ & INFORMATIONS ENTREPRISE

| Champ | Valeur |
|-------|--------|
| **Nom** | Répar'Action Volets |
| **Adresse** | 62 Rue Emile Zola, 77610 Fontenay-Trésigny, FRANCE |
| **Téléphone** | 06 03 20 59 67 |
| **Email** | contact@reparaction-volets.fr |
| **Site** | https://reparaction-volets.fr |
| **Fondation** | 2014 |
| **Certifications** | RGE, Qualibat |

---

## 2. OBJECTIF STRATÉGIQUE

Créer un site web ultra-professionnel optimisé **SEO**, **GEO** (Generative Engine Optimization), **IA (SGE)** pour atteindre le **Top 3** sur toutes les recherches liées à la réparation de volets roulants et vitrerie en France.

### Règles impératives
- ❌ **Pas de mention "local"** : couverture nationale, Paris en priorité
- ❌ **Pas de chatbot** : formulaire de devis intelligent multi-étapes uniquement
- ✅ **Couverture nationale** affichée, Paris/IDF prioritaire pour les redirections actives

---

## 3. TECHNOLOGIES

| Composant | Technologie |
|-----------|-------------|
| Frontend | React 18, TypeScript, Tailwind CSS |
| Animations | Framer Motion |
| Routing | React Router DOM v6 |
| Build | Vite |
| UI Components | shadcn/ui |
| Backend (prévu) | Supabase (formulaires, auth) |

---

## 4. ARCHITECTURE DU SITE

### 4.1 Pages principales
| Route | Page | Statut |
|-------|------|--------|
| `/` | Page d'accueil | ✅ |
| `/qui-sommes-nous` | Qui sommes-nous | ✅ |
| `/blog` | Blog SEO (18 articles) | ✅ |
| `/blog/:slug` | Article de blog | ✅ |
| `/zones-intervention` | Zones d'intervention | ✅ |
| `/zones-intervention/paris` | Page région Paris | ✅ |
| `/zones-intervention/ile-de-france` | Page région IDF | ✅ |
| `/mentions-legales` | Mentions légales | ✅ |
| `/politique-confidentialite` | Politique de confidentialité | ✅ |
| `/cgv` | CGV | ✅ |

### 4.2 Pages services (5 pages, 1500+ mots)
| Route | Service | Statut |
|-------|---------|--------|
| `/services/reparation-volets-roulants` | Réparation Volets Roulants | ✅ |
| `/services/installation-remplacement-volets` | Installation & Remplacement | ✅ |
| `/services/vitrerie-remplacement-vitrage` | Vitrerie & Remplacement Vitrage | ✅ |
| `/services/motorisation-domotique` | Motorisation & Domotique | ✅ |
| `/services/depannage-express` | Dépannage Express | ✅ |

### 4.3 Pages zones localisées (53 pages SEO)

**Paris — 20 arrondissements** : `/zones-intervention/reparation-volet-paris-[1-20]`

**Île-de-France — 33 villes** :
- **Hauts-de-Seine (92)** : Boulogne-Billancourt, Neuilly, Levallois-Perret, Courbevoie, Puteaux, La Défense, Sèvres, Saint-Cloud, Rueil-Malmaison
- **Seine-Saint-Denis (93)** : Saint-Denis, Montreuil, Bobigny, Pantin, Bagnolet, Noisy-le-Sec, Aubervilliers, Saint-Ouen
- **Val-de-Marne (94)** : Créteil, Vitry-sur-Seine, Ivry-sur-Seine, Villejuif, Fontenay-sous-Bois, Vincennes, Saint-Mandé
- **Yvelines (78)** : Versailles, Saint-Germain-en-Laye, Rambouillet, Mantes-la-Jolie
- **Essonne (91)** : Évry-Courcouronnes, Corbeil-Essonnes
- **Seine-et-Marne (77)** : Melun
- **Val-d'Oise (95)** : Cergy, Pontoise

Chaque page contient :
- H1 et métadonnées uniques
- Infos locales (population, repères, caractère)
- 6 services spécialisés
- 3 témoignages clients
- 8 questions fréquentes
- Maillage vers villes limitrophes
- Image locale unique
- Schema.org LocalBusiness + FAQPage

---

## 5. SECTIONS PAGE D'ACCUEIL (ordre)

1. **Navbar** — Navigation sticky avec liens + CTA
2. **HeroSection** — Parallaxe, CTA principal, badges confiance
3. **ServicesSection** — 5 cartes services avec images et badges colorés
4. **QuoteFormSection** — Formulaire de devis multi-étapes
5. **AboutSection** — Présentation entreprise, chiffres clés
6. **ProcessSection** — 4 étapes (timeline visuelle)
7. **ImageTextSection** — Section image + texte expertise
8. **TestimonialsSection** — Avis clients
9. **ServiceRegionsSection** — Toutes les régions de France (dépliable, redirections actives uniquement pour Paris/IDF)
10. **FAQSection** — FAQ avec Schema.org
11. **ContactSection** — Coordonnées + map
12. **Footer** — Liens, légal, réseaux

### 5.1 Sections pages internes (services, à propos, etc.)
Chaque page interne affiche une section **LocalZonesGrid** en bas de page, montrant 12 zones Paris/IDF dans un **ordre différent** (shuffle déterministe basé sur l'identifiant de la page). Ceci assure un maillage interne varié et un contenu unique par page pour le SEO.

---

## 6. DESIGN SYSTEM

### Palette de couleurs (tokens sémantiques)
- `--primary` : Bleu principal
- `--accent` : Orange CTA
- `--service-blue`, `--service-orange`, `--service-emerald`, `--service-violet`, `--service-rose`, `--service-cyan` : Badges par service
- `--background`, `--foreground`, `--muted`, `--muted-foreground` : Textes et fonds

### Typography
- **Display** : Font-display (titres)
- **Body** : Font sans-serif (texte)

### Composants réutilisables
- Badges colorés par service (style unifié : `bg-[color]/90 text-white border shadow-md backdrop-blur-sm`)
- Cartes avec `card-shadow` / `card-shadow-hover`
- Boutons : `variant="accent"`, `variant="accent-outline"`
- Sections avec `bg-section-gradient`
- Statistiques colorées avec tokens `text-service-blue`, `text-service-violet`, `text-service-emerald`, `text-service-orange`

---

## 7. SEO & GEO

### On-Page SEO
- ✅ H1 unique par page avec mots-clés
- ✅ Meta description unique < 160 chars
- ✅ URLs SEO-friendly
- ✅ Balises ALT sur images
- ✅ Maillage interne contextuel
- ✅ Sitemap XML (93 URLs)
- ✅ Robots.txt (bots IA autorisés : GPTBot, ClaudeBot, PerplexityBot)

### Schema.org
- ✅ LocalBusiness (enrichi : @id, foundingDate, hasCredential RGE/Qualibat)
- ✅ Service (pages services)
- ✅ FAQPage (accueil + pages zones)
- ✅ BreadcrumbList (sous-pages)
- ✅ HowTo ("Comment faire réparer un volet roulant ?")
- ✅ AggregateRating
- ✅ Organization (contactPoint)

### Mots-clés principaux
- Réparation volet roulant Paris
- Installation volet roulant
- Motorisation volet
- Dépannage volet urgence
- Vitrerie Paris
- Volet bloqué
- Artisan RGE volets

### Blog SEO (18 articles)
Sujets : entretien volets, comparatifs marques (Somfy vs Bubendorff), guides motorisation, économies d'énergie, aides financières, volets solaires, articles hyper-locaux (Paris 15e, Marais, Boulogne, Saint-Denis, Versailles, Créteil)

---

## 8. PERFORMANCE & ACCESSIBILITÉ

### Core Web Vitals cibles
- LCP < 2.5s
- FID < 100ms
- CLS < 0.1

### Optimisations
- ✅ Lazy loading images (composants et routes)
- ✅ Code splitting (lazy imports React)
- ✅ Images WebP optimisées
- ✅ Responsive mobile-first
- ✅ Framer Motion animations (fadeUp, stagger, parallaxe)

### Breakpoints
- Mobile : < 640px (1 colonne)
- Tablet : 640-1024px (2 colonnes)
- Desktop : > 1024px (3+ colonnes)

---

## 9. FICHIERS DE DONNÉES

| Fichier | Contenu | Lignes | Statut |
|---------|---------|--------|--------|
| `src/data/zonesPagesData.ts` | 53 pages zones (20 arrondissements + 33 villes IDF) | ~1568 | ✅ OK |
| `src/data/blogArticles.ts` | 18 articles de blog SEO | ~1373 | ✅ OK |
| `src/data/content.ts` | Contenu centralisé (contact, nav, hero, services) | ~100 | ✅ Nettoyé v4.0 |
| `src/data/regionsData.ts` | Données régions Paris + IDF | ~55 | ✅ OK |
| `src/data/idfCities.ts` | Mapping villes IDF par département | ~72 | ✅ OK |
| `src/data/villes-geolocalisation.ts` | Coordonnées GPS des 53 zones | ~63 | ✅ OK |

### Fichiers nettoyés (v4.0)
- ❌ `src/data/citiesData.ts` — **Supprimé** (4463 lignes de données "HD Connect" d'un ancien projet, non utilisé)
- ✅ `src/data/content.ts` — **Nettoyé** (suppression des références "HD Connect", remplacement par contenu Répar'Action Volets)
- ✅ `src/hooks/usePhoneCall.tsx` — **Corrigé** (message WhatsApp mis à jour pour volets roulants)

---

## 10. HARMONISATION VISUELLE (v4.0)

### ✅ Badges overlay services
Style unifié sur toutes les pages services pour correspondre à la page d'accueil :
- `bg-[service-color]/90 text-white border shadow-md backdrop-blur-sm`
- Pages impactées : DepannageExpress, InstallationRemplacement, ReparationVolets, MotorisationDomotique, Vitrerie

### ✅ Statistiques colorées
Couleurs par token sémantique appliquées sur toutes les pages :
- `text-service-blue`, `text-service-violet`, `text-service-emerald`, `text-service-orange`
- Pages impactées : ZonesIntervention, ParisPage, IdFPage, MiniTestimonials, RegionHeroParallax, RepairShowcaseSection

---

## 11. CE QUI RESTE À FAIRE

### 🔴 Priorité haute
- [ ] **Connexion Supabase** : formulaire de devis fonctionnel (envoi emails, stockage données)
- [ ] **Vérification rendu mobile** : tester toutes les pages sur mobile (badges, statistiques, cartes)
- [ ] **Tests E2E** : vérifier tous les liens, redirections et le rendu sur chaque page

### 🟡 Priorité moyenne
- [ ] **Google Business Profile** : configuration et optimisation
- [ ] **Pages régions hors IDF** : activer les redirections vers des pages dédiées quand le contenu sera prêt
- [ ] **Optimisation images** : vérifier poids, dimensions, alt-text de toutes les images
- [ ] **Preconnect fonts / DNS-prefetch** : ajouter dans index.html

### 🟢 Priorité basse
- [ ] **Analytics** : Google Analytics / Tag Manager
- [ ] **Avis Google** : intégration widget avis réels
- [ ] **Newsletter** : capture email pour fidélisation
- [ ] **WhatsApp Business** : intégration API (optionnel)

---

## 12. HISTORIQUE DES VERSIONS

| Version | Date | Changements |
|---------|------|-------------|
| 4.0 | 06/03/2026 | Nettoyage données (suppression HD Connect), harmonisation badges et statistiques colorées sur toutes les pages, mise à jour documentation |
| 3.0 | 04/03/2026 | Consolidation documentation, 18 articles blog, harmonisation design, section régions France complète |
| 2.0 | 23/02/2026 | 53 pages localisées, animations avancées, mobile-first |
| 1.5 | 22/02/2026 | Animations et effets visuels |
| 1.0 | 22/02/2026 | Création initiale, SEO/GEO |

---

## 13. DÉPLOIEMENT

```bash
# Installation
pnpm install

# Développement
pnpm run dev

# Build production
pnpm run build

# Vérification TypeScript
pnpm run check
```

### Checklist pré-déploiement
- [ ] Vérifier types TypeScript
- [ ] Tester toutes les pages
- [ ] Vérifier responsivité mobile
- [ ] Tester animations
- [ ] Vérifier liens internes
- [ ] Vérifier métadonnées SEO
- [ ] Tester formulaires
- [ ] Vérifier images
- [ ] Tester multi-navigateurs
- [ ] Vérifier Core Web Vitals

---

**Répar'Action Volets — Cahier des charges v4.0**
