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
  - \usepackage{float}
---

\includegraphics[width=0.25\textwidth]{images/heig-logo.png}

\thispagestyle{empty}
\begin{center}
\vspace*{3cm}

\noindent\rule{\textwidth}{0.4pt}\\[0.6cm]

{\Huge \textbf{Labo 03}}\\[0.5cm]
{\LARGE \textit{Projet sur la propagation des ondes}}\\[0.3cm]
\noindent\rule{\textwidth}{0.4pt}\\[1.5cm]

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

## Experience 2 : Propagation d'une onde longitudinale dans un barreau

### Rappels théoriques

On est ici dans le cas d'une onde longitudinale se propageant dans un barreau. La vitesse de propagation $v$ de l'onde est reliée au module d'Young $E$ et à la masse volumique $\rho$ du matériau par la relation suivante:

| - | Barreau solide |
| ------ | ------ |
| Facteur de force de rappel | $E$ module d'Young |
| Facteur d'inertie | $\rho$ masse volumique |
| Vitesse de l'onde | $v = \sqrt{\frac{E}{\rho}}= \lambda f = dfrac{\lambda}{T} m/s$ |

### But de l'expérience

Le but de cette expérience est de mesurer la vitesse de propagation d'une onde longitudinale dans différents barreaux. Pour cela nous allons analyser l'onde qui se propage dans le barreau à l'aide d'un capteurs placé à la fin du barreau. Ainsi en connaissant la fréquence de l'onde émise et la distance entre le point d'émission et le capteur, nous pourrons en déduire la vitesse de propagation de l'onde dans le barreau. 

### Montage expérimental

Nous allons utiliser le montage suivant:

