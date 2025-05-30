<!DOCTYPE html>
<html lang="es">
<head>
  <meta charset="UTF-8">
  <title>Proceso de Preparación y Análisis de Datos</title>
  <style>
    body {
      font-family: "Georgia", serif;
      background-color: #fff;
      color: #222;
      max-width: 900px;
      margin: 2rem auto;
      padding: 0 1rem;
    }
    h1 {
      text-align: center;
      margin-bottom: 0.5rem;
    }
    .subinfo {
      text-align: center;
      font-style: italic;
      margin-bottom: 1rem;
      color: #555;
    }
    .paso {
      margin-bottom: 3rem;
      border-bottom: 1px solid #ccc;
      padding-bottom: 2rem;
    }
    .paso img {
      width: 100%;
      height: auto;
      border: 1px solid #ccc;
      margin-top: 1rem;
    }
    .paso h2 {
      color: #003366;
    }
    .paso p {
      text-align: justify;
    }
  </style>
</head>
<body>

  <h1>Proceso de Preparación y Análisis de Datos</h1>

  <p class="subinfo">Elaborado por: Tomás González y Sebastián Salamanca</p>
  <p class="subinfo">Sección: BIY7131-001D</p>
  <p class="subinfo">Profesor: Fernando Esteban Fuentes Gallegos</p>
  <p class="subinfo">Evaluación Parcial 2</p>

  <div class="paso">
    <h2>Paso 1: Creación del Bucket</h2>
    <p>Se crea el bucket con el nombre correspondiente al formato “nombre-alumno”, cumpliendo con las indicaciones del entorno de almacenamiento.</p>
    <img src="1.png" alt="Paso 1">
  </div>

  <div class="paso">
    <h2>Paso 2: Carga del Excel</h2>
    <p>Se sube al bucket el archivo Excel que contiene los registros en bruto de los avistamientos para su procesamiento.</p>
    <img src="2.png" alt="Paso 2">
  </div>

  <div class="paso">
    <h2>Paso 3: Carga a Alteryx (Dataprep)</h2>
    <p>Se importa el archivo Excel a la herramienta Alteryx (Dataprep by Trifacta) para iniciar la preparación de los datos.</p>
    <img src="3.png" alt="Paso 3">
  </div>

  <div class="paso">
    <h2>Paso 4: Integración al Flow</h2>
    <p>El Excel es vinculado a un flujo de trabajo (flow) para su análisis dentro de la plataforma.</p>
    <img src="4.png" alt="Paso 4">
  </div>

  <div class="paso">
    <h2>Paso 5: Visualización de Datos en Bruto</h2>
    <p>Se revisa el contenido original del archivo para identificar los campos disponibles y su estado.</p>
    <img src="5.png" alt="Paso 5">
  </div>

  <div class="paso">
    <h2>Paso 6: Transformaciones en la Recipe</h2>
    <p>Se aplican transformaciones visibles en la receta (recipe), como limpieza de datos, renombre de columnas y filtrado de campos.</p>
    <img src="6.png" alt="Paso 6">
  </div>

  <div class="paso">
    <h2>Paso 7: Datos Transformados</h2>
    <p>Se muestran los datos ya transformados y preparados para su análisis, listos para su uso.</p>
    <img src="7.png" alt="Paso 7">
  </div>

  <div class="paso">
    <h2>Paso 8: Creación del Job</h2>
    <p>Se ejecuta el job de exportación para generar una tabla con los datos tratados en BigQuery.</p>
    <img src="8.png" alt="Paso 8">
  </div>

  <div class="paso">
    <h2>Paso 9: Tabla en BigQuery</h2>
    <p>Validación de que la tabla fue correctamente creada en el entorno de BigQuery con los datos procesados.</p>
    <img src="9.png" alt="Paso 9">
  </div>

  <div class="paso">
    <h2>Paso 10: Consulta SQL</h2>
    <p>Se formula una consulta SQL para extraer las 5 formas de objetos más reportadas en los registros de avistamientos.</p>
    <img src="10.png" alt="Paso 10">
  </div>

  <div class="paso">
    <h2>Paso 11: Resultados de Consulta</h2>
    <p>Resultados obtenidos de la consulta, ordenados por frecuencia, lo que permite interpretar los datos más relevantes.</p>
    <img src="11.png" alt="Paso 11">
  </div>

  <div class="paso">
    <h2>Paso 12: Consulta SQL para Análisis Cantidad de avistamiento por año</h2>
    <p>Resultados de cantidad de avistamientos por año de forma descendente.</p>
    <img src="13.png" alt="Consulta SQL BigQuery por estado">
  </div>

  <div class="paso">
    <h2>Paso 13: Visualización Gráfica</h2>
    <p>Gráfico generado a partir de los datos procesados, evidenciando visualmente las principales formas reportadas.</p>
    <img src="12.png" alt="Paso 12">
  </div>

  <div class="paso">
    <h2>Paso 14: Visualización y Análisis</h2>
    <p>Con base en la consulta anterior, se genera una visualización que muestra el Top 10 de estados con más avistamientos. Este gráfico permite identificar que estados como California, Washington y Florida presentan una alta concentración de fenómenos reportados, lo que podría estar relacionado con la densidad poblacional o la cobertura tecnológica en esas áreas.</p>
    <img src="14.png" alt="Gráfico Top 10 estados con más avistamientos">
  </div>

  <div class="paso">
    <h2>Paso 15: Visualización</h2>
    <p>En el gráfico se puede visualizar la cantidad de avistamientos por estados dentro de Estados Unidos de forma descendente.</p>
    <img src="15.png" alt="Gráfico Top 10 estados con más avistamientos">
  </div>

  <div class="paso">
    <h2>Paso 16: Conclusiones</h2>
    <p>El flujo de trabajo completo permitió transformar datos en bruto en información valiosa mediante la carga, limpieza y análisis en Google Cloud Platform. Se recomienda profundizar en los análisis por año, tipo de avistamiento y contexto temporal para establecer correlaciones más robustas. Asimismo, mejorar la calidad del dataset y automatizar parte del pipeline aumentaría la eficiencia del proceso.</p>
  </div>

</body>
</html>
