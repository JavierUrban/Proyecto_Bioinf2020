# Proyecto Copepods

## Los copépodos como modelo de estudio  
La subclase Copépoda es la más rica en especies, con >11,000 especies descritas y son los animales más abundantes en la Tierra (Jorgensen *et al.,* 2019). Los copépodos son un componente crítico de los ecosistemas marinos y de aguas continentales del mundo, son indicadores sensibles del cambio climático local y mundial, componentes clave de los servicios ecosistémicos, depredadores y parásitos de animales acuáticos económicamente importantes (Bron *et al.,* 2011). 

Los copépodos *Leptodiaptomus* son similares morfológicamente a *Leptodiaptomus sicilis* (Forbes, 1882) y habita en lagos de agua dulces y salinos que forman parte de la Cuenca Oriental en México.

### Lagos donde habita el copépodo *Leptodiaptomus*

| **Lago**      |**Salinidad** | **Peces**     |
|:----------|:----------   |:----------|
| Atexcac   | Alta      | No        |
| Carmen    | Variable  | No        |
| Preciosa  | Dulce     | Si        |
| Quechulac | Dulce     | Si        |

Las condiciones ecológicas de estos lagos en general son contrastantes, se ha estudiado el efecto de la salinidad variable como un probable promotor de la adaptación local de los copépodos *Leptodiaptomu*. Se ha demostrado que estas poblaciones presentan una divergencia ecológica en tres fenotipos diferentes: dos especializados en los lagos con salinidad alta (L. "Atexcac"), otro a salinidad baja (L. "La Preciosa" y "Quechulac") y un generalista a salinidad variable (L. "El Carmen") que habita un lago temporal con fluctuaciones de salinidad (Barrera *et al.,* 2015).

Aquí se realizo  una descripción básica de la estructura genética de estas poblaciones para inferir la divergencia genética de las poblaciones y su correlación con los patrones ecológicamente divergentes. 

Se utilizó un conjunto de 109299 SNPs para 23 individuos de cada población, estos SNPs se filtrarón en VCFtools con un maf ≤ 0.5 y un maxing-data = 1.0, y se obtuvo un nuevo conjunto con 11254 SNPs, estos se utilizaron para estimar la estructura genética de las poblaciones.


### Análisis de componentes principales con 93 individuos de 4 poblaciones del copépodo *Leptodiaptomus*
![](https://github.com/JavierUrban/Proyecto_Bioinf2020/blob/master/bin/PCAcopepods.png?raw=true)

### Árbol de Divergencia genética 
![](https://github.com/JavierUrban/Proyecto_Bioinf2020/blob/master/bin/threeDistance.png?raw=true)

La divergencia y estructura genética separan a las poblaciones del copépodo Leptodiaptomus en cuatro grupos diferentes cada uno asociado a su condición salina del lago al que pertenecen.

En general las relaciones genéticas entre poblaciones descrita aquí mantienen una correlación empiríca entre laa divergencia ambiental (particularmente con los gradientes de salinidad), y la divergencia genética, sugiriendo una probable adaptación local.


