# Proyecto-Capstone
Proyecto de Taller de Investigación Operativa: Planificación de mantención de Camiones

## Notas TAPR
Perdón el desorden en primer lugar, se ve como mucho código pero la carpeta para esta entrega se llama E2.

### Archivos importantes carpeta E2
1) clases: Este archivo contiene las clases __Camion__ y la clase __Simulación__.
2) distribuciones: contiene las distribuciones para los distintos tipos de falla.
3) main: es el archivo que se necesita correr para obtener los cálculos que se estimen convenientes.
4) carga_archivos: se utilizó funciones generadoras para leer todos los archivos y los datos.

#### Carpetas importantes en E2
1) KMs: contiene los archivos de curvas de Kapplan-Meir.
2) distribuciones: contiene múltiples gráficos que fueron necesarios para la simulación.

##### Otras consideraciones
- El archivo main está muy desordenado, pero lo que está en estos momentos es un ciclo que genera 50 simulaciones de 1 año con un umbral 0.6, se imprimen las distintas cantidades de falla que fue lo último que se estuvo calculando.

###### Variables de Estado
- T: Reloj Simulación
- Tfin: tiempo que demora la simulación (8760hrs)
- TPE: tiempo próxima operación. Lo que se modela es un tiempo de viaje y un tiempo de ocio, ya que cuando termina eso, podría empezar una nueva operación.
- TPE0: tiempo próxima mantención programada.
- TPEi: tiempo próxima falla i.
- Tmin: minimo tiempo entre TPE, TPE0, TPEi.
- Carga: carga de operación.

####### Medidas de desempeño iniciale
- TOperacion: tiempo en operación.
- CTT: carga total transportada.
- CFallas: cantidad de fallas.
- TReparacion: tiempo en reparación.
