

### 1. **Installer Python et VS Code**
   - Assure-toi que Python est installé sur ton système. Tu peux le télécharger depuis [python.org](https://www.python.org/).
   - Installe VS Code si ce n'est pas encore fait : [VS Code](https://code.visualstudio.com/).

### 2. **Installer l'extension Python dans VS Code**
   - Ouvre VS Code.
   - Clique sur l'icône des extensions sur le côté gauche de la fenêtre (l'icône avec des carrés).
   - Rechercher "Python" et installe l'extension Python officielle de Microsoft.

### 3. **Configurer l'environnement Python**
   - Ouvre ton fichier Python dans VS Code (`.py`).
   - En bas à gauche, tu verras la version de Python actuellement sélectionnée. Assure-toi que c'est la bonne version (celle que tu as installée).
   - Si la version est incorrecte, clique dessus pour sélectionner le bon interpréteur Python.

### 4. **Ajouter une configuration de débogage**
   - Dans la barre latérale gauche, clique sur l'icône du débogueur (icône de lecture avec un insecte).
   - Clique sur le bouton `Run and Debug` ou sur le lien `create a launch.json file` si tu ne l'as pas encore fait.
   - Sélectionne `Python` comme environnement de débogage.
   - Un fichier `launch.json` sera généré dans un dossier `.vscode` à la racine de ton projet.

### 5. **Points d'arrêt (Breakpoints)**
   - Ouvre ton fichier `.py` dans l'éditeur.
   - Clique à gauche du numéro de ligne dans le fichier pour ajouter un point d'arrêt. Ce point d'arrêt stoppera l'exécution du programme à cette ligne, te permettant d'inspecter les variables.

### 6. **Lancer le débogage**
   - Une fois tes points d'arrêt ajoutés, clique sur le bouton vert `Run` ou sur l'icône `Start Debugging` (ou utilise le raccourci `F5`).
   - Le programme s'arrêtera aux points d'arrêt, te permettant de vérifier les valeurs des variables à ce moment de l'exécution.

### 7. **Inspecter les variables**
   - Dans le panneau de débogage à gauche, tu verras une section `Variables` qui te permet de voir les valeurs de toutes les variables locales et globales.
   - Tu peux également survoler une variable avec la souris dans l'éditeur pour voir sa valeur actuelle.

### 8. **Contrôles de débogage**
   - Pendant le débogage, tu peux utiliser les boutons en haut de l'écran :
     - **Continue** (F5) : continue l'exécution jusqu'au prochain point d'arrêt.
     - **Step Over** (F10) : exécute la ligne actuelle et passe à la suivante sans entrer dans les fonctions.
     - **Step Into** (F11) : entre dans une fonction appelée à la ligne actuelle.
     - **Step Out** (Shift + F11) : sort de la fonction actuelle et revient à l'appelant.

### 9. **Console de débogage**
   - Tu peux aussi utiliser la console de débogage en bas de l'interface pour évaluer des expressions et inspecter des valeurs pendant que le programme est en pause.

### Exemple de configuration dans `launch.json` :
```json
{
    "version": "0.2.0",
    "configurations": [
        {
            "name": "Python: Déboguer le fichier actuel",
            "type": "python",
            "request": "launch",
            "program": "${file}",
            "console": "integratedTerminal"
        }
    ]
}
```

### 10. **Lancer le programme sans points d'arrêt**
   - Si tu souhaites exécuter le programme sans débogage, clique sur `Run` dans le menu en haut puis sur `Run Without Debugging` (raccourci `Ctrl + F5`).

Maintenant, tu devrais être prêt à déboguer ton programme Python dans VS Code. N'hésite pas à ajouter des points d'arrêt et à explorer les variables pour mieux comprendre le comportement de ton code.