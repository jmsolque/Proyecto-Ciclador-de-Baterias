# Proyecto-Ciclador-de-Baterias
Este repositorio contiene los archivos correspondientes a un ciclador de módulos de baterías.

## Documentación

### Componentes Utilizados
<div align="center">

| Componente | Cantidad | Modelo | Utilización |
|:----------:|:-----------:|:-----------:|:-----------:|
| Fuente de tensión | 1 | x | Alimentar algunos de los componentes utilizados. |
| x | x | x | x. |
| x | x | x | x. |
| Transistor NPN | 2 | TIP120 | Uno para carga y otro para descarga. |
| Inductor 10µH   | 2 | x | Dos, para regular corriente de carga y descarga y poder utilizar el sistema de control. |
| Amplificador Operacional | 1 | LM353 | Controlar si funciona el circuito de carga o de descarga. |
| Sensores de Corriente | 2 | x | Para medir las corrientes de carga y descarga. |
| Delfino | 1 | C2000 | Controlador. |
| Medidor de Tensión | 1 | x | Incorporado en el C2000, para medir la tensión de la batería. |
| Convertidor Digital Analógico | 1 | x | Controlar si descarga o carga. |

</div>

### Ecuaciones utilizadas

La ecuación utilizada para el circuito de carga es:

$$
V_{carga} = L\frac{di_c}{dt} + V_{batería} 
$$

De donde se tiene que:

$$
V_{carga} = V_{cc} + V_{cp} 
$$

Con base en lo anterior, se considera que: 
$$ 
V_{cp} = V_{\text{batería}} 
$$

Esta igualdad se logra mediante un sistema de prealimentación que compensa la caída de tensión en los elementos intermedios y asegura que el valor aplicado en el punto de control coincida con el voltaje real de la batería.


Por lo cual se tiene que:

$$
\frac{di_c}{dt} = \frac{V_{cc}}{L}
$$

Y de esta forma la función de transferencia será:

$$
\frac{i_c(s)}{V_{cc}(s)} = \frac{1}{Ls}
$$

De forma similar se tendrá para el el circuito de descarga, para el cual lo de realizar los cálculos pertinentes se tendría que la función de transferencia sería.

$$
\frac{i_c(s)}{V_{dc}(s)} = -\frac{1}{Ls}
$$

Donde \({V_{dc}\) es la tensión de descarga.

## [PLECS](PLECS/)

En esta sección se encuentra el código utilizado para la implementación en PLECS y así poder utilizar un C2000, en esta misma también se muestran las simualciones.

## Arvhivos para la impresión de la PCB

.

## Simulaciones

.

## Imágenes del proyecto

.