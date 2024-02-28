
## Ceros de una función analítica

Sea $f:U\to \mathbb{C}$ una [[Función analítica]] con $U$ abierto y conexo. Si $f$ no es constante en $U$ entonces sus ceros son aislados.

### Demostración

Sea $V \subset U$ el conjunto de ceros no aislados de $f$, tenemos que $V$ que es un conjunto cerrado ya que, para todo $z_{0}\notin V$ y es un cero, existe un disco tal que $f$ no se anula ahí (salvo en $z_{0}$). Si $z_{0} \notin V$ y no es un cero también tenemos un entorno donde no se anula por ser $f$ continua. La proposición [[Yoga de funciones analíticas#Analítica con ceros no aislados]] nos dice que los ceros no aislados vienen en entornos, por lo que $V$ va a ser union de entornos de ceros no aislados de $f$, lo que nos da que $V$ es un abierto. Con esto $V$ es abierto y cerrado, por lo que $V=\emptyset$ o $V=U$.

## Observación

Con esto, si tenemos dos funciones que coinciden en un abierto y ambas están definidas en un abierto conexo más grandes, son iguales. Esto nos permite extender una función a un dominio más grande de forma única. Resumimos ésto en el siguiente corolario

## Coincidencia en un conexo

Sean $U$ abierto conexo y $f:U \to \mathbb{C}$ analítica. Si $f \equiv 0$ en un abierto no vacío $V \subset U$ entonces $f \equiv 0$. En particular, si dos funciones analíticas definidas en $U$ coinciden en un abierto no vacío, entonces son iguales.
