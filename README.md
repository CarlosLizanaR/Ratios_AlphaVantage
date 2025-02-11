# Análisis Financiero de Empresas

Este script en Python permite realizar un análisis financiero detallado de una empresa utilizando datos históricos de Yahoo Finance y Alpha Vantage. El análisis se enfoca en una serie de ratios financieros clave, tales como solvencia, rotación de activos e inventarios, rentabilidad, liquidez, cobertura de intereses y beneficio por acción (BPA). Los resultados del análisis se presentan tanto en gráficos como en tablas, lo que facilita la evaluación de la salud financiera de la empresa y la toma de decisiones informadas.

## Funcionalidades

El script ofrece las siguientes funcionalidades principales:

- **Entrada de usuario**: Solicita al usuario el símbolo bursátil de la empresa (por ejemplo, `NVDA` para Nvidia) y el número de períodos (en años) que desea analizar (por ejemplo, 5 o 10 años).
  
- **Cálculos de Ratios Financieros**:
  - **Solvencia**: Incluye ratios como apalancamiento y endeudamiento, para evaluar la capacidad de la empresa de cubrir sus deudas.
  - **Rotación**: Analiza la eficiencia en el uso de activos y la gestión de inventarios.
  - **Rentabilidad**: Calcula indicadores como el ROA, ROE, márgenes y BPA.
  - **Liquidez**: Evalúa la capacidad de la empresa para cubrir sus pasivos de corto plazo.
  - **Cobertura de Intereses**: Mide la capacidad de la empresa para pagar sus deudas mediante indicadores como EBIT y EBITDA.
  
- **Alertas y Promedios**: Para cada ratio, el script proporciona alertas visuales basadas en los promedios históricos de la empresa (🟢 Alto, 🟡 Moderado, 🟠 Bajo). Esto facilita la identificación de áreas críticas en la salud financiera de la empresa.

- **Presentación de Resultados**: Los resultados se muestran mediante gráficos y tablas, con análisis de tendencias a lo largo del tiempo, para proporcionar una visión integral del desempeño financiero.

## Requisitos

Este proyecto requiere **Python 3.x** y las siguientes bibliotecas:

- `https://www.alphavantage.co/query` – Para obtener datos históricos de precios y fundamentales de acciones de Alpha Vantage.
- `pandas` – Para manipulación y análisis de datos.
- `matplotlib` – Para la creación de gráficos visuales.
- `numpy` – Para cálculos numéricos y análisis de datos.

Además, el script también utiliza **Alpha Vantage** para obtener algunos de los ratios financieros. Para acceder a los datos de Alpha Vantage, necesitarás una clave API gratuita.

### Instalación de Dependencias

Puedes instalar las dependencias necesarias ejecutando el siguiente comando:

```bash
pip install -r requirements.txt

### Obtención de la Clave API de Alpha Vantage

Para poder utilizar el servicio de Alpha Vantage y obtener los datos financieros, debes tener una clave API gratuita. Puedes obtenerla registrándote en su [sitio web](https://www.alphavantage.co/support/#api-key).

## Uso

1. **Clona el repositorio**:
    ```bash
    git clone https://github.com/CarlosLizanaR/Ratios_AlphaVantage.git
    ```

2. **Accede al directorio del proyecto**:
    ```bash
    cd Ratios_AlphaVantage
    ```

3. **Ejecuta el script**:
    ```bash
    python script.py
    ```

   El script pedirá el símbolo bursátil de la empresa y el número de años a analizar. Luego, procesará los datos y mostrará los resultados en formato gráfico y tabular.

## Licencia

Este proyecto está licenciado bajo la **MIT License**. Para más detalles, consulta el archivo [LICENSE](LICENSE).
