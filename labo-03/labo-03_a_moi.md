---
header-includes:
  - \usepackage[a4paper, top=2cm, bottom=2cm, left=1.5cm, right=1.5cm]{geometry}
  - \usepackage{fancyhdr}
  - \pagestyle{fancy}
  - \fancyhead[L]{Aurore Delessert \newline Magali Tornare}
  - \fancyhead[R]{Phy3-Labo 02}
  - \fancyfoot[C]{Page \thepage}
  - \usepackage{graphicx}
  - \usepackage{tikz}
  - \usepackage{pgfplots}
  - \pgfplotsset{compat=newest}
  - \usetikzlibrary{arrows.meta}
  - \usepackage{amsmath}
  - \usepackage{capt-of}
  - \usepackage{booktabs}
---

\includegraphics[width=0.25\textwidth]{images/heig-logo.png}

\thispagestyle{empty}
\begin{center}
\vspace*{3cm}

\noindent\rule{\textwidth}{0.4pt}\\[0.6cm]

{\Huge \textbf{Labo 03}}\\[0.5cm]
{\LARGE \textit{Projet sur la propagation des ondes}}\\[0.3cm]
\noindent\rule{\textwidth}{0.4pt}\\[1.5cm]

\begin{center}
\includegraphics[width=\textwidth]{images/Page_de_garde.png} \end{center}

{\Large \textbf{Aurore Delessert, Magali Tornare}}\\
Physique — HEIG-VD\\[1.5cm]

\textbf{Date du laboratoire :} 12 décembre 2025\\
\textbf{Professeure :} Dre Anne-Gabrielle Pawlowski\\
\textbf{Salle de classe :} T06\\[3cm]

\vfill
\end{center}

\clearpage
\setcounter{page}{1}

\tableofcontents

\newpage

## Experience 1: Propagation des ondes ultrasonores dans des milieux liquides

### Introduction

Les ondes acoustiques, qu’est-ce que c’est ?

Une onde acoustique est une perturbation de pression qui se propage dans un milieu fluide/liquide.

Parmi les perturbations sonores, nous retrouvons les ultrasons qui sont des ondes sonores dont la fréquence dépasse les 20kHz, ce qui rend leur perception impossible à entendre par l’oreille humaine. La génération des ondes ultrasonores repose sur un phénomène physique qui est la piézoélectricité. Certains cristaux, comme le quartz par exemple, présentent cette propriété et permettent de convertir une contrainte mécanique en signal électrique et vice-versa.

![La constitution du quartz](images/Quartz.png)

En effet, le quartz a une structure très spéciale car il n’a pas un centre symétrique, ce qui permet l’apparition d’une polarisation électrique lorsque ce dernier est soumis à une certaine contrainte mécanique. Cette polarisation génère une tension mesurable entre des électrodes.

Comme dis précédemment, ce phénomène est réversible. En appliquant une tension alternative, le cristal entre en vibration à la fréquence du signal. Si cette fréquence est la même que la fréquence du signal, un effet de résonnance se produit et amplifie les vibrations. Ce mécanisme est à la base de la génération des ultrasons dans notre montage.

### Objectifs de l'expérience

