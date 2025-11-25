# Boutique Diayma Assietou NDIAYE 

## 1. Récupérez dans Visual Studio et exécutez le code fourni lien Github. 
- Voici le code  dans github
<img width="1439" height="409" alt="Capture d’écran 2025-11-24 à 13 28 48" src="https://github.com/user-attachments/assets/45f2d9bf-6fac-4ad0-98a9-b1cff1f9724c" />

- Voici le code dans Rider (sur Macos)
<img width="1439" height="633" alt="Capture d’écran 2025-11-24 à 22 24 37" src="https://github.com/user-attachments/assets/e960e870-7c24-4106-8308-ec95fc7497d1" />



## 2. Quels sont les projets de la solution ?

- Ouvrir le fichier **Diayma.sln** avec Rider 
- Dans l’Explorateur de solutions, on observe :

| Projet     | Type                        | Framework      | Observations |
|------------|-----------------------------|----------------|--------------|
| **Diayma** | Application web ASP.NET Core MVC | .NET Core 2.0 | Projet unique contenant tout le code (contrôleurs, vues, modèles, services, localisation, etc.) |

<img width="1439" height="201" alt="Capture d’écran 2025-11-24 à 13 35 35" src="https://github.com/user-attachments/assets/5cbf89a3-e23a-4c72-a2b5-33e06c150981" />

**Il n’existe qu’un seul projet dans la solution Diayma.sln.**


### 3. Quelle est la version SDK .NET utilisée par ces projets ?

**Version du SDK .NET utilisée : 2.1 (SDK .NET Core 2.0)**  
Il faut installer le SDK 2.1 pour que `dotnet restore` et `dotnet build` fonctionnent sans erreur.
<img width="1439" height="217" alt="Capture d’écran 2025-11-24 à 20 51 03" src="https://github.com/user-attachments/assets/01bfbfe9-c9ff-4cd0-85a1-8f2f0df47236" />


## 4. Installez le SDK

Le projet nécessite le **SDK .NET Core 2.1**.

### Étapes réalisées :

1. Téléchargement du SDK .NET Core 2.1.817 (dernière version du 2.1) depuis   
   https://dotnet.microsoft.com/download/dotnet-core/2.1
   <img width="1439" height="681" alt="Capture d’écran 2025-11-24 à 14 00 07" src="https://github.com/user-attachments/assets/a998304d-2ef5-4b76-b30c-7762bee56487" />

2. Installation complète du SDK + Hosting Bundle
<img width="1439" height="364" alt="Capture d’écran 2025-11-24 à 13 58 32" src="https://github.com/user-attachments/assets/8a492733-71a9-44a5-9229-6542344f6dbf" />

3. Vérification avec la commande 
<img width="1439" height="531" alt="Capture d’écran 2025-11-24 à 15 16 04" src="https://github.com/user-attachments/assets/f06fae91-715a-4ed4-8b5a-c91c40cd7e25" />

## 5. Créez votre propre dépôt GitHub pour y stocker le code

Dépôt créé et code publié avec succès :  
lien :https://github.com/assietoundiaye/AN_Diayma2025

<img width="1439" height="644" alt="Capture d’écran 2025-11-24 à 15 06 36" src="https://github.com/user-attachments/assets/625981ef-9e96-44ec-bc97-a2a26e33dc5a" />

Résumé des étapes finales :

<img width="1439" height="300" alt="Capture d’écran 2025-11-24 à 15 07 28" src="https://github.com/user-attachments/assets/5332352a-2604-4195-9192-37f8765f76eb" />


## 6. Explorez l’application. Signalez 2 bugs trouvés
1,Le montant total du panier ne prend pas en compte la quantité des produits (toujours calculé comme si la quantité était 1)
<img width="1439" height="633" alt="Capture d’écran 2025-11-24 à 22 15 23" src="https://github.com/user-attachments/assets/8e10f3f3-bd9e-4fc6-b1bb-49b85b439663" />

2,Les page  n’est jamais traduite en espagnol et reste toujours en français ou anglais  quel que soit le sélecteur de langue
<img width="1439" height="633" alt="Capture d’écran 2025-11-24 à 22 41 20" src="https://github.com/user-attachments/assets/89aefb57-e60e-4a6c-8925-b7ad90fc708a" />


## 7. Placez un point d’arrêt sur les lignes suivantes du code :

**a) CartSummaryViewComponent ligne 12

<img width="1439" height="586" alt="Capture d’écran 2025-11-24 à 20 13 35" src="https://github.com/user-attachments/assets/1fa98007-dace-4f63-955d-96496f8be94d" />

**b) ProductController ligne 15

<img width="1439" height="596" alt="Capture d’écran 2025-11-24 à 20 19 12" src="https://github.com/user-attachments/assets/8336ba06-5c70-4618-8eb6-dbf7ac8256a7" />


c) OrderController ligne 17

