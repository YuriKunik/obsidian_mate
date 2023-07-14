
## Definiciones

1. Período: Tiempo mínimo que tarda una señal en repetirse. 
2. Frecuencia: Cuantas repeticiones hay en un segundo. 
3. Tiempo total: La duración total de la medición.
4. Número de Samples: Cantidad total de muestras en una señal discreta.
5. Frecuencia de Sampleo: Cuantos sampleos hay en una unidad de tiempo.
6. Amplitud: Valor máximo de la señal.
7. Paso temporal: Magnitud del paso temporal de muestreo en una señal discreta.

## Relaciones

$\text{Frecuencia} =\frac{1}{\text{Período}}$  
$\text{Frecuencia\_sampleo} = \frac{1}{\text{Paso\_temporal}}$
$\text{Núm\_samples} = \text{Tiempo\_total }\times \text{Frecuencia\_sampleo}$
$\text{Tiempo\_total} = \text{Núm\_samples} \times \text{Paso\_temporal}$

## Usos 

Para obtener un vector `[0,1,2,3,4,5,6,7,8,9]` que tiene:

n_samples = 10
paso_temporal = 1
t0 = 0
tf = 9

Hacemos
```python
np.arange(t0,tf+paso_temporal,paso_temporal)
# o
np.linspace(t0, tf, n_samples)
```
