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
\textbf{Professeure :} Dr Anne-Gabrielle Pawlowski\\
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

## Matériel utilisé & Caractéristiques techniques
Tout au long de notre laboratoire, nous allons utiliser le matériel suivant : 

  - Le canon à électron montré en figure 1 
  - Un écran fluorescent affichant à l'aide d'un point vert l'endroit de l'impact du faisceau à électron. 
  - 2 Multimètres qui nous serviront à mesurer la tension et le courant dans le montage. 
  - 3 Bobines 
  - Une alimentation spécifique pour le laboratoire. 

Pour parler un peu plus en détails des caractéristiques techniques à prendre en compte :

- Une tension anodique ($U_a$) que nous devions choisir entre 200 et 350 Vcc. Nous avons pris 250 $\pm$ 2 Vcc. 
- Un courant anodique de maximum 1 mA.
- une tension de chauffage entre 6 et 12 V
- Une tension en dents de scie de 100 V avec une fréquence entre 3,5 et 650 Hz.
- Des bobines de déviation qui ont soit 300 ou 600 spires, avec une résistance interne de 4,2 $\Omega$ et impédance de 6 mH.

Pour le module de commande, le voici :

![module de commande](images/Module-commande.png)

Avec:
\begin{itemize}
\item A : Anode
\item C : Cathode
\item H : Chauffage
\item W : Cylindre Wehnelt
\item PE : Terre de protection
\item $U_+$ : Electrode de déviation droite
\item $U_-$ : Electrode de déviation gauche
\end{itemize}

\newpage

## Partie théorique

### Rappel des formules

#### Bobine (solénoïde)

![solénoïde](images/solenoide.png)

Champs d'induction magnétique créé par une bobine :

$$B = \dfrac{{\mu}_{0} N I}{L} [T]    (1)$$

Avec : $\begin{cases} \mu_{0} = 4 \pi \times 10^{-7} [Vs/Am] \\ N = \text{nombre de spires} \\ I = \text{courant traversant la bobine} [A] \\ L = \text{longueur de la bobine} [m] \end{cases}$

#### Force de Lorentz

Force exercée sur une particule chargée en mouvement dans un champ magnétique :

$$\vec{F} = q(\vec{E} + \vec{v} \times \vec{B}) [N]   (2)$$

Avec : $\begin{cases} q = \text{charge de la particule} [C] \\ \vec{E} = \text{champ électrique} [V/m] \\ \vec{v} = \text{vitesse de la particule} [m/s] \\ \vec{B} = \text{champ magnétique} [T] \end{cases}$

\newpage

## 1. Expérience 1 - Faisceau d'électron (Canon à électrons)

### 1.0 Introduction

Cette expérience a pour but d'observer la formation et la déviation d'un faisceau d'électrons dans un tube cathodique. Différents phénomènes seront observées tels que :

