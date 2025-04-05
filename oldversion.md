\documentclass{article}
\usepackage{graphicx} % Required for inserting images
\usepackage{amsmath}  % Recommended for math environments like equation, align, etc.

\title{Feinkonzept}
\author{Juri S.}
\date{April 2025}

\begin{document}

\maketitle

\section{What is Bitcoin}

\section{Auction principle}
Explain how the price of Bitcoin is determined 

\section{Exploited}
\subsection*{Edge}
Is it even possible to make money? Because if there is a system wouldn't everbody be using it making the edge unusable or exploited?

\section{Data sources}
Detail your data sources, signal processing, order management, etc.

\subsection{Formulas}
Below I explain the mathematical formulas for the indicators I'm planning to use for an EMA with a 55-period window and for computing price deltas of 1\%, 2.5\%, and 5\%.

\subsubsection{Exponential Moving Average (55)}
An EMA\(_{55}\) at time \(t\) (denoted as \(\text{EMA}_{55}(t)\)) can be computed by:
\begin{equation}
\text{EMA}_{55}(t) = \alpha \cdot \text{Price}(t) \;+\; \bigl(1 - \alpha\bigr) \cdot \text{EMA}_{55}(t-1),
\end{equation}
where
\begin{equation}
\alpha = \frac{2}{55 + 1} = \frac{2}{56}.
\end{equation}

\subsection{Orderbook Deltas}

We define \(\Delta_{1\%}\), \(\Delta_{2.5\%}\), and \(\Delta_{5\%}\) as follows:

\begin{align}
\Delta_{1\%}(t)   &= 0.01 \cdot P(t), \\
\Delta_{2.5\%}(t) &= 0.025 \cdot P(t), \\
\Delta_{5\%}(t)   &= 0.05 \cdot P(t).
\end{align}

Here, \(P(t)\) denotes the current market price (for example, the midpoint between the best bid and ask, or the last traded price). Each \(\Delta\) indicates how far away from \(P(t)\) we measure or place an order in the orderbook.

For instance, you could place an order on the ask side at \(P(t) + \Delta_{1\%}(t)\) or on the bid side at \(P(t) - \Delta_{1\%}(t)\) for a 1\% offset from the current price.


\section{Strategies}
\subsection{Bias}
\subsection{Risk Managment}
\subsection{Finding fitting strategy}
\subsubsection{EMA + Orderbook delta}
\subsubsection{Bias + trailing SL}

\section{Singal processing}


\section{Implementation and Operation}
Discuss the programming tools, security measures, and other implementation details.

\section{Monitoring}

\end{document}
