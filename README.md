# Trabajo_01_Quartz_Meditativo


# Trabajo Práctico - Procesamiento Digital de Imágenes

## Objetivos de Aprendizaje
Al completar este trabajo práctico, los estudiantes serán capaces de:
- Calibrar una cámara real y comprender los parámetros intrínsecos y extrínsecos.  
- Aplicar operaciones fundamentales de procesamiento de imágenes a nivel de píxel.  
- Implementar transformaciones geométricas (rotación, traslación).  
- Realizar corrección y mejora de imágenes mediante análisis de histogramas.  
- Implementar técnicas básicas de segmentación.  
- Documentar y comunicar resultados técnicos de manera profesional.  

> **Nota:** Es posible que se solicite a cada estudiante evaluar de forma anónima el trabajo de sus compañeros. Esta evaluación podrá incidir en la nota individual.

---

## Entregables
- Código Python organizado en **scripts** o **notebooks**.  
- `README.md` con instrucciones de instalación y ejecución.  
- Comentarios claros en todo el código.  
- Estructura de carpetas organizada.  
- `requirements.txt` con todas las dependencias.  
- Documento en formato **Markdown** o **HTML**.  
  - Extensión: **2000-3000 palabras**.  
  - Debe incluir: **teoría, metodología, resultados y análisis**.  
  - Visualizaciones de alta calidad.  
  - Referencias bibliográficas en formato **APA**.  
- Reporte de **contribución individual**.  

---

## Actividades

### 1. Calibración de Cámaras
La calibración de cámara es esencial para cualquier aplicación de visión que requiera mediciones precisas o reconstrucción 3D. Permite:  
- Corregir distorsiones de lente.  
- Establecer la relación entre coordenadas del mundo real y píxeles.  
- Obtener parámetros intrínsecos (matriz K, coeficientes de distorsión).  

📎 [Guía de calibración](https://classroom.google.com/c/NzgwMDM2NDYwMzA5/m/ODEwMDkzMTg1MTgy/details)

**Para el reporte, incluir:**
- 4-6 imágenes con las esquinas detectadas (`cv2.drawChessboardCorners()`).  
- Matriz de cámara **K**:

```text
K = [fx  0  cx]  
    [0  fy  cy]  
    [0   0   1]
```

- Coeficientes de distorsión: `k1, k2, p1, p2, k3`.  
- Error RMS de reproyección (debe ser `< 0.5 píxeles`).  
- Al menos 3 imágenes **originales vs corregidas**.  
- Evidenciar la corrección en las esquinas (donde la distorsión es mayor).  
- Responder:  
  - ¿Qué tipo de distorsión predomina (barril, cojín)?  
  - ¿La longitud focal `fx` es similar a `fy`? ¿Por qué podría diferir?  
  - ¿El punto principal `(cx, cy)` está cerca del centro de la imagen?  

---

### 2. Transformaciones de Intensidad a Nivel de Píxel
- Tomar **2 fotografías de la fachada** (6 am y 7 pm) desde el mismo punto.  
- Implementar manualmente las siguientes operaciones:  
  - Ajuste de brillo.  
  - Ajuste de contraste.  
  - Corrección gamma.  
- Operaciones combinadas:  
  - Suma `(A+B)`.  
  - Resta `(A-B)`.  
  - Multiplicación `(A*B)`.  
  - División `(A/B)`.  

---

### 3. Transformaciones Geométricas (Rotación y Traslación)
- Crear una función que:  
  1. Cargue una imagen.  
  2. Aplique **5-8 transformaciones sucesivas** (traslaciones, rotaciones, escalas).  
  3. Genere un **GIF animado o video** mostrando la secuencia.  
  4. Guarde cada frame intermedio.  

---

### 4. Distribución de Intensidades e Histogramas
- Realizar **ecualización de histograma** (usando la función de distribución acumulada) en las imágenes de la fachada.  
- Responder:  
  - ¿Qué diferencias hay entre los histogramas de la imagen de día vs la de noche?  
  - ¿Cuáles son las transformaciones de ecualización en cada caso?  

---

### 5. Segmentación de Imágenes
- Capturar una escena con objetos de distintos colores (Universidad Nacional u oficina).  
- Usar cámara de celular.  
- Implementar:  
  - Segmentación por color.  
  - Conteo de cuántos objetos de cada color hay.  
  - Cálculo del área de cada objeto.  

---
