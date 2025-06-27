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
    contourpy==1.3.2
    cycler==0.12.1
    et_xmlfile==2.0.0
    fonttools==4.58.4
    fpdf==1.7.2
    joblib==1.5.1
    kiwisolver==1.4.8
    matplotlib==3.10.3
    numpy==2.3.1
    openpyxl==3.1.5
    packaging==25.0
    pandas==2.3.0
    pillow==11.2.1
    pyparsing==3.2.3
    python-dateutil==2.9.0.post0
    pytz==2025.2
    scikit-learn==1.7.0
    scipy==1.16.0
    seaborn==0.13.2
    six==1.17.0
    tabulate==0.9.0
    threadpoolctl==3.6.0
    tzdata==2025.2

