# LaTeX commands 

### Sections: 
`section{Some section names you want}`

### Sub sections: 
`subsection{Some subsection heading}`

### Italics: 
`\emph{This is italic text}`

### Bold: 
`\textbf{This is bold text}`

### Bulletted List:
```
\begin{itemize}
	\item This is your first bulleted item
	\item The \item command tells it to start a new one
\end{itemize}
```

### Numbered List:
```
\begin{enumerate}
	\item This is your first numbered item
	\item The \item command tells it to start a new one
\end{enumerate}
```

### Equation:
```
\begin{equation}
	\phi(t)=\frac{1}{\sqrt{2\pi}}
	\intˆt_0 eˆ{-xˆ2/2} dx
\end{equation}
```

### Insert Regular Figure:

When writing a sentence to reference a figure write `Figure \ref{fig:figure_label}`.
```
\begin{figure}[!htb]\centering
	\includegraphics[width=\textwidth]{some_figure_name}
	\caption{Some figure caption}
	\label{fig:figure_label}
\end{figure}
```

### Insert Sub-Figure:
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

### Insert Table
```
\begin{center}
	\begin{tabular}{|c|c|c|} \hline 
		cell1 & cell2 & cell3 \\ \hline
		cell4 & cell5 & cell6 \\ \hline
		cell7 & cell8 & cell9 \\ \hline
	\end{tabular}
\end{center}
```
