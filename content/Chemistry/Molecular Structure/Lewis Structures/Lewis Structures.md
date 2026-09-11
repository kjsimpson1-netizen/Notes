A Lewis structure shows how [[Chemistry/Basic Chemistry/Valence Electrons]] are shared in a molecule. This model is approximate because it shows that the electrons are shared between the atom in [[Chemistry/Atomic Structure and Properties/Bond/Covalent Compounds]], however it assumes that all the electrons are equally shared, and that they are not pulled more strongly by the ions with higher [[Chemistry/Atomic Structure and Properties/Periodic Properties/Electronegativity]]. The [[Chemistry/Basic Chemistry/Valence Electrons]] that do not form bonds are called lone pairs
```tikz
\usepackage{chemfig}

\begin{document}
\chemfig[atom sep=1, bond offset=2pt,]
{%
\lewis{1:3:,O}
(-[:-37.75]H)
(-[:-142.25]H)
(-[:90]H)
}%
\end{document}
```

