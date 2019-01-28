# LaTeX commands 

## Document Layout: 

1. `\part{Some part}`
2. `\chapter{Some chapter}`
3. `\section{Some section}`
4. `\subsection{Some subsection}`
5. `\subsubsection{Some subsubsection}`
6. `\paragraph{Some paragraph}`
7. `\subparagraph{Some subparagraph}`

## Formatting:

* Italics: `\emph{This is italic text}`
* Bold: `\textbf{This is bold text}`
* Bulletted List:
```
\begin{itemize}
	\item This is your first bulleted item
	\item The \item command tells it to start a new one
\end{itemize}
```
* Numbered List:
```
\begin{enumerate}
	\item This is your first numbered item
	\item The \item command tells it to start a new one
\end{enumerate}
```

## Equations:

* Inline Equation: `$some equation$`
* Single Equation:
```
\begin{equation}
	\phi(t)=\frac{1}{\sqrt{2\pi}}
	\intˆt_0 eˆ{-xˆ2/2} dx
\end{equation}
```
* Multiple Equations
```
\begin{align}
	\label{eqn:equ_1_label}
		left hand side of equation &= right hand sign of equation \\
	\label{eqn:equ_2_label}
		left hand side of equation &= right hand sign of equation 
\end{align}
```


## Figures/Tables:

When writing a sentence to reference a figure write `Figure \ref{fig:figure_label}`.

* Regular Figure:
```
\begin{figure}[!htb]\centering
	\includegraphics[width=\textwidth]{some_figure_name}
	\caption{Some figure caption}
	\label{fig:figure_label}
\end{figure}
```
* Sub-Figures:
```
\begin{figure}[!htb]\centering
	\begin{subfigure}[c]{0.5\textwidth}\centering
	\includegraphics[width=\textwidth]{figure_1_name}
	\caption{Figure 1 caption}
	\label{fig:figure_1_label}
	\end{subfigure}
		\begin{subfigure}[c]{0.5\textwidth}\centering
		\includegraphics[width=\textwidth]{figure_2_name}
		\caption{Figure 2 caption}
		\label{fig:figure_2_label}
		\end{subfigure}
\caption{The caption under everything}
\label{fig:combined_figure_label}
\end{figure}
```
* Table:
```
\begin{center}
	\begin{tabular}{|c|c|c|} \hline 
		cell1 & cell2 & cell3 \\ \hline
		cell4 & cell5 & cell6 \\ \hline
		cell7 & cell8 & cell9 \\ \hline
	\end{tabular}
\end{center}
```

## Using PINE's reporting template

File structure:
```
ReportFolder
|  latexDocker.sh
|  buildReport.sh
|  definitions.tex
|  pine_functions.tex
|  ReportName.tex
|
|-- contributions
|   |   
|   |-- PersonOne
|   |   | ReportPartOne.tex
|   |   | ReportPartTwo.tex
|   |   | 
|   |   |-- images
|   |   |    |-- ImageOne.png
|   |   |    |-- ImageTwo.pdf
|   |
|   |-- PersonTwo
|   |   | ReportPartOne.tex
|   |   | ReportPartTwo.tex
|   |   | 
|   |   |-- images
|   |   |    |-- ImageOne.png
|   |   |    |-- ImageTwo.pdf
...
```

Within the main report (ReportName.tex) using the `contrib{}{}` function to include the report parts as follows:


```
\section{Person one part one section title}
contrib{PersonOne}{ReportPartOne.tex}

\section{Person one part two section title}
contrib{PersonOne}{ReportPartTwo.tex}

\section{Person two part one section title}
contrib{PersonTwo}{ReportPartOne.tex}

\section{Person one part two section title}
contrib{PersonTwo}{ReportPartTwo.tex}
```

Building the latex file:
`./buildReport.sh ReportName.tex`
