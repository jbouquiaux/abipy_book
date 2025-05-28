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
fig.show()
```

# test math rendering

$$
x^2 + y^2 = z^2
$$


## From the Fermi's Golden rule to the luminescence lineshape

Following Fermi's golden rule, the absolute luminescence intensity $I(\hbar\omega)$ (number of photons per unit time per unit energy)
associated to one emitting center with two states e and g, is expressed as a function of the photon energy $\hbar\omega$ as

$$
    I(\hbar \omega)=\frac{n_D \omega^3}{3 \pi \hbar \epsilon_0 c^3} |\boldsymbol{\mu_{eg}}|^2 \delta\left(E_g-E_e-\hbar \omega\right),
$$ (first_lum_intensity)

where $n_D$ is the material refractive index,
$\boldsymbol{\mu_{eg}}=\langle\Psi_{e}|\boldsymbol{\mu}|\Psi_{g}\rangle$ is the total dipole matrix element.
