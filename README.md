# TP .NET - Boutique Diayma

## 1. Présentation
Ce projet est une application ASP.NET Core permettant d’afficher une liste de produits d’une boutique appelée "Diayma".

---

## 2. Exécution du projet
Le projet a été ouvert avec Visual Studio et exécuté avec IIS Express.

---

## 3. Version .NET
Le projet utilise .NET Core 2.0.

---

## 4. Problèmes rencontrés
- Erreur de lancement due à l’absence de .NET Core 2.0
- Solution : installation du runtime .NET Core 2.0

---

## 5. Dépôt GitHub
Le code source est disponible sur GitHub :

Lien : https://github.com/Amethnb2218/TP-Diayma-Debug

---

## 6. Débogage

### Points d’arrêt
Un point d’arrêt est représenté par un point rouge dans le code. Lorsque le programme atteint cette ligne, il s’arrête et la ligne devient jaune.

---

## 7. Parcours d’exécution

Lors du débogage, l’exécution commence dans la classe **Program** avec la méthode **Main()**.

Ensuite, l’application passe par la classe **Startup** pour configurer les services.

Puis, la requête est dirigée vers le contrôleur **ProductController**.

La méthode **Index()** est appelée, et elle récupère les produits grâce à :

```csharp
_productService.GetAllProducts();
