# Labo de Phy3

## Marche à suivre

Avant de modifier le `.md` executer la commande :

```bash
git pull .
```
Après avoir travailler sur le document executer la commande

```bash
git add .
git commit -am "expliquer les modifs entre les guillemets"
git push
``` 

## Syntaxe Markdown

```md
# Titre
## Sous section 1
### Sous section 2
...
```
Exemples :
# Titre
## Sous section 1
### Sous section 2

Nouvelle page ou nouvelle ligne :
```latex
\newpage
\newline
```

Integrer une image :

```md
![texte de la figure](chemin de l'image, dans nos labos c'est : images/nom-de-limage.png)
```

## Syntaxe *latex* pour les formules

### Formules

Pour les formules à gauche ou dans du texte entre $ formule $ et pour des formules centrées $$ formules $$

Exemple :

$f(x) = x^2 +5x +8$

$$f(x) = x^2 +5x +8$$

### Commandes pour caractères spéciaux

Pour faire une barre de fraction ou utiliser des lettres grecques, il faut avoir recours a certaine commande toujours precedée d'un "\"

```latex
$1 = fraction = \dfrac{au dessus de la fraction}{au dessous de la fraction}$

$2 = F_{indice}$

$3 = \sqrt{racine carrée}

$4 = x^{puissance}

$5 = \pi * \omega$
```


