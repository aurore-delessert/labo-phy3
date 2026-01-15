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

$$v = \sqrt{\frac{1}{\rho \cdot \kappa}} \quad \text{avec } \rho~[\text{kg/m}^3],\ \kappa~[\text{Pa}^{-1}]$$\
où $\rho$ est la masse volumique du milieu et $\kappa$ sa compressibilité.

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

\newpage

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

\newpage

### Montage expérimental

Le montage principal repose sur une cuve à faces parallèle remplie de différents liquides (eau distillée, ethanole et glycérine), qui est fixée sur un banc d'optique. Un quartz émetteur (QE) est placé contre une des parois étroites (donc à une extrémité de la cuve) avec une pâte silicone entre elle et la parois afin que le contact avec la cuve se fasse le mieux possible. Un quartz recepteur (QR) est immergé verticalement dans le liquide et peut être déplacé horizontalement grâce à un cavalier d'optique.

![Croquis de la cuve avec QE et QR ](images/Montage_schéma_Cuve_QR_QE.png)

Sur l'image ci-dessous, on peut voir :

- En jaune la cuve qui contiendra les différents liquides
- En rouge, l'oscilloscope permettant de mesurer les 2 signaux générés par QE et QR
- En vert, le générateur d'ultrasons pour QE
- En bleu, l'appareil permetant de mesurer la fréquence générée par le générateur d'ultrasons

![Photo du montage](images/Image_Montage.png){ width=500px }

Le principe de fonctionnement de ce montage repose sur la piézoélectricité du quartz. En effet, lorsqu'un champ électrique alternatif est appliqué au QE, ce dernier vibre mécaniquement à la fréquence du signal, ce qui génère une onde ultrasonore dans le liquide. Le QR sera donc soumis à cette onde et produira un signal électrique proportionnel à la pression accoustique reçue.

### 1e manipulation : Mesure de la vitesse de phase dans différents liquides

Pour la première manipulation, nous avons éxecuter 3 fois la même mesure, soit une fois pour chaque liquide. Cette mesure consiste à :

1. Trouver une distance pour laquelle les 2 signaux de QE et QR sont supperposés comme sur l'image ci-dessous :

2. On translate une fois encore QR jusqu'à trouver à nouveau les 2 signaux superposé. Cela signifie que nous avons parcouru une longueur d'onde, ce qui nous permet de calculer le $\lambda$.

![Superposition de QE et QR](images/QE_et_QR.png){ width=300px }

Voici le tableau de des différentes distances et fréquences que nous avons mesurées :

| Liquide        | x1 [mm] | x2 [mm] | fréquence [Hz] |
|----------------|---------|---------|----------------|
| Eau distillée  | 1,81    | 3,64    |     816'600    |
| Glycérine      | 2,14    | 4,49    |     817'800    |
| Éthanol        | 4,69    | 6,10    |     818'000    |

### Dans la vie de tous les jours

Dans la vie de tous les jours, on retrouve propagation d'une onde avec la vitesse de phase dans pas mal de cas, comme par exemple :

- Les échographies médicales :
Dans les échographies (en mode continu), aussi appelée échographie Doppler, on envoie une onde presque continue dans le corps pour mesurer la vitesse de sang. La vitesse de phase est essentielle pour calculer le décalage Doppler, déterminer la vitesse du flux sanguin et calibrer l'appareil pour que les distances soient correctent.

- Sonar et navigation sous-marine :

![Sonar marin](images/Image_bateau_sonar.png){ width=300px }

Les sonars utilisent uniquement des ondes continues pour : détecter des potentiels obstacles, mesurer la profondeur actuelle et cartographier les fonds marins. La vitesse de phase dans l'eau, qui est estimée à 1500 m/s, est un paramètre fondamental pour convertir le temps de propagation en distance.

- Contrôle industriel : Epaisseur de matériaux
Dans certaines industries, on envoie une onde ultrasonore continue dans un matériau pour mesurer : L'épaisseur d'une plaque, la présence potentielle de défauts internes et la qualité d'une soudure.
La vitesse de phase dans le matériau doit être connue afin que la plécision pour la mesure soit fiable.

### Calculs & Analyse des résultats

Avec le tableau des résultats représenté ci-dessus, nous pouvons maintenant calculer le $\lambda$ et les incertitudes.

Voici le tableau des résultats :

