# Customer & Sales Insights Report 📊

Este proyecto demuestra un flujo completo de análisis de datos mediante un pipeline ETL moderno organizado en capas: **bronze**, **silver**, **gold** y **platinum**. Se genera un informe automatizado en PDF a partir de datos unificados de ventas, clientes, productos y representantes comerciales.

## 🔁 Data Flow (ETL)

    A[Raw CSV files] --> B[Bronze Layer<br>Raw ingestion]
    B --> C[Silver Layer<br>Cleaned & Typed]
    C --> D[Gold Layer<br>Business Logic]
    D --> E[Platinum Layer<br>Unified Dataset]
    E --> F[PDF Report Generation]

## Estructura del repositorio
    📁 bronze                   → 📄 Archivos originales (raw)
    📁 outputs
            /reports/           → 📄 Reporte final PDF
            /data_catalog/      → 📄 Data Catalog xlsx
            /rejects/           → 📄 Sales records rejected due to wrong Date
                                → 📄 visits records rejected due to wrong Date
            /review_sales/      → 📄 Bronze sales in xlsx
                                → 📄 Gold sales in xlsx
    📁 platinum/                → 📄 Datos de ventas unificados para analisis
    📄 README.md                → 📄 Readme

## 📈 Informe generado
El informe PDF incluye:

    Análisis de crecimiento de clientes

    Ventas por categoría de producto y región

    Top 10 representantes de ventas

    Relación descuentos vs ventas

    Gráficos y visuales detallados

## 📌 Tecnologías usadas
    Python 3

    Pandas

    Seaborn / Matplotlib

    FPDF2

    ETL estructurado por capas
