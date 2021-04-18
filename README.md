# PLL40
Colección para IceStudio con las primitivas SB_PLL40.

Los parámetros para el PLL se puede obtener con la utilidad `icepll` de `IceStorm`. Por ejemplo:

```
$ icepll -i 12 -o 60

F_PLLIN:    12.000 MHz (given)
F_PLLOUT:   60.000 MHz (requested)
F_PLLOUT:   60.000 MHz (achieved)

FEEDBACK: SIMPLE
F_PFD:   12.000 MHz
F_VCO:  960.000 MHz

DIVR:  0 (4'b0000)
DIVF: 79 (7'b1001111)
DIVQ:  4 (3'b100)

FILTER_RANGE: 1 (3'b001)
```

En este caso, los parámetros serían:

```
FEEDBACK="SIMPLE"
DIVR=0
DIVF=79
DIVQ=4
FILTER_RANGE=1
```

Más información en los documentos de Lattice, por ejemplo:

https://www.latticesemi.com/-/media/LatticeSemi/Documents/TechnicalBriefs/SBTICETechnologyLibrary201508.ashx?document_id=51401
