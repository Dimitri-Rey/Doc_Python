### 1. **Blocs de code**
Les blocs de code en Python sont définis par **l'indentation** (des espaces ou des tabulations). Python utilise cette indentation pour organiser les instructions.

Exemple d'un bloc de code dans une condition `if` :
```python
if True:
    print("Ceci fait partie du bloc conditionnel")
    x = 10  # Indentation obligatoire pour le bloc
```

### 2. **Variables**
Les variables sont des conteneurs qui permettent de stocker des données. En Python, vous n'avez pas besoin de déclarer explicitement le type de la variable ; il est automatiquement déterminé par l'assignation.

Exemple :
```python
nom = "Alice"  # Variable de type chaîne de caractères (str)
age = 25  # Variable de type entier (int)
```

**Règles de nommage** :
- Ne peut pas commencer par un chiffre.
- Peut contenir des lettres, des chiffres et des underscores (`_`).
- Sensible à la casse (`age` et `Age` sont deux variables différentes).

### 3. **Opérateurs**
Les opérateurs sont utilisés pour effectuer des opérations sur les variables et les valeurs.

#### 3.1. **Opérateurs arithmétiques**
- Addition : `+`
- Soustraction : `-`
- Multiplication : `*`
- Division : `/`
- Modulo (reste de la division) : `%`
- Puissance : `**`
  
Exemple :
```python
x = 5 + 3  # x vaut 8
y = 10 % 3  # y vaut 1 (10 divisé par 3 donne un reste de 1)
```

#### 3.2. **Opérateurs de comparaison**
Ils sont utilisés pour comparer deux valeurs et renvoient un résultat booléen (`True` ou `False`).
- Égalité : `==`
- Différence : `!=`
- Plus grand : `>`
- Plus petit : `<`
- Supérieur ou égal : `>=`
- Inférieur ou égal : `<=`

Exemple :
```python
a = 5
b = 10
print(a == b)  # False
print(a < b)   # True
```

#### 3.3. **Opérateurs logiques**
- **`and`** : Retourne `True` si les deux conditions sont vraies.
- **`or`** : Retourne `True` si au moins une des conditions est vraie.
- **`not`** : Inverse le résultat, retourne `False` si c'est `True` et vice versa.

Exemple :
```python
x = 5
print(x > 3 and x < 10)  # True
print(not(x > 3))  # False
```

### 4. **Portée des variables (scope)**
La portée d'une variable fait référence à l'endroit où elle est accessible dans le code. En Python, il existe deux types principaux de portée :
- **Portée locale** : Les variables définies à l'intérieur d'une fonction ou d'un bloc n'existent que dans cette fonction ou ce bloc.
- **Portée globale** : Les variables définies en dehors de toute fonction sont accessibles partout dans le script.

Exemple :
```python
x = 10  # Variable globale

def ma_fonction():
    x = 5  # Variable locale
    print(x)

ma_fonction()  # Affiche 5
print(x)  # Affiche 10 (la variable globale)
```

### 5. **Boucles**

#### 5.1. **Boucle `for`**
La boucle `for` en Python est utilisée pour itérer sur une séquence (comme une liste ou une chaîne de caractères).

Exemple :
```python
fruits = ["pomme", "banane", "cerise"]
for fruit in fruits:
    print(fruit)
```

#### 5.2. **Boucle `while`**
La boucle `while` continue tant qu'une condition est vraie.

Exemple :
```python
i = 0
while i < 5:
    print(i)
    i += 1
```

### 6. **Procédures (Fonctions)**
Les fonctions permettent de regrouper un ensemble d'instructions sous un nom, que l'on peut appeler à plusieurs reprises.

#### 6.1. **Définir une fonction**
En Python, on définit une fonction à l'aide du mot-clé `def` suivi du nom de la fonction et d'une liste de paramètres (facultative).

Exemple :
```python
def saluer(nom):
    print(f"Bonjour, {nom}!")

saluer("Alice")  # Appelle la fonction avec "Alice" comme argument
```

#### 6.2. **Retourner une valeur**
Une fonction peut renvoyer une valeur à l'aide du mot-clé `return`.
```python
def addition(a, b):
    return a + b

resultat = addition(5, 3)  # résultat vaut 8
```

### 7. **Entrées et sorties**
Vous pouvez demander une entrée à l'utilisateur avec la fonction `input()`, qui retourne toujours une chaîne de caractères.

Exemple :
```python
nom = input("Entrez votre nom : ")
print(f"Bonjour, {nom}")
```

Pour convertir une entrée en entier ou en nombre à virgule flottante, vous pouvez utiliser `int()` ou `float()` :
```python
age = int(input("Entrez votre âge : "))
```

### 8. **Exercice récapitulatif :**
Voici un exemple qui rassemble plusieurs des concepts vus :
```python
def demander_age():
    age = int(input("Quel est votre âge ? "))
    return age

def verifier_majorite(age):
    if age >= 18:
        print("Vous êtes majeur.")
    else:
        print("Vous êtes mineur.")

age_utilisateur = demander_age()
verifier_majorite(age_utilisateur)
```

Cet exercice demande l'âge de l'utilisateur, puis affiche un message en fonction de son âge.

Ces concepts couvrent les bases essentielles de Python pour commencer à écrire des programmes fonctionnels et bien structurés.