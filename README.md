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

1. Téléchargement du SDK .NET Core 2.1.817 (dernière version du 2.1) depuis :  
   https://dotnet.microsoft.com/download/dotnet-core/2.1
   <img width="1439" height="681" alt="Capture d’écran 2025-11-24 à 14 00 07" src="https://github.com/user-attachments/assets/a998304d-2ef5-4b76-b30c-7762bee56487" />
3. Installation complète du SDK + Hosting Bundle.
4. Redémarrage de l’ordinateur.
5. Vérification avec la commande :

```bash
dotnet --info
