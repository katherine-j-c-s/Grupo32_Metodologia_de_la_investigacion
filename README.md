# Evolución del precio del boleto y la demanda de viajes en el Subte de Buenos Aires (2014–2019)

Tercera y última entrega del Trabajo Final Integrador. Licenciatura en Ciencia de Datos, Universidad del Gran Rosario.

El estudio describe la evolución del precio del boleto y de la demanda del Subte de Buenos Aires entre 2014 y 2019. Es cuantitativo, retrospectivo y de alcance descriptivo, exploratorio y correlacional. Las asociaciones no se interpretan como relaciones causales.

## Integrantes

- Katherine Contreras
- Mateo Maibach
- Joaquín Betes
- Emilce Robles
- Silvina Andrea Moyano

## Qué pide la actividad y qué se entrega

La actividad pide tres cosas. Un integrante las carga todas en la plataforma, antes del sábado 7 de noviembre de 2026 a las 23:59.

| Pedido | Dónde está |
| --- | --- |
| Informe final en PDF | El texto está en el documento del grupo. Hay que exportarlo a PDF y subirlo a la actividad. Incluye introducción y objetivos, marco teórico, metodología, desarrollo, resultados, conclusiones y bibliografía. |
| Desarrollo de la solución | Este repositorio: el notebook `entrega_colab/01_analisis_subte.ipynb` y el tablero `Entrega_Final_Proyecto_Integrador.pbix`. |
| Video de defensa, de hasta 10 minutos, con los cinco integrantes en cámara | Se sube a la actividad como archivo o como enlace de Drive con permiso de lectura. No está dentro de este repositorio. |

Las capturas del informe no reemplazan el notebook ni el archivo de Power BI.

## Cómo abrir el tablero

El archivo es `Entrega_Final_Proyecto_Integrador.pbix`, en la raíz del repositorio.

Para verlo hace falta **Power BI Desktop en Windows**. Es gratuito y se descarga desde el sitio de Microsoft: [Power BI Desktop](https://www.microsoft.com/power-platform/products/power-bi/desktop). El archivo no se abre en el navegador, en Excel ni en Google Colab.

1. Instalar Power BI Desktop.
2. Abrir `Entrega_Final_Proyecto_Integrador.pbix`.
3. Recorrer las siete pestañas de abajo. Los datos ya están cargados dentro del archivo.

Si Power BI pide la ruta de las tablas, hay que indicarle la carpeta `dashboard/datos`. Esos CSV usan punto y coma como separador y coma como decimal. En la vista previa, la primera fila de `panel_mensual` tiene que mostrar precio nominal **3,5** y precio real **8,25**. No hace falta actualizar el tablero para leerlo: los valores ya quedaron importados.

No se necesitan los históricos originales de molinetes. Esos archivos superan los 70 millones de filas y no forman parte de esta entrega. El tablero y el notebook leen tablas agregadas.

El tablero no tiene segmentadores. Cada página ya muestra el recorte que corresponde. Las páginas son estas:

| Página | Qué muestra |
| --- | --- |
| Resumen | Variación de la tarifa nominal (442,9 %), de la tarifa real (8,4 %), de la demanda (33,8 %) y elasticidad (−0,168), junto con la demanda anual y la mensual. |
| Tarifas | Serie nominal y real hasta abril de 2019, y la tabla de cada aumento. |
| Demanda | Viajes anuales, de 255 millones en 2014 a 348 millones en 2018, y la serie mensual 2014–2019. |
| Líneas y estaciones | Las seis líneas, las diez estaciones de mayor volumen y las siete estaciones nuevas. |
| Horarios | Imagen del perfil horario de 2019. Los días hábiles tienen picos cerca de las 8 y de las 17–18. |
| Tarifa y demanda | Elasticidad −0,168, elasticidad por línea y tabla de robustez. |
| Metodología | Registros leídos y válidos, cobertura de días y control de viajes. La diferencia de ese control es 0 en los seis años. |

El ingreso analítico está en el informe y en la figura 13. No está en el tablero.

## Cómo abrir el notebook

La carpeta `entrega_colab` alcanza para revisar el análisis sin volver a procesar los históricos.

1. Subir la carpeta `entrega_colab` completa a Google Drive.
2. En Colab, abrir `entrega_colab/01_analisis_subte.ipynb`.
3. Ejecutar **Entorno de ejecución → Ejecutar todas**.
4. Autorizar el acceso a Drive cuando lo pida la primera celda.

No hay que instalar librerías. Colab ya incluye pandas, NumPy, Matplotlib y statsmodels. El notebook solo lee archivos. El detalle está en `entrega_colab/README.md`.

## Contenido del repositorio

```text
├── Entrega_Final_Proyecto_Integrador.pbix   # Tablero para abrir con Power BI Desktop
├── dashboard/datos/                          # Tablas que alimentan el tablero
├── entrega_colab/
│   ├── 01_analisis_subte.ipynb               # Notebook de análisis
│   ├── data/processed/                       # Tablas agregadas que lee el notebook
│   └── outputs/
│       ├── figures/                          # Figuras 1 a 13 del informe
│       ├── tables/
│       └── resultados.json
└── README.md
```

## Qué cubre el informe

- **Introducción, problema y objetivos.** Evolución del boleto y de la demanda entre 2014 y 2019, con los objetivos actualizados según el trabajo realizado.
- **Marco teórico.** Tarifa nominal y real, demanda de transporte público y elasticidad-precio, con las citas usadas en el texto.
- **Metodología.** Estudio cuantitativo y retrospectivo. Fuentes de datos abiertos de Buenos Aires, IPC de la Ciudad y, como control, IPC nacional. Se leyeron 70.095.421 registros y quedaron 70.017.158 válidos.
- **Desarrollo.** Notebook en Python y tablero en Power BI sobre tablas agregadas. El anexo A.2 explica cada página del tablero.
- **Resultados.** Trece figuras y las tablas del capítulo 5: tarifa nominal +442,9 % y real +8,4 %, demanda +33,8 %, elasticidad −0,168.
- **Conclusiones.** Cumplimiento de los objetivos, alcance del resultado y limitaciones. El resultado no es causal.
- **Bibliografía.** Referencias en formato APA, correspondientes a las citas del texto.
