
```{note}
AbiPy provides two different APIs to produce figures either with matplotlib or with plotly.
In this tutorial, we will use the plotly API as much as possible although it should be noted
that not all the plotting methods have been yet ported to plotly.

AbiPy uses a relatively simple rule to differentiate between the two plotting libraries:
if an object provides an `obj.plot` method producing a matplotlib plot, the corresponding
native plotly version (if available) is named `obj.plotly`.
Note that plotly requires a web browser hence the matplotlib version is still valuable if you need to
visualize results on machines in which only the X-server is available.

In AbiPy versions greater than 0.9, it is possible to try converting matplotlib figures produce by `plot` methods 
into Plotly figures using the optional argument `plotly=True`, although the result is not always guaranteed.
```
