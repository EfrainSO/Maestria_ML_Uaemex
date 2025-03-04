# Rotaciones
## Explicacion Matematica

Las rotaciones son transformaciones geométricas que mueven  uno o varios puntos en un espacio bidimensional o tridimensional alrededor de un punto central fijo, llamado centro de rotación, sin alterar la forma ni el tamaño del objeto que se está rotando. La cantidad de rotación se define por el ángulo de rotación, que generalmente se mide en grados y en ocasiones en radianes.

Las rotaciones se pueden describir utilizando matrices de rotación.

### Rotaciones en 2D
En un plano cartesiano bidimensional, una rotación se define por un ángulo $\theta$$\theta$ y un centro de rotación.

Matriz de Rotación en 2D:

La transformación de un punto $(x, y)$ $(x, y)$ a un punto rotado $(x', y')$ $(x', y')$ se realiza mediante la multiplicación por la siguiente matriz de rotación:

$$ R(\theta) = \begin{bmatrix} \cos(\theta) & -\sin(\theta) \\ \sin(\theta) & \cos(\theta) \end{bmatrix} $$$$ R(\theta) = \begin{bmatrix} \cos(\theta) & -\sin(\theta) \\ \sin(\theta) & \cos(\theta) \end{bmatrix} $$

Donde:

$\theta$$\theta$ es el ángulo de rotación en radianes (positivo para rotaciones en sentido antihorario).
$\cos(\theta)$$\cos(\theta)$ es el coseno del ángulo de rotación.
$\sin(\theta)$$\sin(\theta)$ es el seno del ángulo de rotación.
Aplicando la Rotación en 2D:

Para obtener las coordenadas del punto rotado $(x', y')$$(x', y')$, se multiplica la matriz de rotación por las coordenadas del punto original $(x, y)$$(x, y)$:

$$ \begin{bmatrix} x' \\ y' \end{bmatrix} = \begin{bmatrix} \cos(\theta) & -\sin(\theta) \\ \sin(\theta) & \cos(\theta) \end{bmatrix} \begin{bmatrix} x \\ y \end{bmatrix} $$$$ \begin{bmatrix} x' \\ y' \end{bmatrix} = \begin{bmatrix} \cos(\theta) & -\sin(\theta) \\ \sin(\theta) & \cos(\theta) \end{bmatrix} \begin{bmatrix} x \\ y \end{bmatrix} $$

Esto se traduce en las siguientes ecuaciones:

$$ x' = x \cos(\theta) - y \sin(\theta) \\ y' = x \sin(\theta) + y \cos(\theta) $$$$ x' = x \cos(\theta) - y \sin(\theta) \\ y' = x \sin(\theta) + y \cos(\theta) $$

Estas ecuaciones describen cómo las coordenadas del punto original $(x, y)$$(x, y)$ se transforman en las coordenadas del punto rotado $(x', y')$$(x', y')$ después de una rotación de ángulo $\theta$$\theta$ alrededor del origen.

### Rotaciones en 3D
Las rotaciones en el espacio tridimensional involucran rotaciones alrededor de tres ejes: x, y, z. Cada rotación se describe mediante una matriz de rotación de 3x3.

Matrices de Rotación en 3D:

Rotación alrededor del eje x:
$$ R_x(\theta) = \begin{bmatrix} 1 & 0 & 0 \\ 0 & \cos(\theta) & -\sin(\theta) \\ 0 & \sin(\theta) & \cos(\theta) \end{bmatrix} $$$$ R_x(\theta) = \begin{bmatrix} 1 & 0 & 0 \\ 0 & \cos(\theta) & -\sin(\theta) \\ 0 & \sin(\theta) & \cos(\theta) \end{bmatrix} $$

Rotación alrededor del eje y:
$$ R_y(\theta) = \begin{bmatrix} \cos(\theta) & 0 & \sin(\theta) \\ 0 & 1 & 0 \\ -\sin(\theta) & 0 & \cos(\theta) \end{bmatrix} $$$$ R_y(\theta) = \begin{bmatrix} \cos(\theta) & 0 & \sin(\theta) \\ 0 & 1 & 0 \\ -\sin(\theta) & 0 & \cos(\theta) \end{bmatrix} $$

Rotación alrededor del eje z:
$$ R_z(\theta) = \begin{bmatrix} \cos(\theta) & -\sin(\theta) & 0 \\ \sin(\theta) & \cos(\theta) & 0 \\ 0 & 0 & 1 \end{bmatrix} $$$$ R_z(\theta) = \begin{bmatrix} \cos(\theta) & -\sin(\theta) & 0 \\ \sin(\theta) & \cos(\theta) & 0 \\ 0 & 0 & 1 \end{bmatrix} $$

Combinando Rotaciones en 3D:

Para realizar rotaciones compuestas en 3D, se multiplican las matrices de rotación correspondientes. Es crucial tener en cuenta que el orden de multiplicación importa, ya que las rotaciones en 3D no son conmutativas. La rotación resultante dependerá del orden en que se apliquen las rotaciones individuales.

Ejemplo:

Para rotar un punto primero alrededor del eje x por un ángulo $\alpha$$\alpha$ y luego alrededor del eje y por un ángulo $\beta$$\beta$, se utiliza la siguiente matriz compuesta:

$$ R = R_y(\beta) R_x(\alpha) $$$$ R = R_y(\beta) R_x(\alpha) $$

La multiplicación de matrices se realiza de derecha a izquierda, lo que significa que la rotación alrededor del eje x se aplica primero.

## Aplicaciones en Ciencias de datos


