Función read_bin_packing_instance:

Lee el archivo de instancia.
Extrae el número de problemas (P).
Para cada problema, lee el identificador, la capacidad del contenedor, el número de objetos y el número de contenedores de la mejor solución conocida.
Almacena estos datos en una lista de tuplas.

Función bin_packing_glpk:

Define y resuelve el problema de bin packing utilizando JuMP y GLPK.
Modela las variables binarias x[i,j] y y[i].
Agrega las restricciones necesarias.
Define la función objetivo para minimizar el número de contenedores utilizados.
Resuelve el modelo y devuelve los resultados.

Función bin_packing_cbc

Define y resuelve el problema de bin packing utilizando JuMP y Cbc.
Modela las variables binarias x[i,j] y y[i].
Agrega las restricciones necesarias.
Define la función objetivo para minimizar el número de contenedores utilizados.
Resuelve el modelo y devuelve los resultados.

Función process_and_solve:

Lee y procesa las instancias de bin packing desde un archivo.
Para cada problema, llama a bin_packing_glpk y muestra el resultado junto con la mejor solución conocida.