En Python, il existe plusieurs types de données intégrés qui permettent de stocker et de manipuler différents types de valeurs. Voici un aperçu des types les plus courants :

| Type      | Description                                      | Exemple                               |
|-----------|--------------------------------------------------|---------------------------------------|
| `int`     | Nombres entiers                                  | 10, -5, 0                            |
| `float`   | Nombres à virgule flottante                      | 3.14, -2.5, 0.0                      |
| `str`     | Chaînes de caractères                            | 'Python', 'Alice', 'Bonjour'          |
| `bool`    | Valeurs booléennes (True/False)                  | True, False                          |
| `list`    | Collection ordonnée et modifiable                | [1, 2, 3], ['pomme', 'banane']        |
| `tuple`   | Collection ordonnée et immuable                  | (1, 2, 3), ('rouge', 'bleu')          |
| `dict`    | Collection non ordonnée de paires clé-valeur     | {'nom': 'Alice', 'âge': 25}           |
| `set`     | Collection non ordonnée d'éléments uniques       | {1, 2, 3}, {'pomme', 'banane'}        |
| `NoneType`| Absence de valeur ou valeur nulle                | None                                 |

### 1. **Types numériques**
Python supporte différents types de nombres, chacun adapté à des besoins spécifiques.

#### 1.1. **`int` (entier)**
Les entiers représentent des nombres sans décimales, positifs ou négatifs, de taille illimitée en Python (contrairement à d'autres langages comme C où la taille est limitée).

Exemples :
```python
x = 10  # Un entier positif
y = -25  # Un entier négatif
```

#### 1.2. **`float` (nombre à virgule flottante)**
Les nombres à virgule flottante représentent des nombres réels avec des décimales. Ils sont utilisés pour les calculs nécessitant des valeurs fractionnaires.

Exemples :
```python
a = 3.14  # Nombre flottant
b = -7.5  # Nombre flottant négatif
```

#### 1.3. **`complex` (nombre complexe)**
Python prend en charge les nombres complexes, composés d'une partie réelle et d'une partie imaginaire, notée `j` en Python (au lieu de `i`).

Exemple :
```python
z = 1 + 2j  # Nombre complexe (1 est la partie réelle, 2 est la partie imaginaire)
```

### 2. **Chaînes de caractères (`str`)**
Les chaînes de caractères sont des séquences de texte entourées de guillemets simples (`' '`) ou doubles (`" "`). Elles sont immuables, ce qui signifie qu'une fois créées, elles ne peuvent pas être modifiées.

Exemple :
```python
texte = "Bonjour, Python!"
```

Les chaînes de caractères peuvent être manipulées de différentes manières :
- **Concaténation** : Fusionner deux chaînes.
  ```python
  nom = "Alice"
  salutation = "Bonjour, " + nom
  ```

- **Indexation** : Accéder à un caractère spécifique dans la chaîne.
  ```python
  premier_caractere = texte[0]  # 'B'
  ```

- **Slicing** : Extraire une sous-chaîne.
  ```python
  sous_chaine = texte[0:7]  # 'Bonjour'
  ```

### 3. **Booléens (`bool`)**
Les booléens sont un type de données qui ne peut prendre que deux valeurs : `True` (vrai) ou `False` (faux). Ils sont souvent utilisés dans les conditions et les comparaisons.

Exemple :
```python
is_valid = True
```

Les booléens résultent souvent d'expressions conditionnelles :
```python
resultat = (10 > 5)  # True
```

### 4. **Listes (`list`)**
Les listes sont des collections ordonnées, modifiables et qui peuvent contenir des éléments de types variés. Elles sont définies entre crochets (`[]`).

Exemple :
```python
fruits = ["pomme", "banane", "cerise"]
nombres = [1, 2, 3, 4, 5]
melange = [1, "texte", True, 3.14]
```

Vous pouvez :
- **Ajouter un élément** : `fruits.append("orange")`
- **Supprimer un élément** : `fruits.remove("banane")`
- **Accéder à un élément** par son index : `fruits[0]`  # "pomme"

### 5. **Tuples (`tuple`)**
Les tuples sont des collections ordonnées, mais **immuables** (non modifiables après leur création). Ils sont souvent utilisés pour représenter des ensembles de données qui ne doivent pas être modifiés. Les tuples sont définis avec des parenthèses (`()`).

Exemple :
```python
coordonnees = (10.0, 20.0)
```

Vous pouvez accéder aux éléments du tuple par leur index, mais vous ne pouvez pas les modifier :
```python
x = coordonnees[0]  # 10.0
# coordonnees[0] = 15.0  # Cela provoquerait une erreur
```

### 6. **Dictionnaires (`dict`)**
Les dictionnaires sont des collections non ordonnées d'éléments en **paires clé-valeur**. Ils sont utilisés pour stocker des données qui peuvent être facilement récupérées par une clé.

Exemple :
```python
personne = {"nom": "Alice", "âge": 25, "ville": "Paris"}
```

Vous pouvez accéder et modifier les valeurs à l'aide des clés :
```python
nom = personne["nom"]  # "Alice"
personne["âge"] = 26  # Modifie l'âge
```

### 7. **Ensembles (`set`)**
Les ensembles sont des collections non ordonnées d'éléments uniques. Ils sont utiles pour stocker des valeurs sans duplication. Les ensembles sont définis avec des accolades (`{}`).

Exemple :
```python
nombres = {1, 2, 3, 4, 4, 5}  # L'ensemble ne contient que des éléments uniques
```

Opérations courantes sur les ensembles :
- **Ajout d'un élément** : `nombres.add(6)`
- **Union** : `ensemble1.union(ensemble2)`
- **Intersection** : `ensemble1.intersection(ensemble2)`

### 8. **NoneType**
`None` est un type spécial en Python qui représente l'absence de valeur ou une valeur nulle.

Exemple :
```python
x = None
```

`None` est souvent utilisé pour indiquer qu'une variable ne contient aucune donnée ou qu'une fonction ne retourne pas de résultat.

### 9. **Les types composites (objets)**
Python est un langage orienté objet, ce qui signifie que vous pouvez créer vos propres types de données en définissant des **classes**. Une classe est un modèle pour créer des objets (des instances de la classe).

Exemple d'une classe simple :
```python
class Personne:
    def __init__(self, nom, age):
        self.nom = nom
        self.age = age

    def saluer(self):
        print(f"Bonjour, je m'appelle {self.nom}.")

# Créer une instance de la classe Personne
personne1 = Personne("Alice", 25)
personne1.saluer()  # "Bonjour, je m'appelle Alice."
```

### 10. **Conversion entre types**
Python permet la conversion explicite d'un type à un autre. Par exemple, vous pouvez convertir une chaîne de caractères en entier ou un entier en flottant.

Exemples de conversions :
```python
x = int("10")  # Convertit une chaîne en entier
y = float(5)   # Convertit un entier en flottant
z = str(123)   # Convertit un entier en chaîne
```

### Conclusion
En Python, la flexibilité des types permet de travailler avec des données variées tout en gardant une syntaxe simple et intuitive. Les structures de données comme les listes, tuples, dictionnaires et ensembles offrent de puissants outils pour organiser et manipuler les informations dans vos programmes.


