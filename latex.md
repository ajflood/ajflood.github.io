# LaTeX commands 

## Insert Regular Figure
When writing a sentence to reference a figure write `Figure \ref{fig:figure_label}`.
```
\begin{figure}[!htb]\centering
	\includegraphics[width=\textwidth]{some_figure_name}
	\caption{Some figure caption}
	\label{fig:figure_label}
\end{figure}
```

## Insert Sub-Figure
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

