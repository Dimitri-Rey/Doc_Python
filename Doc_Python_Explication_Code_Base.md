
### Programme Python Simple

```python
# Fonction pour demander et retourner le nom de l'utilisateur
def demander_nom():
    nom = input("Quel est votre nom ? ")
    return nom

# Fonction pour demander et retourner l'âge de l'utilisateur
def demander_age():
    age = int(input("Quel est votre âge ? "))
    return age

# Fonction qui affiche un message basé sur l'âge
def afficher_message(nom, age):
    if age >= 18:
        print(f"Bonjour {nom}, vous êtes majeur.")
    else:
        print(f"Bonjour {nom}, vous êtes mineur.")

# Programme principal
nom_utilisateur = demander_nom()  # Appelle la fonction pour obtenir le nom
age_utilisateur = demander_age()  # Appelle la fonction pour obtenir l'âge
afficher_message(nom_utilisateur, age_utilisateur)  # Affiche un message basé sur les informations fournies
```

### Explication détaillée

#### 1. **Variables**
Les variables sont des conteneurs qui stockent des informations que vous pouvez réutiliser plus tard dans le programme.

- **`nom_utilisateur`** : Stocke le nom saisi par l'utilisateur.
- **`age_utilisateur`** : Stocke l'âge saisi par l'utilisateur.

Les variables sont utilisées pour maintenir des valeurs dans un programme et passer ces valeurs entre les différentes fonctions.

#### 2. **Opérateurs**
Les opérateurs sont utilisés pour comparer, additionner ou effectuer d'autres opérations sur des valeurs.

- **Opérateur de comparaison (`>=`)** : Dans la condition `if age >= 18`, on compare l'âge de l'utilisateur avec 18 pour déterminer s'il est majeur ou mineur.
- **Opérateur d'assignation (`=`)** : Il est utilisé pour assigner des valeurs aux variables comme dans `nom_utilisateur = demander_nom()`.

#### 3. **Fonctions**
Les fonctions sont des blocs de code réutilisables qui effectuent une tâche spécifique. Elles prennent des **paramètres** et peuvent retourner une **valeur**.

- **`demander_nom()`** : Demande le nom de l'utilisateur via `input()` et le renvoie.
- **`demander_age()`** : Demande l'âge de l'utilisateur, convertit la chaîne en entier avec `int()`, et le renvoie.
- **`afficher_message(nom, age)`** : Affiche un message personnalisé en fonction de l'âge, avec une condition pour vérifier si l'utilisateur est majeur ou mineur.

---

### Tableau explicatif des concepts en Markdown

| Concept      | Explication                                                                                  | Exemple                                                                  |
|--------------|----------------------------------------------------------------------------------------------|--------------------------------------------------------------------------|
| **Variable** | Une variable stocke une valeur qui peut être utilisée et modifiée dans le programme.          | `nom_utilisateur = demander_nom()`                                        |
| **Opérateur**| Les opérateurs permettent d'effectuer des opérations sur les valeurs (comparaison, calcul).   | `age >= 18` (comparaison), `age = int(input())` (assignation)             |
| **Fonction** | Une fonction est un bloc de code qui réalise une tâche précise. Elle peut prendre des arguments et retourner une valeur. | `def afficher_message(nom, age):`                                         |
| **Condition**| Permet de prendre une décision basée sur une expression booléenne (vrai ou faux).             | `if age >= 18:` (si l'âge est supérieur ou égal à 18, alors...)           |
| **Entrée**   | La fonction `input()` permet d'obtenir des informations saisies par l'utilisateur.            | `nom = input("Quel est votre nom ? ")`                                    |
| **Affichage**| La fonction `print()` permet d'afficher des informations à l'écran.                           | `print(f"Bonjour {nom}, vous êtes majeur.")`                              |

---

### Détails supplémentaires :

1. **`input()`** : Cette fonction demande à l'utilisateur de saisir une valeur. Elle retourne toujours une chaîne de caractères.
   ```python
   nom = input("Quel est votre nom ? ")  # Le nom est saisi par l'utilisateur
   ```

2. **`int()`** : Convertit une chaîne de caractères en entier. Ceci est important, car `input()` retourne toujours une chaîne, même si l'utilisateur entre un nombre.
   ```python
   age = int(input("Quel est votre âge ? "))  # Convertit l'entrée en entier
   ```

3. **Conditions (`if/else`)** : La condition `if age >= 18` vérifie si l'âge est supérieur ou égal à 18. Si la condition est vraie, un message pour les majeurs est affiché. Sinon, le message pour les mineurs est affiché.
   ```python
   if age >= 18:
       print(f"Bonjour {nom}, vous êtes majeur.")
   else:
       print(f"Bonjour {nom}, vous êtes mineur.")
   ```

---

### Conclusion

Ce programme simple utilise les notions de **variables**, d'**opérateurs**, de **fonctions**, et de **conditions** pour réaliser une interaction avec l'utilisateur. Il demande des entrées utilisateur, compare ces valeurs, et affiche des résultats basés sur cette comparaison. Vous pouvez le modifier et l'améliorer pour inclure plus de fonctionnalités ou de conditions.