
### 1. **Qu'est-ce que Python ?**
Python est un langage de programmation interprété, ce qui signifie que le code est exécuté directement sans nécessiter de compilation préalable. Il est populaire pour sa simplicité de syntaxe, ce qui le rend facile à lire et à écrire.

### 2. **Installation et configuration**
- Python est généralement installé sur la plupart des systèmes d'exploitation. Vous pouvez vérifier si Python est installé sur votre machine en exécutant `python --version` ou `python3 --version` dans votre terminal.
- Si Python n'est pas installé, vous pouvez le télécharger sur le site officiel : [python.org](https://www.python.org/downloads/).

### 3. **Syntaxe de base**
La syntaxe Python est simple et lisible. Voici quelques concepts clés :

#### 3.1. **Impression à l'écran**
```python
print("Hello, World!")
```
Cette instruction affiche le texte "Hello, World!" sur la console.

#### 3.2. **Variables**
Les variables en Python sont des conteneurs utilisés pour stocker des valeurs.
```python
x = 5
y = "Bonjour"
```
Ici, `x` est une variable qui contient un nombre, et `y` contient une chaîne de caractères (texte).

#### 3.3. **Types de données**
Les principaux types de données en Python sont :
- **int** : entiers (ex. `x = 10`)
- **float** : nombres décimaux (ex. `y = 10.5`)
- **str** : chaînes de caractères (ex. `name = "Alice"`)
- **bool** : valeurs booléennes (ex. `is_valid = True`)

#### 3.4. **Opérateurs**
- **Opérateurs arithmétiques** : `+`, `-`, `*`, `/`, `%` (modulo)
- **Opérateurs de comparaison** : `==`, `!=`, `>`, `<`, `>=`, `<=`
- **Opérateurs logiques** : `and`, `or`, `not`

### 4. **Conditions**
Les conditions permettent de prendre des décisions en fonction de certaines situations :
```python
x = 10
if x > 5:
    print("x est supérieur à 5")
elif x == 5:
    print("x est égal à 5")
else:
    print("x est inférieur à 5")
```
L'indentation est cruciale en Python. Elle permet de structurer le code et définir des blocs.

### 5. **Boucles**
#### 5.1. **Boucle `for`**
Utilisée pour parcourir une séquence (liste, chaîne de caractères, etc.)
```python
for i in range(5):
    print(i)
```
Cela affiche les nombres de 0 à 4.

#### 5.2. **Boucle `while`**
Exécute un bloc de code tant qu'une condition est vraie.
```python
x = 0
while x < 5:
    print(x)
    x += 1
```

### 6. **Fonctions**
Les fonctions permettent de structurer et de réutiliser du code.
```python
def saluer(nom):
    print(f"Bonjour, {nom}!")

saluer("Alice")
```
Ici, la fonction `saluer` prend un paramètre `nom` et affiche un message personnalisé.

### 7. **Listes et dictionnaires**
#### 7.1. **Listes**
Les listes sont des collections ordonnées et modifiables.
```python
fruits = ["pomme", "banane", "cerise"]
print(fruits[0])  # Affiche "pomme"
fruits.append("orange")  # Ajoute un élément
```

#### 7.2. **Dictionnaires**
Les dictionnaires sont des collections non ordonnées qui associent des clés à des valeurs.
```python
personne = {"nom": "Alice", "âge": 25}
print(personne["nom"])  # Affiche "Alice"
personne["âge"] = 26  # Modifie la valeur de l'âge
```

### 8. **Gestion des erreurs**
Python propose des blocs `try` et `except` pour gérer les exceptions (erreurs).
```python
try:
    x = 1 / 0
except ZeroDivisionError:
    print("Erreur : division par zéro")
```

### 9. **Entrée utilisateur**
Vous pouvez demander une entrée de l'utilisateur avec `input()`.
```python
nom = input("Quel est votre nom ? ")
print(f"Bonjour, {nom}")
```

### 10. **Modules**
Python dispose d'une riche bibliothèque standard et vous pouvez importer des modules pour ajouter des fonctionnalités.
```python
import math
print(math.sqrt(16))  # Affiche 4.0
```

### Exercice simple :
Essayez d'écrire un programme qui demande à l'utilisateur son âge et affiche un message s'il est majeur ou mineur :
```python
age = int(input("Quel est votre âge ? "))
if age >= 18:
    print("Vous êtes majeur.")
else:
    print("Vous êtes mineur.")
```

Ce cours couvre les bases essentielles de Python. Une fois que vous maîtrisez ces concepts, vous pouvez passer à des sujets plus avancés comme la programmation orientée objet, les classes, les modules, et les frameworks comme Flask ou Django pour le développement web.