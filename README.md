# FoodApp

Application Android de recettes de cuisine, entièrement en Kotlin et Jetpack Compose. Projet de groupe réalisé en cours, avec une attention particulière portée à l'interface.

## Fonctionnalités

- Écran d'accueil avec les recettes classées par catégorie
- Recherche et liste des catégories
- Fiche détaillée de chaque plat (description, ingrédients, informations)
- Page des favoris
- Profil utilisateur avec statistiques et menu (modifier le profil, favoris, contact, déconnexion)
- Barre de navigation en bas (Accueil, Recherche, Favoris, Profil)
- Écrans de lancement, de connexion et d'inscription

## Technologies

- Kotlin
- Jetpack Compose et Material Design 3
- Navigation Compose
- Une seule `Activity`, tous les écrans sont des composables
- Gradle (Kotlin DSL) avec catalogue de versions
- SDK minimum 24

## Structure

```
app/src/main/java/com/example/foodapp_kotlin/
  MainActivity.kt        point d'entrée et navigation
  model/                 Recipe, Category, UserPreference
  data/                  base de données de l'application
  ui/
    components/          MainScaffold, TopBar, BottomBar, RecipeCard, CategoryCard, FoodSection
    screens/             Splash, Login, Register, Home, Search, Dish, Favorites,
                         Profile, EditProfile, Contact, AllRecipes, CategoryDetail
    theme/               couleurs, typographie, thème
```

## Lancer le projet

1. Cloner le dépôt :
   ```bash
   git clone https://github.com/imene-be/recipe-app-android.git
   ```
2. L'ouvrir avec **Android Studio** (Hedgehog ou plus récent).
3. Laisser Gradle se synchroniser, puis lancer sur un émulateur ou un téléphone (Android 7.0 minimum).

## État du projet

Les recettes sont pour l'instant des données statiques. Pistes pour la suite :

- Connecter une vraie base de données (Room ou Firebase)
- Rendre les favoris persistants
- Implémenter la recherche
- Ajouter une authentification réelle

---

Projet réalisé en groupe par [Imène Bentifraouine](https://imenebe.fr), Lyam Matic et Ewen Lukacik.