\begin{itemize}
\item \textbf{L'accélération des électrons} qui subissent l'effet d'un champ électrique axial (le canon à électrons).
\item \textbf{La déviation du faisceau} qui est provoquée par l'action de champ électrique et même magnétique.
\item \textbf{La visualisation de signaux électriques} sur l'écran fluorescent grâce à un balayage contrôlé.
\end{itemize}

## 1.1 Prise en main & Calibration du système 
Dans le but de pouvoir mieux comprendre comment régler le système et de réaliser des mesures précises et plus simple à analyser, nous avons calibré notre oscilloscope en déterminant la tension de Wehnelt. 

### 1.1.1 Méthode de mesure 
Afin de pouvoir réaliser ce laboratoire avec une meilleurs visibilité des mesures, nous avons : 
\begin{itemize}
\item Fixer une tension anodique à 250V 
\item Comme la tension de chauffage n'impacte pas la manipulation actuelle, nous l'avons mise au maximum, soit 8V. 
\item Pour pouvoir trouver la meilleure position du point sur l'oscilloscope didactique, nous avons orienté / tourné les 2 petits aiments qui se situaient sous l'écran comme montré sur la photo ci-dessous 
\end{itemize}

![Aiments](images/Aiment%20sur%20oscilloscope.png){width=300px}

En testant différentes tension de Wehnelt, nous avons trouvé que la meilleure tension pour pouvoir bien visualiser le point est de 18 $\pm$ 0,2V 
  
## 1.2 Manipulation 1 - Déviation électrique du faisceau électronique

### 1.2.1 Rappels théoriques

#### La génération des électrons
Les électrons sont produits par **une émission themoïonique** à partir d'une cathode chauffée. 
"Une émission thermoïonique (ou émission thermoélectronique) est un flux d'électrons provenant d'un métal ou d'un oxyde métallique, qui est provoqué par les vibrations des atomes dues à l'énergie thermique lorsque ceux-ci parviennent à surmonter les forces électrostatiques." (source : Wikipedia)
Le chauffage diminue la barrière de potentiel et permet aux électrons de s'échapper de la surface. Un **cylindre de Wehnelt**, polarisé de quelques dizaines de volts encore plus négativement que la cathode, repousse les électrons émis hors axe et les focalise en faisant un point de croissement sur l'axe. Une **anode** est placée à environ 10mm plus loin, portée à une tension positive par rapport à la cathode, attire et accélère les électrons à travers l'ouverture centrale. 

#### Le rôle des plaques de déviation
  
Le tube est équipé de 2 plaques de déviation électrostatiques. Cette paire de plaques latérale génère un champ électrique transverse $\vec{E}$, qui exercce sur les électrons une force $\vec{F} = q \cdot \vec{E}$. Cette force change la direction du faisceau perpendiculairement à son axe. Pour réaliser cette déviation latérale (droite ou gauche) les plaques sont polarisée de manière différentielle (+V ou -V) ce qui permet de modifier la trajectoire du faisceau sans toucher à son énergie. Contrairement à la déviation magnétique $\vec{F} = q \, \vec{v} \times \vec{E}$, qui sera étudié par la suite, la déviation électrostatique agit directement dans la direction du champ imposé entre les plaques.

Pour calculer la déviation, nous allons partir de l'hypothèse que les électrons ne sont pas *relativistes*, c'est-à-dire que leur vitesse est suffisamment faible pour que les effets de relativité soient négligeable. Nous allons donc utiliser la mécanique classique. Nous démontrerons plus bas que comme la vitesse des électrons est très loins de la vitesse de la lumière, les effets relativistes (comme l'augmentation de la masse effective) sont négligeables. 

#### Vitesse des électrons  
  
On sait que : $E_c = \dfrac{1}{2} m_e v^2 = e V_a$. Alors on peut facilement trouver la vitesse de l'électron qui donne : $v_e = \sqrt{\dfrac{2 e V_a}{m_e}}$ 

#### Equation de la déviation électrostatique  
  
Sachant que : $\begin{cases} d = \text{distance entre les plaques} [m] \\ L = \text{longueur de la bobine} [m] \\ D = \text{distance entre la sortie des plaques et l'écran} [m] \\ V_a = \text{tension d'accélération (anode-cathode)} [V] \\ V_p = \text{tension appliquée aux plaques de déviation} [V] \\ e = \text{charge d'un électron} [C] \\ m_e = \text{masse d'un électron} [kg] \end{cases}$

On sait que : $y \approx \frac{V_p}{V_a} \cdot \frac{L \cdot D}{2d}$

### 1.2.2 Calibration

## 1.3 Manipulation 2 - Déviation magnétique du faisceau électronique

### 1.3.3 Mesure et résultats

Pour commencer, nous avons décider de vérifier la polarisation du champ d'une bobine suivant la polarisation du courant avec une boussole. Nous en avons déduit que le pôle Nord est attiré par le $V_{CC}$ et donc que le pôle Sud est attiré par le GDN.Le champ $\vec{B}$ se déplace donc du $V_{CC}$ au GND.

## 3. Formes de lissajous

### 3.1 Introduction

Les formes de Lissajous tiennent leurs noms du physicien Jules Antoine Lissajous. Il a étudié les mouvements vibratoires et a découvert que lorsque deux mouvements sinusoïdaux sont combinés, ils peuvent créer des figures géométriques complexes. Ces figures sont obtenues en traçant la trajectoire en X et Y d'un point en fonction du temps, où chaque axe représente un mouvement sinusoïdal différent.

### 3.2 Équations des mouvements

Les mouvements en X et Y sont décrits par les équations suivantes :

\begin{itemize}
\item Mouvement en X : $x(t) = A_x \sin(\omega_x t + \phi_x)$
\item Mouvement en Y : $y(t) = A_y \sin(\omega_y t + \phi_y)$
\end{itemize}

Toutes les figures de Lissajous sont caractérisées par le rapport des fréquences (et donc des pulsations) $\dfrac{\omega_x}{\omega_y}$ et le déphasage entre les deux mouvements $\Delta \phi = \phi_x - \phi_y$.

La figure la plus simple est obtenue lorsque les pulsations sont égales ($\omega_x = \omega_y$) et le déphasage est nul ($\Delta \phi = 0$), ce qui donne une ligne droite diagonale.

![Figure de Lissajous diagonale](images/lissajous_diagonal.png)

### 3.3 Exemples de figures de Lissajous

#### 3.3.1 Variations des amplitudes

Voici quelques exemples de variation d’amplitude avec une phase et fréquence identique :  

\centering

\begin{minipage}{0.3\textwidth}
  \centering
  \includegraphics[width=\linewidth]{images/lissajous_2.png}
  \captionof{figure}{Amplitude de Y plus grande que celle de X}
\end{minipage}
\hfill
\begin{minipage}{0.3\textwidth}
  \centering
  \includegraphics[width=\linewidth]{images/lissajous_3.png}
  \captionof{figure}{Amplitude de X plus grande que celle de Y}
\end{minipage}
\raggedright


#### 3.3.2 Variations du déphasage

Voici quelques exemples de variation de déphasage avec des amplitudes et fréquences identiques :  

\centering

\begin{minipage}{0.3\textwidth}
  \centering
  \includegraphics[width=\linewidth]{images/lissajous_4.png}
  \captionof{figure}{Déphasage de $\dfrac{\pi}{3}$}
\end{minipage}
\hfill
\begin{minipage}{0.3\textwidth}
  \centering
  \includegraphics[width=\linewidth]{images/lissajous_5.png}
  \captionof{figure}{Déphasage de $\dfrac{\pi}{2}$}
\end{minipage}
\hfill
\begin{minipage}{0.3\textwidth}
  \centering
  \includegraphics[width=\linewidth]{images/lissajous_6.png}
  \captionof{figure}{Déphasage de $\dfrac{\pi}{3}$ en $x$ et $\dfrac{\pi}{2}$ en $y$}
\end{minipage}
\raggedright


#### 3.3.3 Variations du rapport des fréquences

Pour trouver le rapport des fréquences, on peut compter le nombre de pics dans chaque direction. Le rapport des fréquences est alors donné par le ratio du nombre de pics en X sur le nombre de pics en Y.

Voici quelques exemples de variation du rapport des fréquences avec des amplitudes et déphasages identiques :

\centering
\begin{minipage}{0.3\textwidth}
  \centering
  \includegraphics[width=\linewidth]{images/ratio_1-2.png}
  \captionof{figure}{ratio 1:2}
\end{minipage}
\hfill
\begin{minipage}{0.3\textwidth}
  \centering
  \includegraphics[width=\linewidth]{images/ratio_1-6.png}
  \captionof{figure}{ratio 1:6}
\end{minipage}
\hfill
\begin{minipage}{0.3\textwidth}
  \centering
  \includegraphics[width=\linewidth]{images/ratio_3-1.png}
  \captionof{figure}{ratio 3:1}
\end{minipage}

\centering

\begin{minipage}{0.3\textwidth}
  \centering
  \includegraphics[width=\linewidth]{images/ratio_3-2.png}
  \captionof{figure}{ratio 3:2}
\end{minipage}
\hfill
\begin{minipage}{0.3\textwidth}
  \centering
  \includegraphics[width=\linewidth]{images/ratio_4-3.png}
  \captionof{figure}{ratio 4:3}
\end{minipage}
\hfill
\begin{minipage}{0.3\textwidth}
  \centering
  \includegraphics[width=\linewidth]{images/ratio_4-7.png}
  \captionof{figure}{ratio 4:7}
\end{minipage}
\raggedright

### 3.4 Parallèle avec le canon à électrons

Le canon à électrons utilise des champs électriques et magnétiques pour dévier le faisceau d'électrons (voir partie 2). En appliquant des tensions alternatives avec des générateurs de signaux aux bobines de déviation horizontales et verticales, on peut créer des mouvements sinusoïdaux similaires à ceux décrits par les équations des figures de Lissajous. Ainsi, en ajustant les fréquences et les phases des tensions appliquées, on peut obtenir des figures de Lissajous sur l'écran du tube cathodique, permettant d'analyser les signaux électriques de manière visuelle.

Voici des figures de Lissajous obtenues avec le canon à électrons :

\centering
\begin{minipage}{0.3\textwidth}
  \centering
  \includegraphics[width=\linewidth]{images/labo-3-4.jpg}
  \captionof{figure}{ratio 3:4}
\end{minipage}
\begin{minipage}{0.3\textwidth}
  \centering
  \includegraphics[width=\linewidth]{images/labo-2-3.jpg}
  \captionof{figure}{ratio 2:3}
\end{minipage}
\raggedright

On remarque que les figures obtenues avec le canon à électrons sont similaires à celles générées mathématiquement, confirmant ainsi la relation entre les mouvements sinusoïdaux et les figures de Lissajous.

Avec le rapport de fréquence $\dfrac{200Hz}{150Hz} = \dfrac{4}{3}$, on obtient une figure de Lissajous correspondant au ratio 4:3, on voit bien les $4$ pics en vertical et les $3$ pics en horizontal.
Avec le rapport de fréquence $\dfrac{200Hz}{100Hz} = \dfrac{2}{3}$, on obtient une figure de Lissajous correspondant au ratio 2:3, on voit bien les $3$ pics en vertical et les $2$ pics en horizontal.

Ces images confirment bien le lien entre les figures de Lissajous et la déviation des électrons par des champs électriques alternatifs ainsi que le rapport entre les fréquences des tensions appliquées et la forme obtenue.

## 3.5 Conclusion

Les figures de Lissajous offrent une représentation visuelle fascinante des interactions entre deux mouvements sinusoïdaux. En variant les amplitudes, les déphasages et les rapports de fréquences, on peut générer une multitude de formes géométriques complexes. Ces figures ne sont pas seulement esthétiques, elles ont également des applications pratiques en physique et en ingénierie, notamment dans l'analyse des signaux électriques à l'aide d'oscilloscopes et de canons à électrons. Comprendre les principes sous-jacents aux figures de Lissajous permet d'approfondir notre connaissance des phénomènes vibratoires et des interactions dynamiques dans divers systèmes physiques.

Plus précisement, cette partie de labo nous à permis de voir une application concrète de la déviation des électrons par des champs électriques alternatifs, et de comprendre comment les anciens oscilloscopes fonctionnaient pour analyser des signaux électriques.