¡Claro! Analizando el documento, he desglosado los pasos y requisitos clave para la entrega de tu **Práctica Final: Informática, Algoritmos y Programación**.

Aquí tienes la guía paso a paso para desarrollar el proyecto llamado **`SoftwareEncuestas`**:

---

## 📋 **Fase 1: Preparación y Estructura del Proyecto**

1.  **Crear la Carpeta Principal:** Crea una carpeta llamada **`SoftwareEncuestas`**. Todo tu desarrollo debe estar **exclusivamente** dentro de ella.
2.  **Colocar el Archivo de Datos:** Asegúrate de colocar el archivo **`DataBase.csv`** en la raíz de la carpeta `SoftwareEncuestas`.
3.  **Definir la Estructura Modular:** Planifica y crea los archivos `.py` necesarios para lograr la modularidad requerida (se desaconseja el uso de Jupyter Notebooks). Ejemplos recomendados:
    * `main.py` (para el menú interactivo y la lógica principal)
    * `procesamiento.py` (para la lectura, filtrado y organización de datos)
    * `graficos.py` (para la generación de gráficos)
    * `utilidades.py` (para funciones auxiliares como manejo de tiempo y validaciones)
4.  **Crear el `README.md`:** Incluye un archivo `README.md` con **instrucciones claras** sobre cómo ejecutar tu programa.

## 💻 **Fase 2: Desarrollo del Programa Principal (`main.py`)**

El programa debe implementar un **menú interactivo** en consola con las siguientes opciones, y debe gestionar el flujo siguiendo el diagrama provisto.

### **Opciones del Menú (Implementación)**

| Opción | Descripción | Requisitos Clave |
| :---: | :--- | :--- |
| **1** | **Procesamiento de los Registros** | * Preguntar **nombre del archivo** (`DataBase.csv`).
| | | * Preguntar **ruta absoluta** para almacenar resultados.
| | | * Crear la estructura jerárquica de carpetas: **`SEDE / FACULTAD / PROGRAMA ACADÉMICO`**.
| | | * Guardar **CSVs filtrados por programa** en la carpeta de su respectivo programa. |
| **2** | **Datos Generales de Registro** | * Mostrar: Número de **sedes**, número de **programas académicos**, y **cantidad total de estudiantes**.
| | | * Mostrar la cantidad de registros por **género** (Hombres/Mujeres/Otro). |
| **3** | **Gráficos** | * Generar y mostrar (guardar como PNG en una subcarpeta `Resultados/` dentro de `SoftwareEncuestas`):
| | | * **Diagrama de Barras**: Hombres vs. Mujeres, discriminado por **sede**.
| | | * **Gráfico de Torta**: Porcentaje de estudiantes por **región**.
| | | * **Gráfico de Torta**: Porcentaje de estudiantes por **municipio**.
| | | * **Gráfico General**: Inspirado en el poster de Gapminder. |
| **4** | **Ingresar Nuevos Registros** | * Preguntar **ruta absoluta** y **nombre** del archivo nuevo.
| | | * **Cargar y appendear** los nuevos datos al archivo principal (`DataBase.csv`), manteniendo la consistencia de los datos. |
| **5** | **Tiempo de Ejecución del Programa** | * Mostrar el tiempo total transcurrido desde el inicio del programa en formato **`HH:MM:SS`**. |
| **6** | **Salir** | * Terminar el programa de forma limpia (cerrar archivos, liberar recursos). |

## 🛠️ **Fase 3: Requisitos Técnicos y Calidad**

* **Librerías:** Utiliza `pandas`, `matplotlib`, `os`, `sys`, `time`, y `csv`. Si usas otras, debes sustentarlo.
* **Manejo de Errores:** Implementa **validaciones robustas** para:
    * Entradas de rutas válidas.
    * Existencia de archivos.
    * Formato CSV correcto.
    * Muestra mensajes de error claros al usuario.
* **Modularidad:** Asegúrate de que las funciones estén separadas por su responsabilidad.
* **Salida de Gráficos:** Los gráficos deben ser claros, con títulos y leyendas, y guardarse en una subcarpeta **`Resultados/`** dentro de **`SoftwareEncuestas`**.
* **Manejo del Tiempo:** Utiliza la librería `time` para registrar el tiempo de ejecución.

## 🗓️ **Fase 4: Entrega y Sustentación**

| Hito | Fecha | Notas |
| :--- | :--- | :--- |
| **Entrega** | **2 de diciembre** | Enviar al correo: `tmaria.gaviria@udea.edu.co`. Asegúrate de que la carpeta **`SoftwareEncuestas`** contenga todos los archivos. |
| **Sustentación** | **4 de diciembre** | Prepárate para las 5 preguntas técnicas individuales sobre tu código, algoritmos, decisiones de diseño y manejo de casos límite (*edge cases*). |

---

¡Éxito con tu práctica final! ¿Te gustaría que te ayude a comenzar con la estructura de archivos en Python o a planificar la implementación de alguna de las opciones del menú?