L’expérience vise principalement à :  
\begin{itemize}
\item Observer la propagation d’une onde acoustique dans un liquide
\item Mesurer la célérité (donc la vitesse de phase) d’une onde générée dans différents liquides.
\item Mesurer la célérité en groupe (vitesse de groupe d’une onde générée dans un liquide et comparer cette vitesse avec celle de phase.
\end{itemize}

Comme il était demandé d’analyser la vitesse de groupe mais que nous l’avions déjà fait dans un précédent rapport, nous allons essayer de tirer des parallèles entres ces 2 expériences.

### Rappels théoriques

La vitesse de propagation d’une onde acoustique dans un liquide, appelée célérité ou vitesse de phase, dépend de la fréquence de l’onde et de sa longueur d’onde. Pour une onde sinusoïdale, on peut calculer la vitesse avec la formule suivante :

$$v = f \cdot \lambda \quad \text{avec } v~[\text{m/s}],\ f~[\text{Hz}],\ \lambda~[\text{m}]$$

Avec lambda qui vaut $$\lambda = x_2 - x_1 \quad \text{avec} \quad x_1~[\text{mm}],\ x_2~[\text{mm}],\ \lambda~[\text{mm}]$$

La vitesse peut aussi dépendre des propriétés mécaniques du milieu dans lequel l’onde se propage. Dans ce cas, la formule devient :

$$v = \sqrt{\frac{1}{\rho \cdot \kappa}} \quad \text{avec } \rho~[\text{kg/m}^3],\ \kappa~[\text{Pa}^{-1}]$$\\
textit{où } $\rho$ est la masse volumique du milieu et $\kappa$ sa compressibilité.

Cette formule dépend donc directement les propriétés mécaniques du milieu, en particulier de :

- La compressibilisé $\kappa$ du liquide qui est sa capacité à se comprimer.
- Sa dentisé $\rho$

Chaque liquide possède donc un combinaison différente de densité de compressibilité et de densité. Cela explique pourquoi la célérité varie en fonction du milieu dans lequel elle se propage.

Dans la donnée, on nous donnait le tableau suivant :

![Tableau avec valeurs tabulées](images/Tableau_Val_Vitesse_Liquide.png){width=500px}

En théorie, la vitesse de groupe est définie par :

$$ v_p = \frac{\omega}{k} $$
Avec :

$\omega$ est la **pulsation** de l’onde (en rad/s),
$\kappa$ est le **nombre d’onde** (en rad/m).

Cependant, dans notre car, nous ne pouvons pas mesurer directement $\omega$ ou $\kappa$. Alors on va mesurer la propagation d'un paquet d'onde (impulsion) entre deux positions. On transforme donc la formule comme suit :

On sait que :
$$ \omega = 2\pi f $$
$$ \kappa = \frac{2\pi}{\lambda} $$

On remplace donc dans la formule :
$$ v_p = \frac{2\pi f}{\frac{2\pi}{\lambda}} $$

Et en simplifiant, on trouve :
$$ v_p = f \lambda $$

$$ v_g = \frac{\Delta x}{\Delta t} = \frac{x}{t}$$
où $x = x_2 - x_1$ est le déplacement de QR et $t = t_2 - t_1$ la différence de période.

Dans un milieu peu dispersif (comme l'eau distillée ou l'alcool) la vitesse de groupe est à peu près égal à la vitesse de phase.

### Incertitudes

Pour la vitesse de phase :

En supposant que la fréquence (f) et la longueur d’onde ($\lambda$) sont indépendantes,
l’incertitude sur la vitesse (v) est donnée par :
$$
\Delta v = \sqrt{
\left(\frac{\partial v}{\partial f} \, \Delta f\right)^2
+
\left(\frac{\partial v}{\partial \lambda} \, \Delta \lambda\right)^2
}
\quad \text{avec} \quad
\Delta v~[\text{m·s}^{-1}]
$$

Les dérivées partielles donnent :

À partir de (v = f $\lambda$), on obtient :
$$
\frac{\partial v}{\partial f} = \lambda
\quad [\text{m}]
\qquad \text{et} \qquad
\frac{\partial v}{\partial \lambda} = f
\quad [\text{Hz}]
$$

Comme $x_1$ et $x_2$ sont indépendantes, l’incertitude sur la longueur d’onde est :
$$
\Delta \lambda = \sqrt{(\Delta x_1)^2 + (\Delta x_2)^2}
\quad \text{avec} \quad
\Delta x_1~[\text{mm}],\
\Delta x_2~[\text{mm}]
$$

Ainsi, l’incertitude sur la célérité du son s’écrit :
$$
\Delta v = \sqrt{(\lambda \, \Delta f)^2 + (f \, \Delta \lambda)^2}
\quad \text{avec} \quad
\Delta f~[\text{Hz}],\
\Delta \lambda~[\text{m}]
$$

Après réflexion, nous avons pris la décision de mettre :
$$
\Delta x_1 = \pm 0,5 [mm]\space
\Delta x_2 = \pm 0,5 [mm]\space
\Delta f = \pm 5 [Hz]
$$

Pour la vitesse de groupe :

La formule de l'incertitude globale non simplifiée donne :

$$ \Delta {v_g} = \sqrt{ \left(\frac{\partial v_g}{\partial x} \Delta x \right)^2 + \left(\frac{\partial v_g}{\partial t} \Delta t \right)^2 } $$

Avec les dérivées partielles :

$$ \frac{\partial v_g}{\partial x} = \frac{1}{\Delta t} $$
$$ \frac{\partial v_g}{\partial t} = -\frac{\Delta x}{(\Delta t)^2} $$

Les incertitudes sur le déplacement et sur la différence de période donne :
$$ \Delta x = \sqrt{(\Delta x_2)^2 + (\Delta x_1)^2} $$
$$ \Delta t = \sqrt{(\Delta t_2)^2 + (\Delta t_1)^2} $$

Après réflexion, nous avons pris la décision de mettre :
$$ \Delta x_1 = \Delta x_2 = \pm 0{,}5 \,\text{mm} $$
$$ \Delta t_1 = \Delta t_2 = \pm 0{,}2 \,\mu s $$

Au final, la formule pour l'incertitude sur $v_g$ donne :
$$ \Delta{v_g} = \sqrt{ \left(\frac{\Delta x}{\Delta t}\right)^2 + \left(\frac{\Delta x}{(\Delta t)^2} \Delta t \right)^2 } $$

### Montage expérimental

![Croquis de la cuve avec QE et QR ](images/Montage_schéma_Cuve_QR_QE.png)

Le montage principal repose sur une cuve à faces parallèle remplie de différents liquides (eau distillée, ethanole et glycérine), qui est fixée sur un banc d'optique. Un quartz émetteur (QE) est placé contre une des parois étroites (donc à une extrémité de la cuve) avec une pâte silicone entre elle et la parois afin que le contact avec la cuve se fasse le mieux possible. Un quartz recepteur (QR) est immergé verticalement dans le liquide et peut être déplacé horizontalement grâce à un cavalier d'optique.

![Photo du montage](images/Image_Montage.png){ width=500px }  

Sur l'image ci-dessus, on peut voir :

- En jaune la cuve qui contiendra les différents liquides
- En rouge, l'oscilloscope permettant de mesurer les 2 signaux générés par QE et QR
- En vert, le générateur d'ultrasons pour QE
- En bleu, l'appareil permetant de mesurer la fréquence générée par le générateur d'ultrasons

Le principe de fonctionnement de ce montage repose sur la piézoélectricité du quartz. En effet, lorsqu'un champ électrique alternatif est appliqué au QE, ce dernier vibre mécaniquement à la fréquence du signal, ce qui génère une onde ultrasonore dans le liquide. Le QR sera donc soumis à cette onde et produira un signal électrique proportionnel à la pression accoustique reçue.

### 1e manipulation : Mesure de la vitesse de phase dans différents liquides

Pour la première manipulation, nous avons éxecuter 3 fois la même mesure, soit une fois pour chaque liquide. Cette mesure consiste à :

1. Trouver une distance pour laquelle les 2 signaux de QE et QR sont supperposés comme sur l'image ci-dessous :

![Superposition de QE et QR](images/QE_et_QR.png){ width=300px }

2. On translate une fois encore QR jusqu'à trouver à nouveau les 2 signaux superposé. Cela signifie que nous avons parcouru une longueur d'onde, ce qui nous permet de calculer le $\lambda$.

Voici le tableau de des différentes distances et fréquences que nous avons mesurées :

| Liquide        | x1 [mm] | x2 [mm] | fréquence [Hz] |
|----------------|---------|---------|----------------|
| Eau distillée  | 1,81    | 3,64    |     816'600    |
| Glycérine      | 2,14    | 4,49    |     817'800    |
| Éthanol        | 4,69    | 6,10    |     818'000    |

### Calculs & Analyse des résultats

Avec le tableau des résultats représenté ci-dessus, nous pouvons maintenant calculer le $\lambda$ et les incertitudes.

Voici le tableau des résultats :

| Liquide        | $\lambda$ [mm] | $\lambda$ [m] | $\Delta \lambda$[mm] | v [m/s] | $\Delta v$ [m/s] |
|----------------|----------------|---------------|----------------------|---------|------------------|
| Eau distillée  |      1,83      |    0,00183    | 0,7 * $10^{-3}$      |  1'496  |   577            |
| Glycérine      |      2,35      |    0,00235    | 0,7 * $10^{-3}$      |  1'922  |   578            |
| Éthanol        |      1,45      |    0,00145    | 0,7 * $10^{-3}$      |  1'186  |   578            |

Pour l'analyse des résultats obtenus, nous pouvons voir que les incertitudes sont énormes. Cela est lié au fait que nous avions beaucoup de problème pour lire correctement.

### 2e Manipulation : Mesure de la vitesse de groupe dans l'eau distillé

### Introduction manip 2

Pour cette deuxième partie de l'expérience, nous devions mesurer la vitesse de groupe des ultrasons dans l'eau distilée à l'aide du montage émetteur-récepteur. Contrairement à la vitesse de phase, qui caractérise la propagation d'une onde sinusoïdale infinie, la vitesse de groupe correspond à la vitesse de propagation d'un paquet d'onde, c'est-à-dire d'un signal de durée finie.

Dans notre cas, le quartz émetteur (QE) peut fontionner en régime impulsionnel. Il envoie donc des impulsion acoustiques brèves, qui se répète à environ 1kHz. Le quartz récepteur (QR) détecte les impulsions après la propagation dans le liquide.

Normalement, comme nous sommes dans un milieu homogène et non dispersif, nous devrions retrouver à peu près la même vitesse que nous avons calculée pour la vitesse de phase.