![Montage expérimental](images/schema_barreau.jpg){#fig:QE width=80%}

### Résultats de l'expérience

Nous avons effectué des mesures sur trois barreaux différents: un barreau en aluminium, un barreau en laiton et un barreau en acier. Pour chaque barreau, nous avons emis des ondes en tapant dessus avec un petit "marteau" et nous avons enregistré la réponse à l'aide d'un capteur placé à l'extrémité du barreau. Voici les résultats obtenus:

#### Barreau en aluminium

- Longueur du barreau: $L_{Al} = 0.2 \pm 0.001 m$
- Masse volumique: $\rho_{Al} = 2700 kg/m^3$ (CRM)
- Module d'Young: $E_{Al} = 70 GPa$ (CRM)

Vitesse théorique:

$$v_{Al} = \sqrt{\frac{E_{Al}}{\rho_{Al}}} = \sqrt{\frac{70 \times 10^9}{2700}} \approx 5091 m/s$$

Ici pas d'incertitude car ce sont des valeurs de référence.

Vitesse mesurée:

- $T_{Al} = 40.9 \times 10^{-6} \pm 3 \times 10^{-6} s$ (temps entre deux crêtes successives)

$$v_{Al,mes} = \frac{L_{Al}}{T_{Al}} = \frac{0.2}{40.9 \times 10^{-6}} = 4888 m/s$$

Incertitude sur la vitesse mesurée:

- Incertitude sur la longueur: $\Delta L_{Al} = 0.001 m$
- Incertitude sur la période: $\Delta T_{Al} = 3 \times 10^{-6} s$

$\delta v_{Al,mes} = v_{Al,mes} \sqrt{\left(\frac{\Delta L_{Al}}{L_{Al}}\right)^2 + \left(\frac{\Delta T_{Al}}{T_{Al}}\right)^2} = 4888 \sqrt{\left(\frac{0.001}{0.2}\right)^2 + \left(\frac{3 \times 10^{-6}}{40.9 \times 10^{-6}}\right)^2} \approx 4888 \sqrt{(0.005)^2 + (0.073)^2} \approx 4888 \times 0.073 = 356 m/s$

Donc la vitesse mesurée dans le barreau en aluminium est:

$$v_{Al,mes} = 4888 \pm 356 m/s$$

On voit que la vitesse mesurée est en accord avec la vitesse théorique dans les limites de l'incertitude.

#### Barreau en laiton

- Longueur du barreau: $L_{CuZn} = 0.2 \pm 0.001 m$
- Masse volumique: $\rho_{CuZn} = 8470 kg/m^3$ (CRM)
- Module d'Young: $E_{CuZn} = 100 GPa$ (CRM)

Vitesse théorique:

$$v_{CuZn} = \sqrt{\frac{E_{CuZn}}{\rho_{CuZn}}} = \sqrt{\frac{100 \times 10^9}{8470}} \approx 3436 m/s$$

Ici pas d'incertitude car ce sont des valeurs de référence.

Vitesse mesurée:

- $T_{CuZn} = 61.0 \times 10^{-6} \pm 3 \times 10^{-6} s$ (temps entre deux crêtes successives)

$$v_{CuZn,mes} = \frac{L_{CuZn}}{T_{CuZn}} = \frac{0.2}{61.0 \times 10^{-6}} = 3278 m/s$$

Incertitude sur la vitesse mesurée:

- Incertitude sur la longueur: $\Delta L_{CuZn} = 0.001 m$
- Incertitude sur la période: $\Delta T_{CuZn} = 3 \times 10^{-6} s$

$$\delta v_{CuZn,mes} = v_{CuZn,mes} \sqrt{\left(\frac{\Delta L_{CuZn}}{L_{CuZn}}\right)^2 + \left(\frac{\Delta T_{CuZn}}{T_{CuZn}}\right)^2} = 3278 \sqrt{\left(\frac{0.001}{0.2}\right)^2 + \left(\frac{3 \times 10^{-6}}{61.0 \times 10^{-6}}\right)^2} \approx 3278 \sqrt{(0.005)^2 + (0.049)^2} \approx 3278 \times 0.049 = 161 m/s$$

Donc la vitesse mesurée dans le barreau en laiton est:

$$v_{CuZn,mes} = 3278 \pm 161 m/s$$

On voit que la vitesse mesurée est en accord avec la vitesse théorique dans les limites de l'incertitude.

#### Barreau en acier

- Longueur du barreau: $L_{Fe} = 0.2 \pm 0.001 m$
- Masse volumique: $\rho_{Fe} = 7850 kg/m^3$ (CRM)
- Module d'Young: $E_{Fe} = 200 GPa$ (CRM)

Vitesse théorique:

$$v_{Fe} = \sqrt{\frac{E_{Fe}}{\rho_{Fe}}} = \sqrt{\frac{200 \times 10^9}{7850}} \approx 5051 m/s$$

Ici pas d'incertitude car ce sont des valeurs de référence.

Vitesse mesurée:

- $T_{Fe} = 41.08 \times 10^{-6} \pm 3 \times 10^{-6} s$ (temps entre deux crêtes successives)

$$v_{Fe,mes} = \frac{L_{Fe}}{T_{Fe}} = \frac{0.2}{41.08 \times 10^{-6}} = 4868 m/s$$

Incertitude sur la vitesse mesurée:

- Incertitude sur la longueur: $\Delta L_{Fe} = 0.001 m$
- Incertitude sur la période: $\Delta T_{Fe} = 3 \times 10^{-6} s$

$$\delta v_{Fe,mes} = v_{Fe,mes} \sqrt{\left(\frac{\Delta L_{Fe}}{L_{Fe}}\right)^2 + \left(\frac{\Delta T_{Fe}}{T_{Fe}}\right)^2} = 4868 \sqrt{\left(\frac{0.001}{0.2}\right)^2 + \left(\frac{3 \times 10^{-6}}{41.08 \times 10^{-6}}\right)^2} \approx 4868 \sqrt{(0.005)^2 + (0.073)^2} \approx 4868 \times 0.073 = 355 m/s$$

Donc la vitesse mesurée dans le barreau en acier est:

$$v_{Fe,mes} = 4868 \pm 355 m/s$$

On voit que la vitesse mesurée est en accord avec la vitesse théorique dans les limites de l'incertitude.

### A quoi ça sert dans la vie de tous les jours?

La connaissance de la vitesse de propagation des ondes dans différents matériaux est cruciale dans de nombreux domaines d'ingénierie et de physique appliquée. Par exemple, dans le domaine de la construction, comprendre comment les ondes sonores se propagent à travers les matériaux permet de concevoir des bâtiments avec une meilleure isolation acoustique. De plus, dans l'industrie automobile et aérospatiale, la connaissance des propriétés des matériaux aide à optimiser la résistance aux vibrations et aux chocs, améliorant ainsi la sécurité et le confort.

### Conclusion

Dans cette expérience, nous avons mesuré la vitesse de propagation d'une onde longitudinale dans trois types de barreaux: aluminium, laiton et acier. Pour chaque matériau, nous avons comparé la vitesse mesurée avec la vitesse théorique calculée à partir du module d'Young et de la masse volumique. Nos résultats montrent que les vitesses mesurées sont en bon accord avec les vitesses théoriques, ce qui confirme la validité de la relation entre la vitesse de l'onde, le module d'Young et la masse volumique. Les incertitudes associées à nos mesures sont raisonnables et n'affectent pas significativement la conclusion de l'expérience.

## Experience 3 : Cuve à ondes

### But de l'expérience

Une cuve à ondes est un dispositif utilisé pour étudier la propagation des ondes à la surface de l'eau. En générant des ondes à une extrémité de la cuve, on peut observer comment elles se propagent, se réfléchissent et interagissent avec des obstacles.

Ici notre but va être de déterminer la vitesse de propagation des ondes à la surface de l'eau en fonction de la fréquence des ondes générées, aussi de montrer l'effet Doppler avec une source mobile et enfin d'observer des phénomènes d'interférences entre deux sources d'ondes.

### Montage expérimental

![Cuve à ondes](images/cuve_a_ondes.png){#fig:QE width=80%}

- a : interrupteur du stroboscope
- b : bouton (réglage fin de la fréquence du stroboscope)
- c : bouton poussoir (excitation d’ondes uniques)
- d : bouton (réglage de l‘amplitude de l’excitation d’ondes)
- e : bouton (réglage de la fréquence de l‘excitation d’ondes)
- f : vis moletée (rotation manuelle du disque stroboscopique)
- g : écran d’observation
- h1 : Raccord d’un excitateur d’ondes circulaires
- h2 : Raccord d’un excitateur d’ondes rectilignes

Sur l'image de gauche on peut voir le dispositif au complet avec le générateur d'ondes (air) et la cuve à ondes. Sur l'image en haut à droite on peut voir un zoom sur la cuve à ondes avec le générateur d'ondes circulaire immergé dans l'eau et sur l'image en bas à droite on peut voir le générateur d'ondes linéaire immergé dans l'eau.

### Calibration de la cuve à ondes

Pour calibrer la cuve à ondes, nous avons utilisé un petit bâton de $97 mm$ que nous avons posé dans la cuve afin d'observer son image sur l'écran. En mesurant la longueur de l'image projetée sur l'écran, nous avons pu déterminer le facteur de grossissement de la cuve à ondes.

| Longueur réelle du bâton | Longueur de l'image projetée |
| ------------------------ | ---------------------------- |
| $97 \pm 0.5 mm$          | $158 \pm 1 mm$             |

Le facteur de grossissement $G$ est donné par la formule:

$$G = \frac{\text{Longueur de l'image}}{\text{Longueur réelle}} = \frac{158 mm}{97 mm} \approx 1.63$$

Ce qui veut dire que lorsque nous mesurons une distance sur l'écran, nous devons la diviser par $1.63$ pour obtenir la distance réelle dans la cuve à ondes.

Incertitude sur le facteur de grossissement:

$$\Delta G = G \sqrt{\left(\frac{\Delta \text{Longueur de l'image}}{\text{Longueur de l'image}}\right)^2 + \left(\frac{\Delta \text{Longueur réelle}}{\text{Longueur réelle}}\right)^2} = 1.63 \sqrt{\left(\frac{1 mm}{158 mm}\right)^2 + \left(\frac{0.5 mm}{97 mm}\right)^2} \approx 1.63 \sqrt{(0.00633)^2 + (0.00515)^2} \approx 1.63 \times 0.0082 \approx 0.013$$

Donc le facteur de grossissement est: $G = 1.63 \pm 0.013$

### Mesure de la vitesse des ondes en fonction de la fréquence

Nous avons généré des ondes à différentes fréquences en utilisant le générateur d'ondes linéaire. Pour chaque fréquence, nous avons mesuré la longueur d'onde des ondes générées en observant la distance entre deux crêtes successives.

Nous allons utiliser la formule de la vitesse des ondes $v = \lambda f$ et calculer l'incertitude associée avec la formule $\delta v = v \sqrt{\left(\frac{\Delta \lambda}{\lambda}\right)^2 + \left(\frac{\Delta f}{f}\right)^2}$. L'incertitude sur la longueur d'onde réelle est donnée par $\Delta \lambda = \frac{\Delta \lambda_{mes}}{G}$ où $\Delta \lambda_{mes}$ est l'incertitude sur la longueur d'onde mesurée sur l'écran qui est égale à $0.013$.

| Fréquence (Hz) | Longueur d'onde mesurée sur l'écran (mm) | Longueur d'onde réelle (m) | Vitesse des ondes (m/s) |
| -------------- | -----------------------------------------| --------------------------- | ----------------------- |
| 30             | $12 \pm 1$                               | $0.0073 \pm 0.013$  | $0.220 \pm 0.03$ |
| 40             | $9 \pm 1$                                | $0.0055 \pm 0.013$  | $0.220 \pm 0.04$ |
| 50             | $8 \pm 1$                                | $0.0049 \pm 0.013$  | $0.247 \pm 0.05$ |
| 60             | $7 \pm 1$                                | $0.0043 \pm 0.013$  | $0.258 \pm 0.06$ |
| 70             | $6 \pm 1$                                | $0.0037 \pm 0.013$  | $0.258 \pm 0.07$ |

### Effet Doppler

Grâce à la cuve à ondes, nous avons pu observer l'effet Doppler en déplaçant une source d'ondes circulaires. N'ayant pas de moyen de mesurer précisément la vitesse de la source, nous allons nous contenter d'observer qualitativement le phénomène.

#### Rappels théoriques

L'effet Doppler est un phénomène physique qui se manifeste par une variation de la fréquence perçue d'une onde lorsqu'il y a un mouvement relatif entre la source de l'onde et l'observateur. Lorsque la source se rapproche de l'observateur, la fréquence perçue augmente (décalage vers le bleu), tandis que lorsque la source s'éloigne, la fréquence perçue diminue (décalage vers le rouge).

La formule générale de l'effet Doppler pour une onde se propageant dans un milieu est donnée par:

$$f' = f \frac{v + v_o}{v + v_s}$$

où:

- $f'$ est la fréquence perçue par l'observateur,
- $f$ est la fréquence émise par la source,
- $v$ est la vitesse de l'onde dans le milieu,
- $v_o$ est la vitesse de l'observateur par rapport au milieu (positive si l'observateur se rapproche de la source),
- $v_s$ est la vitesse de la source par rapport au milieu (positive si la source s'éloigne de l'observateur).

#### Observation expérimentale

Pour cette experience nous avons juste déplacer le générateur d'ondes circulaires rapidement de haut en bas et de bas en haut dans la cuve à ondes. Nous avons pu observer que lorsque la source se déplaçait vers le haut, les crêtes des ondes étaient plus rapprochées, indiquant une fréquence plus élevée. Inversement, lorsque la source se déplaçait vers le bas, les crêtes des ondes étaient plus espacées, indiquant une fréquence plus basse.

Nous avons aussi vu le phénomène de cônes de Mach lorsque la source se déplaçait plus vite que la vitesse des ondes dans le milieu, formant un angle caractéristique avec la direction du mouvement.

Voici une illustration de l'effet Doppler et du cône de Mach observé dans la cuve à ondes:

![Effet Doppler et cône de Mach](images/doppler_mach.png){#fig:QE width=80%}

Ici on peut voir que les ondes sont plus rapprochées devant la source en mouvement (fréquence plus élevée) et plus espacées derrière la source (fréquence plus basse). 

La valeur de l'angle $\theta$ du cône de Mach peut être reliée à la vitesse de la source $v_s$ et à la vitesse des ondes $v$ par la relation:

$$\sin(\theta) = \frac{v}{v_s}$$

En mesurant cet angle, nous pourrions estimer la vitesse de la source par rapport à la vitesse des ondes dans la cuve.

![Cône de Mach](images/photo_mach.png){#fig:QE width=80%}

Ici l'angle $\theta$ peut être mesuré pour estimer la vitesse de la source.

$\theta \approx 66^\circ \pm 1^\circ$

Donc avec $v$ repris de la table précédente pour une fréquence de $60 Hz$:

$$\sin(66^\circ) = \frac{v}{v_s} \Rightarrow v_s = \frac{v}{\sin(66^\circ)} = \frac{0.258 m/s}{0.9135} \approx 0.282 m/s$$

Incertitude sur la vitesse de la source:

$$\Delta v_s = v_s \sqrt{\left(\frac{\Delta v}{v}\right)^2 + \left(\frac{\Delta \sin(\theta)}{\sin(\theta)}\right)^2} = 0.282 \sqrt{\left(\dfrac{0.07}{0.258}\right)^2 + \left(\dfrac{0.017}{0.914}\right)^2} = 0.0767$$

Donc la vitesse estimée de la source est:

$$v_s = 0.282 \pm 0.077 m/s$$

#### Dans la vie de tous les jours

On retrouve l'effet Doppler dans de nombreux phénomènes quotidiens. Par exemple, le son d'une sirène d'ambulance ou de police change de hauteur lorsqu'elle passe près de nous, en raison du mouvement de la source sonore par rapport à l'observateur. De même, en astronomie, l'effet Doppler est utilisé pour déterminer la vitesse des étoiles et des galaxies par rapport à la Terre, ce qui aide à comprendre l'expansion de l'univers. Enfin, les radars de vitesse utilisent également l'effet Doppler pour mesurer la vitesse des véhicules en mouvement.

Pour le cône de Mach, on le retrouve dans les avions supersoniques. Lorsqu'un avion dépasse la vitesse du son, il crée un cône de Mach similaire à celui observé dans la cuve à ondes, ce qui peut entraîner un bang sonique entendu au sol.

#### Conclusion

L'expérience de l'effet Doppler dans la cuve à ondes nous a permis d'observer qualitativement le phénomène de variation de fréquence perçue en fonction du mouvement relatif entre la source et l'observateur. En déplaçant la source d'ondes circulaires, nous avons constaté que les crêtes des ondes se rapprochaient lorsque la source se déplaçait vers le haut et s'éloignaient lorsqu'elle se déplaçait vers le bas, illustrant ainsi l'effet Doppler. De plus, nous avons observé la formation d'un cône de Mach lorsque la source se déplaçait plus rapidement que la vitesse des ondes dans le milieu, ce qui a permis d'estimer la vitesse de la source par rapport à la vitesse des ondes. Ces observations confirment les principes fondamentaux de l'effet Doppler et démontrent son importance dans la compréhension des phénomènes ondulatoires dans divers contextes physiques.

### Interférences entre deux sources d'ondes

Pour cette expérience, nous avons utilisé deux générateurs d'ondes circulaires placés à une distance fixe l'un de l'autre dans la cuve à ondes. En réglant les deux générateurs pour qu'ils émettent des ondes à la même fréquence et en phase, nous avons pu observer le phénomène d'interférences entre les ondes générées par les deux sources.

![Interférences dans la cuve à ondes](images/interference.png){#fig:QE width=80%}

#### Rappels théoriques

Lorsque deux ondes se superposent, elles peuvent interférer de manière constructive ou destructive en fonction de leur phase relative. L'interférence constructive se produit lorsque les crêtes des deux ondes coïncident, ce qui amplifie l'amplitude résultante. En revanche, l'interférence destructive se produit lorsque la crête d'une onde coïncide avec le creux de l'autre, ce qui réduit l'amplitude résultante.

Voici comment calculer les lignes d'interférence :

$d_c = n \lambda$ pour les interférences constructives (maxima), où $n$ est un entier (0, 1, 2, ...).

$d_d = (n + 0.5) \lambda$ pour les interférences destructives (minima), où $n$ est un entier (0, 1, 2, ...).

![Schéma des interférences](images/interference_couleur.png){#fig:QE width=80%}

#### Observation expérimentale

En observant l'écran de la cuve à ondes, nous avons pu identifier des zones où les ondes des deux sources s'additionnaient pour former des crêtes plus élevées (interférences constructives) et des zones où les ondes s'annulaient partiellement (interférences destructives).

Voici une photo prise de l'écran montrant les motifs d'interférence:

![Photo des interférences](images/photo_interference.png){#fig:QE width=80%}

Avec en noir les hyperboles d'interférences.

Avec $\lambda \approx \dfrac{0.008}{1.63} m \approx 0.0049 m$ et la distance entre les deux sources $d = 0.1 m$.

$$d_c = n \lambda = 0.0049m$$

$$d_d = (n + 0.5) \lambda = 0.00245m$$

#### Dans la vie de tous les jours

Les interférences entre ondes sont un phénomène courant dans de nombreux domaines de la physique et de la technologie. Par exemple, en acoustique, les interférences peuvent affecter la qualité du son dans une salle de concert, où des ondes sonores provenant de différentes sources peuvent se superposer pour créer des zones de son plus fort ou plus faible. En optique, les interférences sont utilisées dans des dispositifs tels que les interféromètres pour mesurer des distances très précises ou des variations de phase. Dans les télécommunications, les interférences entre signaux peuvent entraîner des perturbations dans la transmission des données, ce qui nécessite des techniques de modulation et de filtrage pour minimiser ces effets.

#### Conclusion

L'expérience des interférences entre deux sources d'ondes dans la cuve à ondes nous a permis d'observer les motifs caractéristiques d'interférence résultant de la superposition des ondes émises par les deux générateurs. En réglant les sources pour qu'elles émettent des ondes à la même fréquence et en phase, nous avons pu identifier clairement les zones d'interférences constructives et destructives sur l'écran de la cuve. Ces observations confirment les principes fondamentaux des interférences ondulatoires et illustrent comment la superposition des ondes peut conduire à des variations significatives de l'amplitude résultante en fonction de la phase relative des ondes impliquées.

### Diffraction des ondes

La diffraction est un phénomène qui se produit lorsque des ondes rencontrent un obstacle ou une ouverture, provoquant une déviation de leur trajectoire. Dans cette expérience, nous avons observé la diffraction des ondes à la surface de l'eau en utilisant la cuve à ondes.

#### Observation expérimentale

En plaçant un obstacle partiel dans le chemin des ondes générées par le générateur d'ondes linéaire, nous avons pu observer comment les ondes se courbaient autour de l'obstacle, créant des motifs de diffraction sur l'écran de la cuve.

![Diffraction des ondes](images/diffraction.png){#fig:QE width=80%}

Ce phénomène est interessant car il montre que les ondes ne se propagent pas uniquement en ligne droite, mais peuvent également contourner des obstacles, ce qui est crucial dans de nombreux domaines, tels que l'acoustique, l'optique et les télécommunications.

Comme ici sur l'image, On peut voir que les ondes passent à travers une ouverture et se propagent en formant des cercles, illustrant ainsi le phénomène de diffraction alors que les ondes de base étaient rectilignes.

#### Conclusion

Ici nous avons juste fait une courte observation qualitative de la diffraction des ondes à la surface de l'eau dans la cuve à ondes. En plaçant un obstacle partiel dans le chemin des ondes, nous avons pu observer comment les ondes se courbaient autour de l'obstacle, créant des motifs de diffraction caractéristiques. Cette observation illustre le principe fondamental de la diffraction, qui est essentiel pour comprendre le comportement des ondes dans divers contextes physiques.