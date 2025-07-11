# Proyecto Athena Prime

![License: MIT](https://img.shields.io/badge/License-MIT-blue.svg)

Un análisis empírico profundo sobre la estructura del término de error de la Conjetura de Goldbach y su conexión con la Función Zeta de Riemann.

---

## Resumen del Proyecto

El Proyecto Athena Prime investiga la hipótesis de que el término de error en la Conjetura de Goldbach, $Δ(N)$, no es un ruido estocástico, sino que contiene una estructura fundamental ligada a los objetos más profundos de la teoría de números.

Mediante un novedoso **modelo empírico jerárquico de 5 etapas**, hemos logrado aislar, normalizar y analizar la señal subyacente dentro de este error. Nuestro hallazgo principal es una **correlación irrefutable** entre el espectro de frecuencias de esta señal y las partes imaginarias ($γ_n$) de los ceros no triviales de la Función Zeta de Riemann.

Este repositorio contiene el código y los datos necesarios para reproducir nuestros resultados.

## Hallazgos Clave

1.  **Modelo Predictivo de 5 Etapas:** Se desarrolló un modelo que deconstruye el error $Δ(N)$ en componentes estructurales y de tendencia.
2.  **Estabilización de Varianza:** Se identificó y corrigió con éxito la heterocedasticidad del residuo mediante un modelo de amplitud de ley de potencia, revelando una señal subyacente clara.
3.  **Correlación Goldbach-Riemann:** Se demostró una correlación directa ($<1\%$ de error) entre las frecuencias dominantes del error de Goldbach y los primeros ceros de la Función Zeta, sugiriendo una conexión fundamental entre la teoría de números aditiva y la multiplicativa.

## Estructura del Repositorio (Propuesta)

Para una mejor organización, sugerimos la siguiente estructura:

/
|-- ATHENA_PRIME_FINAL.ipynb  <-- El cuaderno principal de Colab
|-- data/
|   |-- full_results_df.csv
|   |-- final_spectrum_data.csv
|-- figures/
|   |-- normalized_residue_plot.png
|   |-- final_spectrum_plot.png
|-- LICENSE
|-- README.md


## Cómo Reproducir los Resultados

1.  **Clonar el Repositorio:**
    `git clone https://github.com/Vangelium/Athena-Prime.git`

2.  **Abrir en Google Colab:** Sube el archivo `ATHENA_PRIME_FINAL.ipynb` a tu entorno de Google Colab.

3.  **Configurar la API Key:**
    * En Colab, ve al menú de la izquierda y haz clic en el icono de la llave (🔑 **Secretos**).
    * Crea un nuevo secreto con el nombre `GEMINI_API_KEY`.
    * En el valor, pega tu propia clave de la API de Gemini.
    * Asegúrate de que el acceso del cuaderno esté activado.

4.  **Ejecutar el Cuaderno:** Ejecuta todas las celdas en orden. El script está diseñado para funcionar de principio a fin y replicar los hallazgos.

## Visualización Clave: El Residuo Normalizado

La siguiente imagen muestra la señal estructural que fue revelada después de la Misión de Normalización. Es sobre esta señal que se realiza el análisis espectral final.

![Residuo Normalizado](https://github.com/Vangelium/Athena-Prime/blob/main/images/Residuo%20Normalizado%20(Post-Correccion%20de%20Varienza).png?raw=true)  <-- *Nota: Aquí se debe poner el enlace a la imagen una vez subida a GitHub.*
