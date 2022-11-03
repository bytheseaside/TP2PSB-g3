# Interfaz ECG - Grupo 3

<hr/>

## Integrantes

- Brisa Rojas 60535
- Camila Sobrino (agregar número)

<hr/>

## Main Window
Se decidio ... <p style='color: red'> COMPLETAR</p> 


## Conectar
Esta seccion contiene un boton que conecta la placa cyton a la computadora.

## Registro
Esta seccion contiene un boton que inicia el registro de la señal tomada de la placa cyton y uno que detiene el registro. El de finalizar
tambien guarda la señal en un archivo .csv

## Frecuencia 
Esta seccion tiene un label que muestra la frecuencia cardiaca calculada de forma online por medio del algoritmo de Pan y Tompkins y un input que permite elegir un nombre para el archivo .csv donde se guardara la señal.
En caso de no ingresarse se utiliza un nombre estandar de ECG y la fecha y hora del registro para que asi sea unico el nombre y no pise ningun archivo ya existente.

## Visualizacion
Nuestra interfaz grafica una señal tomada de la placa cyton y la grafica.

## METODOS IMPLEMENTADOS

### `def comunica_cyton(self):`
Esta funcion se encarga de conectar la placa cyton a la computadora. Para esto se utiliza la libreria OpenBCI y se crea ....<p style='color: red'> COMPLETAR</p> 

### `def iniciar_registro(self):`
Esta funcion se encarga de iniciar el flujo de informacion desde la placa hacia la computadora con el comando start_stream

Se define tambien la frecuencia de muestreo (`self.fs`) en 250Hz, se inicializan los arreglos donde se guardaran los datos como `self.vector`, `self.guardar` y `self.tiempo` y se inicializa el contador de muestras como `self.contador`. Tambien se inicializa un contador, y un timer (`self.timerB`) que se encarga de actualizar la grafica cada 2 segundos.

### `def fin_registro(self):`

### `def deteccion_QRS(self, señal, fs):`

### `def graficar(self, vector, tiempo):`

### `def bucleBCI(self):`