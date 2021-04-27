### Notebook interactivo 

La idea es averiguar cómo hacer un notebook interactivo sin necesidad de instalar programas y dependencias.

Se usarán los ejemplos de: https://ipywidgets.readthedocs.io/en/latest/examples/Using%20Interact.html


```python
from __future__ import print_function
from ipywidgets import interact, interactive, fixed, interact_manual
import ipywidgets as widgets

# Graficación y métodos numéricos
import numpy as np
import matplotlib.pyplot as plt
```


```python
def f(x):
    return x
```


```python
interact(f, x=10);
```


    interactive(children=(IntSlider(value=10, description='x', max=30, min=-10), Output()), _dom_classes=('widget-…


Ejemplo rápido: recta


```python
equis = np.linspace(1,10,100)

def recta(a,b):
    global equis
    plt.plot(a*equis + b)
```


```python
interact(recta,a=5, b=6);
```


    interactive(children=(IntSlider(value=5, description='a', max=15, min=-5), IntSlider(value=6, description='b',…



```python

```
