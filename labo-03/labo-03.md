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
| Vitesse de l'onde | $v = \sqrt{\frac{E}{\rho}} m/s$ |
| Impédance $Z$ | $Z = \sqrt{E \rho} Pa \dot s/m$ |
| Grandeur caractéristique | $\sigma_0 = Z\omega \psi_0$ contrainte |
| Puissance moyenne $\bar{P}$ | $\dfrac{S\sigma_0^2}{2Z}$ |
| Intensité moyenne $\bar{I}$ | $\dfrac{\sigma_0^2}{2Z}$ |