<img width="1439" height="691" alt="Capture d’écran 2025-11-24 à 20 26 46" src="https://github.com/user-attachments/assets/021dc762-86f2-4bc9-a9fa-30d489fa6e69" />


d) CartController ligne 15

<img width="1439" height="673" alt="Capture d’écran 2025-11-24 à 20 29 31" src="https://github.com/user-attachments/assets/040cd41f-53fb-435a-a43f-a27503bc03cc" />


e) Startup ligne 20

<img width="1439" height="673" alt="Capture d’écran 2025-11-24 à 20 31 12" src="https://github.com/user-attachments/assets/4f59178c-0d83-434a-9f02-3d613a08dc2e" />


## 8. Namespaces, classes et méthodes visités avant l’affichage des produits sur l’écran d’accueil

L’application a été lancée en mode debug avec **RIDER.  
Un point d’arrêt a été placé sur la toute première ligne exécutable de `Startup.cs` (ligne 20) puis sur `ProductController.Index`.


### Séquence complète observée lors de l’accès à http://localhost:62929/

| Étape | Namespace                                      | Classe                                         | Méthode / Propriété significative                                      | Commentaire / Raison du passage                                      |
|-------|------------------------------------------------|------------------------------------------------|-------------------------------------------------------------------------|----------------------------------------------------------------------|
| 1     | `Microsoft.AspNetCore`                         | `WebHost`                                      | `CreateDefaultBuilder()` → `Build()` → `Run()`                          | Point d’entrée du programme (Program.cs)                             |
| 2     | `Microsoft.AspNetCore.Builder`                 | `ApplicationBuilder`                           | `UseRouting()`, `UseStaticFiles()`, `UseEndpoints()`                    | Configuration des middlewares dans Startup.Configure                  |
| 3     | `Microsoft.Extensions.DependencyInjection`    | `ServiceCollection`                            | `AddScoped<>`, `AddMvc()`, `AddLocalization()`                         | Enregistrement des services dans **Startup.ConfigureServices**       |
| 4     | `Microsoft.AspNetCore.Mvc.ApplicationModels`  | (framework)                                    | Résolution du contrôleur par convention                                | Recherche du contrôleur correspondant à la route "/"                 |
| 5     | `P2FixAnAppDotNetCode.Controllers`            | **ProductController**                          | **Index()** (ligne ~15)                                                 | Contrôleur appelé pour la route par défaut                          |
| 6     | `P2FixAnAppDotNetCode.Services`                | `ProductService`                               | `GetAllProducts()`                                                      | Appel du service injecté                                             |
| 7     | `P2FixAnAppDotNetCode.Repositories`            | `ProductRepository`                            | `GetAll()` ou `ToList()`                                                | Récupération des produits depuis la source (mémoire ou DB)           |
| 8     | `P2FixAnAppDotNetCode.Models`                  | `Product`                                      | Constructeur / propriétés                                               | Instanciation des objets métier                                      |
| 9     | `Microsoft.AspNetCore.Mvc`                     | `ViewResult`                                   | `ExecuteResultAsync()` → rendu de `/Views/Product/Index.cshtml`         | Génération du HTML                                                           |
| 10    | `P2FixAnAppDotNetCode.Components`             | **CartSummaryViewComponent**                   | `Invoke()` → ligne 12 (`return View(cart)`)                             | Composant de vue appelé dans le _Layout.cshtml                       |
| 11    | `P2FixAnAppDotNetCode.Models`                  | `Cart` + `SessionCart`                         | `GetCart()` (extension session)                                         | Récupération du panier depuis la session                             |
| 12    | `Microsoft.AspNetCore.Localization`            | (middleware)                                   | Lecture du cookie/culture → définition de `CultureInfo.CurrentCulture`  | Gestion de la langue (FR/EN)                                         |


## 9. Déploiement de la solution sous forme d’exécutable Windows

**Contexte important** : La fonctionnalité `PublishSingleFile` n’est officiellement supportée qu’à partir de .NET Core 3.0.  
Dans .NET Core 2.1 (notre version), elle est désactivée même si les options sont passées.

**Solution appliquée et validée** : Publication **self-contained** (autonome) avec trimming → tout le dossier `publish` est 100 % exécutable sur Windows sans installation de .NET.

Commande exécutée :
<img width="1439" height="328" alt="Capture d’écran 2025-11-24 à 20 54 37" src="https://github.com/user-attachments/assets/45d43c26-3495-4913-a55d-b157a90812b5" />

Lien: 
https://drive.google.com/drive/folders/1JJ5Sq4qjWBl9VjStJvw85x35F7_y9Ht1?usp=share_link

## 8. Optionnel :
a) Ajoutez une langue d’affichage à l’interface, Wolof par exemple. Conservez les options de
culture du français.
<img width="1439" height="762" alt="Capture d’écran 2025-11-24 à 22 49 22" src="https://github.com/user-attachments/assets/5c1cba29-db78-4e52-a40d-c39529c22f85" />


