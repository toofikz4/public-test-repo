# MATH-XSS-2

Q1 mglyph: $\mglyph$ and $a_{\mglyph}$

Q2 includegraphics: $\includegraphics{x onerror=alert(1)}$

Q3 htmlClass: $\htmlClass{x}{y}$ $\htmlId{x}{y}$ $\htmlData{x}{y}$ $\htmlStyle{x}{y}$

Q4 raw-tex-html: $\html{<img src=x onerror=alert(4)>}$

Q5 enclose: $\enclose{circle}[mathcolor="red" onclick="alert(5)"]{x}$

Q6 def: $\def\x{alert(6)}\x$ and $\newcommand{\y}{z}\y$

Q7 textbf-html: $\textbf{<img src=x onerror=alert(7)>}$ $\text{<b onclick=alert(7)>x</b>}$

Q8 ce-chem: $\ce{<img src=x onerror=alert(8)>}$

Q9 fbox: $\fbox{<script>alert(9)</script>}$

Q10 colorbox: $\colorbox{red}{x}$ $\textcolor{red}{x}$