| Liquide        | $\lambda$ [mm] | $\lambda$ [m] | $\Delta \lambda$[mm] | $\Delta f$ [Hz] | v [m/s] | $\Delta v$ [m/s] |
|----------------|----------------|---------------|----------------------|-----------------|---------|------------------|
| Eau distillée  |      1,83      |    0,00183    | 0,7 * $10^{-3}$      |        5        |  1'496  |   577            |
| Glycérine      |      2,35      |    0,00235    | 0,7 * $10^{-3}$      |        5        |  1'922  |   578            |
| Éthanol        |      1,45      |    0,00145    | 0,7 * $10^{-3}$      |        5        |  1'186  |   578            |

Pour l'analyse des résultats obtenus, nous pouvons voir que les incertitudes sont énormes. Cela est lié au fait que nous avions beaucoup de problème pour lire correctemen correctement les valeurs des positions car le système de mesure était peu stable et surtout difficile à lire.

Concernant les valeurs de la vitesse de propagation trouvée, nous remarquons que ces dernières sont très près des valeurs données par la consigne. Voici un tableau qui les compare :

Comme la vitesse donnée est entre 20°C et 25°C, nous avons pris la moyenne entre les 2 valeurs afin de retrouver une valeur à approximativement 22°C.
Sachant que $v_i$ est la valeur numérique donnée dans la notice du laboratoire.

| Liquide        |      $v_i$ [m/s] |  v [m/s] |      $v_i$ - v [m/s]| erreur en [%] |
|----------------|------------------|----------|---------------------|---------------|
| Eau distillée  |      1'497       |  1'496   |         -1          |     -0,66     |
| Glycérine      |      1'914       |  1'922   |         -8          |     -0,42     |
| Éthanol        |      1'194       |  1'186   |          8          |      0,67     |

Comme pour chaque mesure, nous avons une erreur qui se trouve en dessous de $\pm$ 1%, nous sommes satisfaite de nos mesures.
Bien sûr comme nous ne sommes pas sûre que la température du laboratoire au moment où nous avons fait nos expériences, nous ne pouvons pas être sûre que toutes les mesures sont correctes mais du moins, elles se rapprochent de la valeur voulue.

### 2e Manipulation : Mesure de la vitesse de groupe dans l'eau distillé

### Introduction manip 2

Pour cette deuxième partie de l'expérience, nous devions mesurer la vitesse de groupe des ultrasons dans l'eau distilée à l'aide du montage émetteur-récepteur. Contrairement à la vitesse de phase, qui caractérise la propagation d'une onde sinusoïdale infinie, la vitesse de groupe correspond à la vitesse de propagation d'un paquet d'onde, c'est-à-dire d'un signal de durée finie.

Dans notre cas, le quartz émetteur (QE) peut fontionner en régime impulsionnel. Il envoie donc des impulsions acoustiques brèves, qui se répètent à environ 1kHz. Le quartz récepteur (QR) détecte les impulsions après la propagation dans le liquide.

Normalement, comme nous sommes dans un milieu homogène et non dispersif, nous devrions retrouver à peu près la même vitesse que nous avons calculée pour la vitesse de phase.

### Dans la vie de tous les jours manip 2

Pour ces exemples de la vie courante, nous allons reprendre les 2 premiers exemples pris pour la première manipulation. Soit :

- Les échogrpahies médicales :

![Echographie explications](images/exemple_echographie.png){ width=300px }

Dans les échographies médicales, il existe un autre mode d'utilisation qui est le mode impulsionnel. Les échographies classiques qui donnent des imageries 2D, fonctionnent en envoyant des impulsions utlrasonores dans le corps. La vitesse de groupe est donc utilisée pour déterminer la profondeur d'un organe, reconstruire une image en temps réel ou localiser avec précision les interfaces (soit les os, muscles ou les organes). C'est une méthode qui permet une meilleure précision sur un point / endroit bien précis. Si l'image de groupe n'est pas connue, l'image serait déformée. Déformée car un échographe reconstruit toute la géométrie interne du coprs seulement à partir du temps que mettent les impulsions ultrasonores à revenir.

- Les radars :

