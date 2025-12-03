# Proyecto-Ciclador-de-Baterias
Este repositorio contiene los archivos correspondientes a un ciclador de módulos de baterías.

## Documentación

### Componentes Utilizados
<div align="center">

| Componente | Modelo | Utilización |
|:----------:|:-----------:|:-----------:|
| Fuente de tensión | x | Alimentar algunos de los componentes utilizados. |
| x | x | x. |
| x | x | x. |
| x | x | x. |
| Transistor NPN| TIP120 | Dos, uno para carga y otro para descarga. |
| Inductor 10µH   | x | Dos, para regular corriente de carga y descarga y poder utilizar el sistema de control. |
| Amplificador Operacional | LM353 | Controlar si funciona el circuito de carga o de descarga. |
| Sensores de Corriente | x | Dos, para medir las corrientes de carga y descarga. |
| Delfino | C2000 | Controlador. |
| Medidor de Tensión | x | Incorporado en el C2000, para medir la tensión de la batería. |
| Convertidor Digital Analógico | x | Controlar si descarga o carga. |

</div>

### Ecuaciones utilizadas

La ecuación utilizada para el circuito de carga es:

$$
V_{carga} = L\frac{di_c}{dt} + V_{batería} 
$$



## [PLECS](PLECS/)

En esta sección se encuentra el código utilizado para la implementación en PLECS y así poder utilizar un C2000, en esta misma también se muestran las simualciones.

## Arvhivos para la impresión de la PCB

.

## Simulaciones

.

## Imágenes del proyecto

.