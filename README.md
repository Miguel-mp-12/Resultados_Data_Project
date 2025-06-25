# Customer & Sales Insights Report 📊

Este proyecto demuestra un flujo completo de análisis de datos mediante un pipeline ETL moderno organizado en capas: **bronze**, **silver**, **gold** y **platinum**. Se genera un informe automatizado en PDF a partir de datos unificados de ventas, clientes, productos y representantes comerciales.

## 🔁 Data Flow (ETL)

    A[Raw CSV files] --> B[Bronze Layer<br>Raw ingestion]
    B --> C[Silver Layer<br>Cleaned & Typed]
    C --> D[Gold Layer<br>Business Logic]
    D --> E[Platinum Layer<br>Unified Dataset]
    E --> F[PDF Report Generation]

## Estructura del repositorio
    📁 outputs/reports/         → 📄 Reporte final PDF
    📁 data_examples/           → 📄 Datos de muestra para ilustración (sin datos reales)
    📄 README.md                → Este archivo

## 📈 Informe generado
El informe PDF incluye:

    Análisis de crecimiento de clientes

    Ventas por categoría de producto y región

    Top 10 representantes de ventas

    Relación descuentos vs ventas

    Gráficos detallados y visuales atractivos

## 📌 Tecnologías usadas
    Python 3

    Pandas

    Seaborn / Matplotlib

    FPDF2

    ETL estructurado por capas