- ![Radar d'un bateau](images/Image_bateau_radar.jpg){ width=300px }

Dans les radars, on utilise le même principe que pour les échographies mais avec des ondes électromagnétiques. Les radars vont envoyer des impulsions pour mesurer la distance d'un avion, la vitesse d'une voiture ou encore la position d'un drône. La vitesse de groupe est utilisée pour convertir un temps de retour en distance.

- La télécommunication (la fibre optique) :
Dans la fibre optique, les signaux sont envoyés sous forme de pleins d'impulsions lumineuses. La vitesse de groupe va déterminer le temps de propagation du signal, la latence d'internet ou encore la dispersion des impulsions (qui déterminent le limite du débit maximale).
Cet exemple est parfait car c'est un milieu dispersif, contrairement au liquide de notre expérience.

### Calculs & Analyse des résultats manip 2

Pour pouvoir montrer la propagation dans le liquide, dans notre car l'eau distillée, voici une image de nos mesures :

![Vitesse de groupe : QE et QR](images/QE_et_QR_Vitesse_De_Groupe.png){ width=300px }

Voici le tableau indiquant les résultats des calculs effectués.

|$\Delta x$      | $\Delta t$ [s] |$\Delta v_g$ [s] |
|----------------|----------------|-----------------|
|0,7 * $10^{-3}$ |    0,028       |       0, 36     |

| Liquide        | x1 [mm] | x2 [mm] |     t1 [s]   |   t2 [s]     | x [mm] |    t [s]    | $v_g$ [m/s] |
|----------------|---------|---------|--------------|--------------|--------|-------------|-------------|
| Eau distillée  | 0,0706  | 0,0806  |$56,7*10^{-6}$| $50*10^{-6}$ | 0,01   |$7,7*10^{-6}$|     1'493   |

Comme dans la théorie nous avions souligné le fait d'être dans un milieu non dispersif, nous allons le vérifier en comparant cette valeur obtenue avec la valeur donnée dans la notice du laboratoire.

Voici le tableau comparatif :

| Liquide        |      $v_i$ [m/s] |  $v_g$ [m/s] |    $v_i - v_g$ [m/s]| erreur en [%] |
|----------------|------------------|--------------|---------------------|---------------|
| Eau distillée  |      1'497       |    1'493     |         4           |     0,27      |

Nous constatons donc que la valeur trouvée pour la vitesse de groupe est très proche de celle donnée dans la notice. Nous nous trouvons donc bel et bien dans un milieu non dispersif.

### Conclusion

Récapitulons les résultats de la première manipulation.

Nous avons eu un gros porblème avec les valeurs de l'incertitude de $\Delta v$ qui vaut le 30% de la valeur mesurée lors du laboratoire. Cet écart est directement lié au fait que nous avons eu des difficultés à mesurer précisement la distance x ce qui a augmenté grandement la valeur de $\Delta \lambda$. Le fait que la variation de distance soit très faible et que l'incertitude de la mesure soit grande, cela pose un problème.

Au niveau des valeurs mesurées, nous avons obtenu des résultats qui se rapprochent grandement des valeurs de la consigne du laboratoire. Cela confirme que nous avons effectué correctement les mesures et que les valeurs mesurées sont correctes. Comme nous pouvons le voir, chaque écart entre la valeur donnée et la valeur mesurée est très faible.

Résultats de la vitesse de phase

| Liquide        | $\lambda$ [mm] | f [Hz]     | v = f·$\lambda$ [m/s]  | v_tab [m/s] | Écart [%] |
|----------------|----------------|------------|------------------------|-------------|-----------|
| Eau distillée  | 1.83           | 816600     | 1496                   | 1497        | -0.07     |
| Glycérine      | 2.35           | 817800     | 1922                   | 1914        | +0.42     |
| Éthanol        | 1.45           | 818000     | 1186                   | 1194        | -0.67     |

Maintenant, récapitulons les résultats de la deuxième manipulation.

C'était une manipulation qui pouvait nous faire visualiser plus en détail et surtout plus facilement la vitesse de propagation dans un liquide. Nous avons aussi vu que il y avait une grande différence entre le signal émit et celui qui est reçu. Notre objectif était de pouvoir calculer la vitesse de groupe.
Pour les résultats de nos mesures, nous avons retrouvé une valeur de vitesse de groupe très proche de celle de la vitesse de phase, ce qui confirme le fait que nous sommes dans un milieu non dispersif. Au niveau des écarts, nous sommes en dessous de 1% ce qui reste très bien.

Résultats de la vitesse de groupe :

| Liquide        |      $v_i$ [m/s] |  $v_g$ [m/s] |    $v_i - v_g$ [m/s]| erreur en [%] |
|----------------|------------------|--------------|---------------------|---------------|
| Eau distillée  |      1'497       |    1'493     |         4           |     0,27      |

Globalement, nous pouvons donc dire que nous avons réussit à prouver les valeurs théoriques grâce à nos mesures.
Comme sythèse, nous pouvons souligner :

- Les vitesses de phase mesurées dans trois liquides sont toutes à moins de 1 % des valeurs tabulées.
- La vitesse de groupe mesurée dans l’eau distillée est pratiquement identique à la vitesse de phase.
- Les incertitudes sur $\lambda$ dominent l’erreur dans la première manipulation.
- L’eau se comporte comme un milieu non dispersif pour les ultrasons autour de 800 kHz.
