This is how you equations number to a math sandbox:

```
$$
g = \int_a^b f(x)dx \\
a = b + c
\tag{44}
$$
```

Result:

$$
g = \int_a^b f(x)dx \\
a = b + c
\tag{44}
$$

In the above there is only one `\tag{}` is allowed. If you want to use multiple `\tag{}` wrap them in `\begin{align}...\end{align}`:

```
$$
\begin{align}
  g &= \int_a^b f(x)dx \tag{3a} \\
  a &= b + c           \tag{3b}
\end{align}
$$
```

Result:
$$
\begin{align}
  g &= \int_a^b f(x)dx \tag{3a} \\
  a &= b + c           \tag{3b}
\end{align}
$$

You can reference an equation:
```
$$
\begin{align}
  g &= \int_a^b f(x)dx \label{eq4}\tag{4} \\
  a &= b + c \label{eq2}\tag{2}
\end{align}
$$
See equation$(\ref{eq4})$ and equation$(\ref{eq2})$
```

Result:
$$
\begin{align}
  g &= \int_a^b f(x)dx \label{eq4}\tag{4} \\
  a &= b + c \label{eq2}\tag{2}
\end{align}
$$
See equation$(\ref{eq4})$ and equation$(\ref{eq2})$


`\ref{}` only works in in MathJax, it does not work in vscode because vscode use (KeTex). `\ref{}` suppose to work on github since github uses MathJax but does some it is now broken:

---

The following suppose to work in github but it is broken
```math
\sqrt{3}
```


