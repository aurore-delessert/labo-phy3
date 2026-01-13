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

![Montage expérimental](images/schema_barreau.jpg)

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

insérer schéma du montage

### Effet Doppler

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

#### But de l'expérience

Le but est d'observer l'effet Doppler en bougeant une source d'ondes à une vitesse constante et en mesurant la fréquence des ondes. Nous allons pouvoir determiner la vitesse de la source à partir des fréquences mesurées lorsque la source se rapproche et s'éloigne de l'observateur.

