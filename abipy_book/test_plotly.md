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



# Test Plotly Integration

```{code-cell}
import plotly.graph_objects as go
import plotly.io as pio

# Create a simple plot
fig = go.Figure(data=go.Scatter(x=[1, 2, 3], y=[4, 5, 6], mode='markers'))
# Show the plot
fig.show()
```
