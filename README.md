# les-fourmis
exercice05Fourmis
* **`classes/`**: Ce dossier contient les fichiers JavaScript définissant chaque classe de fourmi (Fourmi, Reine, Male, Femelle, Princesse, Eclaireuse, Soldat, Larve, Ouvriere, Nourrice). Chaque fichier exporte la classe qu'il définit.
* **`Fourmi.js`**: Définit la classe de base `Fourmi` avec les attributs `age` et `taille`, ainsi que les comportements `dormir` et `manger`. Les attributs sont définis comme privés (`#`).
* **`Reine.js`**: Définit la classe `Reine`, héritant de `Fourmi`, avec l'attribut `nbOeufsPondus` et le comportement `pondre`.
* **`Male.js`**: Définit la classe `Male`, héritant de `Fourmi`, avec les comportements `feconderReine` et `voler`.
* **`Femelle.js`**: Définit la classe `Femelle`, héritant de `Fourmi`, avec le comportement `chercherNourriture`.
* **`Princesse.js`**: Définit la classe `Princesse`, héritant de `Femelle`, avec l'attribut `partenaireMale` et les comportements `voler` (essaimage) et `volNuptial`.
* **`Eclaireuse.js`**: Définit la classe `Eclaireuse`, héritant de `Femelle`, avec l'attribut `rayonAction` et le comportement `explorer`.
* **`Soldat.js`**: Définit la classe `Soldat`, héritant de `Femelle`, avec l'attribut `endurance` et le comportement `attaquer`.
* **`Larve.js`**: Définit la classe `Larve` avec l'attribut `type` et le comportement `metamorphose`.
* **`Ouvriere.js`**: Définit la classe `Ouvriere`, héritant de `Femelle`, avec l'attribut `poste` et les comportements `creuserGalerie`, `nettoyerGalerie` et `chercherNourriture`.
* **`Nourrice.js`**: Définit la classe `Nourrice`, héritant de `Ouvriere`, avec l'attribut `listeLarves` et le comportement `nourrirLarve`.
* **`app.js`**: Ce fichier est le script principal qui importe et teste les différentes classes définies. Il crée des instances de chaque classe et appelle leurs méthodes pour simuler leur comportement. Il affiche également des informations sur l'état des objets dans la console.
* **`index.html`**: Un fichier HTML simple qui inclut les scripts JavaScript en tant que modules (`type="module"`). Il contient un titre et un élément `div` avec l'ID `output` (bien que le script actuel utilise principalement la `console.log`).

## Comment exécuter le projet

Pour exécuter ce projet et observer le résultat des tests dans la console :

1.  Assurez-vous d'avoir un navigateur web moderne qui supporte les modules JavaScript (`type="module"`).
2.  Ouvrez le fichier `index.html` dans votre navigateur web.
3.  Ouvrez la console du développeur de votre navigateur (généralement en appuyant sur F12 ou en faisant un clic droit et en sélectionnant "Inspecter" puis en allant dans l'onglet "Console").
4.  Les résultats des tests (appels de méthodes et affichage des propriétés des objets) seront visibles dans la console.

## Points clés de l'implémentation

* **Attributs privés**: Tous les attributs spécifiés dans le diagramme de classes ont été définis comme privés en utilisant la syntaxe `#` (par exemple, `#age`, `#taille`). L'accès et la modification de ces attributs se font via des getters et des setters publics.
* **Héritage**: Les relations d'héritage entre les classes (indiquées par les flèches dans le diagramme UML) ont été implémentées en utilisant le mot-clé `extends` en JavaScript (par exemple, `class Reine extends Fourmi`).
* **Constructeurs**: Chaque classe possède un constructeur (`constructor`) qui initialise ses attributs et appelle le constructeur de la classe parente avec `super()` si nécessaire.
* **Méthodes**: Les comportements spécifiés dans le diagramme de classes ont été implémentés comme des méthodes au sein de chaque classe.
* **Modules JavaScript**: Le projet utilise les modules JavaScript (`import` et `export`) pour organiser le code dans des fichiers séparés et gérer les dépendances entre les classes.

