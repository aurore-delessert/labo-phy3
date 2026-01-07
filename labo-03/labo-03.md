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

## Experience 2: Propagation d'une onde dans un barreau

### Rappels théoriques

On est ici dans le cas d'une onde longitudinale se propageant dans un barreau. La vitesse de propagation $v$ de l'onde est reliée au module d'Young $E$ et à la masse volumique $\rho$ du matériau par la relation suivante:

| | Barreau solide |
|---|---|
| Facteur de force de rappel | $E$ module d'Young |
| Facteur d'inertie | $\rho$ masse volumique |
| Vitesse de l'onde | $v = \sqrt{\frac{E}{\rho}}= \lambda f m/s$ |


### But de l'expérience

Le but de cette expérience est de mesurer la vitesse de propagation d'une onde longitudinale dans différents barreaux. Pour cela nous allons analyser l'onde qui se propage dans le barreau à l'aide d'un capteurs placé à la fin du barreau. Ainsi en connaissant la fréquence de l'onde émise et la distance entre le point d'émission et le capteur, nous pourrons en déduire la vitesse de propagation de l'onde dans le barreau. 

### Montage expérimental

Nous allons utiliser le montage suivant:

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

- $\lambda_{Al} = 41.08 \times 10^{-6} \pm 3 \times 10^{-6} m$ (distance entre deux crêtes successives)

$$v_{Al,mes} = \frac{L_{Al}}{t_{Al}} = \frac{0.2}{41.08 \times 10^{-6}} = 4868 m/s$$

Incertitude sur la vitesse mesurée:

- Incertitude sur la longueur: $\Delta L_{Al} = 0.001 m$
- Incertitude sur la longueur d'onde: $\Delta \lambda_{Al} = 3 \times 10^{-6} m$

$$\delta v_{Al,mes} = v_{Al,mes} \sqrt{\left(\frac{\Delta L_{Al}}{L_{Al}}\right)^2 + \left(\frac{\Delta \lambda_{Al}}{\lambda_{Al}}\right)^2} = 4868 \sqrt{\left(\frac{0.001}{0.2}\right)^2 + \left(\frac{3 \times 10^{-6}}{41.08 \times 10^{-6}}\right)^2} \approx 4868 \sqrt{(0.005)^2 + (0.073)^2} \approx 4868 \times 0.073 = 356 m/s$$

Donc la vitesse mesurée dans le barreau en aluminium est:

$$v_{Al,mes} = 4868 \pm 356 m/s$$

On voit que la vitesse mesurée est en accord avec la vitesse théorique dans les limites de l'incertitude.



