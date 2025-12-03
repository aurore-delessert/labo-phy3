---
header-includes:
  - \usepackage[a4paper, top=2cm, bottom=2cm, left=1.5cm, right=1.5cm]{geometry}
  - \usepackage{fancyhdr}
  - \pagestyle{fancy}
  - \fancyhead[L]{Aurore Delessert \newline Magali Tornare}
  - \fancyhead[R]{Phy3-Labo 02}
  - \fancyfoot[C]{Page \thepage}
  - \usepackage{graphicx}
---

\includegraphics[width=0.25\textwidth]{images/heig-logo.png}

\thispagestyle{empty}
\begin{center}
\vspace*{3cm}

\noindent\rule{\textwidth}{0.4pt}\\[0.6cm]

{\Huge \textbf{Labo 02}}\\[0.5cm]
{\LARGE \textit{Canon à électrons}}\\[0.3cm]
\noindent\rule{\textwidth}{0.4pt}\\[1.5cm]

{\Large \textbf{Aurore Delessert, Magali Tornare}}\\
Physique — HEIG-VD\\[1.5cm]

\textbf{Date du laboratoire :} 17 octobre 2025\\
\textbf{Professeure :} A-G Pawlowski\\
\textbf{Salle de classe :} T06\\[3cm]

\vfill
\end{center}

\clearpage
\setcounter{page}{1}

\tableofcontents

\newpage

## Introduction

![canon à électrons](images/intro-image.png)

Des faisceaux d’électrons sont aujourd’hui beaucoup utilisés industriellement, par exemple pour la gravure de microstructures pour la microélectronique ou pour le soudage ou l’impression 3D par faisceau d’électrons. Ces applications sont récentes, d’autres exemples plus traditionnels d’application de faisceaux à électrons se trouvent dans des sources à rayons X pour l’imagerie médicale ou dans des microscopes électroniques pour l’analyse de matériaux, mais aussi dans des oscilloscopes ou télévisions traditionnelles qui utilisent des faisceaux d’électrons pour l’affichage d’un signal électrique ou d’une image.

Ces instruments et applications se basent sur la déviation d’un faisceau d’électrons dans des champs électriques et magnétiques. Ces systèmes contiennent donc un canon à électrons (tube cathodique) pour générer le faisceau d’électrons et utilisent des champs électriques et magnétiques pour le dévier.

Le système d’expérimentation “oscilloscope didactique” du laboratoire PHY3 permet d’étudier la déviation d’un faisceau d’électrons par des champs électriques et magnétiques. De plus, un balayage contrôlé du faisceau à l’aide de signaux périodiques peut être étudié, ainsi que la représentation à résolution temporelle de signaux électriques sur un écran fluorescent, telle que réalisée dans des oscilloscopes traditionnels.
Le faisceau est généré et focalisé sous vide dans un tube cathodique (dit aussi tube de Braun). Le point d’impact des électrons peut être observé sur un écran fluorescent sous la forme d’une tâche lumineuse verte.

- Afin d’observer également le tracé de la trajectoire du faisceau, on peut obscurcir le système, par exemple à l’aide d’un grand carton. La trajectoire du faisceau des électrons est visible grâce à l’ionisation d’un gaz résiduel (ici néon) par lequel le tube à vide avait été rempli à faible pression (les électrons qui entrent en collision avec des molécules du gaz, les excitent et on observe ensuite la lumière qui est émise par les atomes du gaz).
- Un champ électrique axiale appliqué à l’intérieure de la partie tube cathodique (entre la cathode et l’anode) permet l’accélération des électrons qui sont libérés par la cathode (chauffée à l’aide d’un filament) et ainsi de régler la vitesse des électrons.
- Un champ électrique latérale et orienté horizontalement (entre deux plaques d’un condensateur à plaques parallèles) permet une déviation et balayage horizontal du faisceau, à l’aide d’une tension à dents de scie (le faisceau d’électrons se déplace ainsi à vitesse constante de gauche à droite pour revenir d’un saut à son point d’origine ; le processus se répète de manière périodique avec une fréquence réglable).
- Des champs magnétiques, orientés perpendiculairement par rapport au faisceau d’électrons, peuvent également dévier le faisceau. Pour générer les champs magnétiques des bobines électriques sont utilisées et peuvent être placées sous différents angles à l’extérieur du tube à vide, sur une armature circulaire et concentrique autour de l’axe du tube cathodique, afin d’étudier la déviation du faisceau de manière contrôlée en fonction de l’alimentation des bobines et de la vitesse des électrons.
Lorsque l’on choisit l’emplacement d’une bobine telle que la déviation du faisceau d’électrons par le champ magnétique résulte le long l’axe verticale, on peut alimenter la bobine avec un signal électrique que l’on souhaite représenter en fonction du temps, simultanément à un balayage horizontal du faisceau, et ainsi rendre visible le signal électrique sur l’écran fluorescent comme sur un oscilloscope.


## Partie théorique

### Rappel des formules

#### Bobine (solénoïde)

![solénoïde](images/solenoide.png)

Champs d'induction magnétique créé par une bobine :

$$B = \dfrac{{\mu}_{0} N I}{L} [T]  (1)$$

Avec : $\begin{cases} \mu_{0} = 4 \pi \times 10^{-7} [Vs/Am] \\ N = \text{nombre de spires} \\ I = \text{courant traversant la bobine} [A] \\ L = \text{longueur de la bobine} [m] \end{cases}$

#### Force de Lorentz

Force exercée sur une particule chargée en mouvement dans un champ magnétique :

$$\vec{F} = q(\vec{E} + \vec{v} \times \vec{B}) [N]  (2)$$

Avec : $\begin{cases} q = \text{charge de la particule} [C] \\ \vec{E} = \text{champ électrique} [V/m] \\ \vec{v} = \text{vitesse de la particule} [m/s] \\ \vec{B} = \text{champ magnétique} [T] \end{cases}$