# VisionComputadoraI
## Ejercicios practicos de cursada

## TP1 
branch /tp1
## Trabajo Práctico: Procesamiento de Imágenes - Balance de Blancos e Histogramas
Esta branch contiene la resolución del trabajo práctico integrador, enfocado en técnicas de balance de color y análisis estadístico de imágenes mediante histogramas. A continuación se detallan las consignas solicitadas.

---

## 📋 Consignas

### Actividad 1: Balance de Blancos con el Algoritmo White Patch
Utilizando las imágenes de entrada ubicadas en el directorio `/white_patch`:
1. **Implementación:** Desarrollar y aplicar el algoritmo *White Patch* para corregir y normalizar las desviaciones de color producidas por las diferentes fuentes de iluminación.
2. **Análisis:** Visualizar las imágenes originales junto a los resultados obtenidos tras la corrección. Realizar un análisis crítico de los resultados identificando y explicando las posibles fallas o limitaciones que presenta este método en los casos evaluados.

### Actividad 2: Análisis Comparativo de Histogramas
Para las imágenes de prueba `img1_tp.png` y `img2_tp.png`:
1. **Lectura y Visualización:** Cargar ambas imágenes utilizando OpenCV en escala de grises y proceder a su visualización.
2. **Construcción de Histogramas:** Seleccionar un número de contenedores (*bins*) adecuado para representar la distribución de intensidad. Graficar y comparar ambos histogramas de manera simultánea.
3. **Evaluación de Desempeño (Features para ML):** 
   * Explicar detalladamente las observaciones y diferencias encontradas entre ambos gráficos.
   * Responder de forma justificada: Si tuviera que entrenar un modelo de clasificación o detección de imágenes, ¿considera que los histogramas de intensidad pueden ser de utilidad para utilizarse como características (*features*) de entrada?
  
   
## TP2
branch /tp2
## Trabajo Práctico: Procesamiento de Imágenes y Video - Balance de Color, Histogramas y Enfoque

Este repositorio contiene la resolución del trabajo práctico integrador, enfocado en técnicas de balance de color, análisis estadístico de intensidad y algoritmos de detección de enfoque en dominio frecuencial. A continuación se detallan las consignas solicitadas.

---

## 📋 Consignas

### Actividad 1: Balance de Blancos con el Algoritmo White Patch
Utilizando las imágenes de entrada ubicadas en el directorio `/white_patch`:
1. **Implementación:** Desarrollar y aplicar el algoritmo *White Patch* para corregir y normalizar las desviaciones de color producidas por las diferentes fuentes de iluminación.
2. **Análisis:** Visualizar las imágenes originales junto a los resultados obtenidos tras la corrección. Realizar un análisis crítico de los resultados identificando y explicando las posibles fallas o limitaciones que presenta este método en los casos evaluados.

### Actividad 2: Análisis Comparativo de Histogramas
Para las imágenes de prueba `img1_tp.png` y `img2_tp.png`:
1. **Lectura y Visualización:** Cargar ambas imágenes utilizando OpenCV en escala de grises y proceder a su visualización.
2. **Construcción de Histogramas:** Seleccionar un número de contenedores (*bins*) adecuado para representar la distribución de intensidad. Graficar y comparar ambos histogramas de manera simultánea.
3. **Evaluación de Desempeño (Features para ML):** * Explicar detalladamente las observaciones y diferencias encontradas entre ambos gráficos.
   * Responder de forma justificada: Si tuviera que entrenar un modelo de clasificación o detección de imágenes, ¿considera que los histogramas de intensidad pueden ser de utilidad para utilizarse como características (*features*) de entrada?

### Actividad 3: Detector de Máximo Enfoque en Video (Análisis Espectral)
**Objetivo:** Implementar un algoritmo automático de detección de máximo enfoque sobre el archivo de video `focus_video.mov`, aplicando técnicas de análisis en el dominio de la frecuencia similares a las utilizadas por las cámaras digitales modernas.

1. **Métrica de Nitidez:** Desarrollar una función que, dada una imagen o región de interés (ROI), calcule la métrica propuesta en el paper *"Image Sharpness Measure for Blurred Images in Frequency Domain"*.
2. **Diseño de Experimentos:** Ejecutar la medición frame a frame bajo dos configuraciones:
   * **Experimento A:** Medición de la métrica sobre la totalidad del frame.
   * **Experimento B:** Medición sobre una región de interés (ROI) fija ubicada en el centro del frame (con un área equivalente al 5% o 10% del área total del frame).
3. **Análisis de Resultados y Automatización:**
   * Presentar las curvas temporales de la evolución de la métrica frame a frame para cada experimento. Las gráficas deben mostrar con claridad el comportamiento del algoritmo al transicionar por el punto de máxima nitidez.
   * Desarrollar e integrar un algoritmo de decisión que procese estas curvas y devuelva/etiquete de manera **automática** los frames exactos donde se produce el máximo enfoque.
  
   
