# Proyecto-Analisis-Databricks-Spark
# Procesamiento y Análisis de Datos en la Nube: Implementación de un Pipeline ETL con Apache Spark y Databricks

Este proyecto implementa un Pipeline ETL completo (Extracción, Transformación y Carga) en el entorno de Databricks utilizando Apache Spark (PySpark y Spark SQL) y el formato Delta Lake.

---

## ⚙️ Requisitos de Ejecución

Para ejecutar este Notebook en su entorno de Databricks, siga estos pasos críticos:

### 1. Entorno Databricks
El código fue desarrollado y probado en la **Databricks Free Edition**. Se recomienda usar esta misma versión.

### 2. Creación del Clúster (Job Cluster)
Debido a las restricciones del entorno, el código **NO** se puede ejecutar haciendo clic en la celda. El cómputo debe ser provisto por un Job Cluster.

**Pasos para Ejecutar el Notebook:**

1.  **Importar el Notebook:** Importe el archivo `ETL_Spark_Project.ipynb` en su Workspace.
2.  **Verificar Rutas:** Asegúrese de que la ruta del dataset público sea la utilizada en el código:
    ```python
    csv_file_path = "/databricks-datasets/flights/departuredelays.csv"
    ```
3.  **Ejecutar como Job:**
    * Vaya a la esquina superior derecha del Notebook.
    * Haga clic en **"Schedule"** (Programar).
    * Seleccione **"Create Job"** (Crear Trabajo).
    * En la configuración del Job, haga clic en **"Create"** y luego en **"Run Now"** (Ejecutar ahora).

### 3. Visualización de Resultados

Las visualizaciones (Gráfico de Barras y Dispersión) se generan utilizando las librerías de Python **Pandas** y **Matplotlib**.

* Para ver el gráfico, debe acceder al historial de **Job Runs** (Ejecuciones de Trabajos) y hacer clic en la salida de la celda donde se ejecuta `plt.show()`.
