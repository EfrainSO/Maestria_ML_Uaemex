# Normas
## Explicacion Matematica

### Antesedente geometrico

Desde la grecia antigua se tenia la distancia euclideana la cual se define como 

$$
d(x,y) = \sqrt{ (x_1 - y_1)^2 + (x_2 - y_2)^2 + \dots + (x_n - y_n)^2 }
$$

Esto es consistente con el teorema de pitagoras de su momento

### Espacios vectoriales

En el siglo XIX se forma la teoria de espacios vectoriales, y se empiezan a estudiar a los vectores como elementos algebraicos, así aparecio la norma euclideana, que mide la longitud de un vector respecto al origen.

$$
 ||x||_2 = \sqrt{\sum_{i=1}^n x_i^2}
$$

### Casos especificos

Se investigan problemas con restricciones en cuanto a la longitud, como el caso de solo moverse de forma horizontal y vertical, ademas de identificar el valor maximo de los componentes para temas de administración de errores

$$
||x||_1 = \sum_{i=1}^n ||x_i||    
$$

$$
||x||_\infty = max|x_i|
$$

### Espacio de funciones

A principios del siglo XX se dieron cuenta que mucha ideas de algebra lineal se podian extender a espacios de funciones por lo que surgio la necesidad de normas mas flexibles para medir el tamaño de funciones. Nace la familia $L^p$

$$
||x_p|| = (\sum_{i=1}^n |x_i|^p)^{1/p}
$$

### Formalización de normas

Para poder tabajar con cualquier espacio vectorial se requiere una formalización.

1- Positividad y definitud positiva

* Se mide el tamaño por lo que no puede ser negativa

* El unico vector que debe tener tamaño 0 debe ser el vector 0

$$
||x|| \geq 0
$$
$$
||x|| = 0 \iff x=0
$$

2- Homogeneidad

* Es natural que si estiras el vector su magnitud se estira igual
* Si duplicas un vector su tamaño debe duplicarse igual

$$
||\alpha x =  ||\alpha ||x||
$$

3. Desigualdad triangular

* Que es una traducción de la distancia entre dos puntos directos siempre es menor o igual que ir dando un rode.

$$
||x+y|| \leq ||x|| + ||y||
$$


# Aplicaciones en Ciencias de datos

1- Sirve de base para algoritmos K-NN o clustering

2- Evaluación de errores en predicción

