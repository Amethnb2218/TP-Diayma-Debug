# TP .NET - Boutique Diayma

## 1. Présentation

Ce projet est une application ASP.NET Core permettant d’afficher une liste de produits d’une boutique appelée **Diayma**.

---

## 2. Exécution du projet

Le projet a été ouvert avec **Visual Studio** et exécuté avec **IIS Express**.

---

## 3. Version .NET

Le projet utilise **.NET Core 2.0**.

---

## 4. Problèmes rencontrés

Lors de l’exécution du projet, une erreur est apparue indiquant que la version .NET Core 2.0 était manquante.

### Solution :

Installation du runtime **.NET Core 2.0**, ce qui a permis de lancer correctement l’application.

---

## 5. Dépôt GitHub

Le code source du projet est disponible sur GitHub :

Lien : https://github.com/Amethnb2218/TP-Diayma-Debug

---

## 6. Débogage

### Points d’arrêt

Un point d’arrêt est représenté par un **point rouge** dans le code.
Lorsque le programme atteint cette ligne, il s’arrête et la ligne devient **jaune**, ce qui permet d’analyser l’exécution.

---

## 7. Parcours d’exécution

Lors du débogage, l’exécution du programme commence dans la classe **Program** avec la méthode **Main()**.

Ensuite, l’application passe par la classe **Startup** pour configurer les services et le routage.

Puis, la requête est dirigée vers le contrôleur **ProductController**.

La méthode **Index()** est appelée, et elle récupère la liste des produits grâce à :

```csharp
_productService.GetAllProducts();
```

Lors de l’exécution, il a été observé que la liste contient **9 produits**.

Enfin, les produits sont envoyés à la vue avec :

```csharp
return View(products);
```

ce qui permet leur affichage dans le navigateur.

---

## 8. Éléments observés

### Namespaces :

* P2FixAnAppDotNetCode
* P2FixAnAppDotNetCode.Controllers

### Classes :

* Program
* Startup
* ProductController

### Méthodes :

* Main()
* Startup()
* ConfigureServices()
* Index()

---

## 9. Modes de débogage utilisés

* **F10** : pas à pas principal (ligne par ligne)
* **F11** : pas à pas détaillé (entrer dans les méthodes)
* **Shift + F11** : sortir d’une méthode

---

## 10. Conclusion

Le débogage a permis de comprendre le fonctionnement de l’application, notamment le chemin parcouru avant l’affichage des produits, depuis **Program** jusqu’au **ProductController**.

Ce TP a permis de mieux comprendre :

* l’exécution d’une application ASP.NET Core
* l’utilisation du débogage
* la structure d’un projet .NET

---

11. Lien de téléchargement
L’application a été publiée sous forme d’exécutable Windows.

Lien : https://drive.google.com/file/d/1J9mzAKETvFoC0sxRqPIV-C_RtVVWaA0z/view?usp=drive_link
