# Entrega para Google Colab — Subte BA 2014-2019

Carpeta mínima e indispensable para ejecutar `01_analisis_subte.ipynb` en Google Colab, sin descargar los datos originales ni ejecutar el ETL.

## Contenido

```
entrega_colab/
├── 01_analisis_subte.ipynb          # Notebook listo para ejecutar
├── README.md                        # Este archivo
├── data/processed/                  # 11 tablas procesadas que lee el notebook
└── outputs/
    ├── figures/                     # 13 figuras que muestra el notebook
    ├── tables/
    │   └── tabla_robustez_elasticidad.csv
    └── resultados.json              # Resultados de la sección final
```

No se incluyen los archivos crudos de `datasets/` (~6 GB), la base DuckDB ni los scripts de ETL: el notebook solo necesita las tablas agregadas, las figuras y los resultados.

## Cómo ejecutarlo en Colab

1. Subir la carpeta `entrega_colab` completa a Google Drive (por ejemplo, en `Mi unidad/entrega_colab`).
2. En Colab: **Archivo → Abrir notebook → Google Drive** y elegir `entrega_colab/01_analisis_subte.ipynb`.
3. Ejecutar **Entorno de ejecución → Ejecutar todas**.
   - La primera celda busca la carpeta del proyecto automáticamente y, si está en Drive, solicita montarlo y autorizar el acceso.
   - No hace falta instalar nada: `pandas`, `numpy`, `matplotlib`, `IPython` y `statsmodels` ya vienen preinstalados en Colab.

### Alternativa: subir el ZIP a `/content`

También se puede comprimir la carpeta, subir el ZIP desde el panel **Archivos** de Colab y descomprimirlo:

```python
!unzip -q -o entrega_colab.zip -d /content
```

Luego abrir el notebook y ejecutar todas las celdas. La primera celda detecta la carpeta en `/content/entrega_colab`.

## Requisitos

- Google Colab (Python 3.10 o superior).
- Librerías: `pandas`, `numpy`, `matplotlib`, `statsmodels` (preinstaladas en Colab).

## Notas

- El notebook solo lee archivos: no modifica datos ni genera archivos nuevos.
- Si se ejecuta localmente, abrir el notebook desde esta misma carpeta para que la primera celda encuentre `data/processed/`.
