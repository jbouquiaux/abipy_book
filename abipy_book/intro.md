---
jupytext:
  text_representation:
    extension: .md
    format_name: myst
    format_version: 0.13
    jupytext_version: 1.10.3
kernelspec:
  display_name: Python 3
  language: python
  name: python3
---

# Introduction

Welcome to the AbiPy Jupyter Book!
This book contains notebook-based documentation for [AbiPy](https://github.com/abinit/abipy).
This augments our Sphinx-based [documentation](https://abinit.github.io/abipy) with jupyter notebooks
containing interactive tutorials and examples.

Additional examples are available on the:

* [AbiPy plot gallery](https://abinit.github.io/abipy/gallery/index.html)
* [AbiPy flow gallery](https://abinit.github.io/abipy/flow_gallery/index.html)
* [Matgenb website](https://matgenb.materialsvirtuallab.org)

# Test Plotly Integration

```{code-cell}
import plotly.graph_objects as go
import plotly.io as pio

# Create a simple plot
pio.renderers.default = 'notebook_connected'
fig = go.Figure(data=go.Scatter(x=[1, 2, 3], y=[4, 5, 6], mode='markers'))
# Show the plot
fig
```



# test math rendering

$$
x^2 + y^2 = z^2
$$

$$
L(\hbar\omega) = \frac{1}{\hbar\omega} \int_{-\infty}^{\infty} e^{i\omega t} dt
$$