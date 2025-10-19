# Trabajo Práctico - Procesamiento Digital de Imágenes

## Descripción del Proyecto

Este repositorio contiene la implementación completa del primer trabajo de Vision por computador, que abarca cinco áreas fundamentales: calibración de cámaras, transformaciones de intensidad, transformaciones geométricas, análisis de histogramas y segmentación por color. El proyecto está desarrollado en Python utilizando OpenCV, NumPy, Matplotlib y otras librerías especializadas.

## Estructura del Proyecto

```
Trabajo_01_Quartz_Meditativo/
├── Calibracion_camara/                    # Calibración de cámara y corrección de distorsión
│   ├── calibracion_paso_a_paso.ipynb     # Notebook principal de calibración
│   ├── images/                           # Imágenes de buena calidad
│   ├── images_opencv/                    # Imágenes de OpenCV
│   ├── images_resized_1438x1080/         # Imágenes redimensionadas de buena calidad
│   ├── images3/                          # Imágenes de mala calidad
│   └── imgs_to_correct/                  # Imágenes para probar la corrección de distorsión
├── Transformaciones_Dia_Noche/           # Transformaciones de intensidad
│   ├── Transformación_imagenes.ipynb     # Notebook de transformaciones
│   ├── casa_dia.jpg                     # Imagen de fachada en día
│   └── casa_noche.jpg                   # Imagen de fachada en noche
├── Rotacion_Traslacion_Ecualizacion/    # Transformaciones geométricas (rotación, traslación) y ecualización de histograma
├── Segmentacion/                         # Segmentación por color
│   ├── segmentacion_por_color.ipynb     # Notebook de segmentación
│   ├── input/                           # Imágenes de entrada
│   └── output/                          # Resultados de segmentación
├── requirements.txt                      # Dependencias del proyecto
├── Trabajo_01.md                        # Reporte del trabajo
└── README.md                            # Este archivo
```

### Reporte técnico del trabajo
[!IMPORTANT]
> [Reporte técnico del trabajo](https://github.com/spalaciobUNAL/Trabajo_01_Quartz_Meditativo/blob/main/Trabajo_01.md)

## Requisitos del Sistema

- Python 3.8 o superior
- Jupyter Notebook/Lab
- Cámara web o dispositivo móvil (*opcional* en caso de replicar con otras imágenes)

## Instalación

### 1. Clonar el repositorio

```bash
git clone https://github.com/spalaciobUNAL/Trabajo_01_Quartz_Meditativo.git
cd Trabajo_01_Quartz_Meditativo
```

### 2. Crear entorno virtual (recomendado)

```bash
# Crear entorno virtual
python -m venv venv

# Activar entorno virtual
# En Windows:
venv\Scripts\activate
# En Linux/Mac:
source venv/bin/activate
```

### 3. Instalar dependencias

```bash
pip install -r requirements.txt
```

## Ejecución

### 1. Calibración de Cámaras

```bash
cd Calibracion_camara
jupyter notebook calibracion_paso_a_paso.ipynb
```

### 2. Transformaciones de Intensidad

```bash
cd Transformaciones_Dia_Noche
jupyter notebook Transformación_imagenes.ipynb
```

### 3. Transformaciones Geométricas (Rotación y Traslación) y ecualización de histograma

```bash
cd Rotacion_Traslacion_Ecualizacion
jupyter notebook Rotacion_Traslacion_Ecualizacion.ipynb
```

### 4. Segmentación por Color

```bash
cd Segmentacion
jupyter notebook segmentacion_por_color.ipynb
```

## Dependencias

El proyecto utiliza las siguientes librerías principales:

- **OpenCV** (>=4.8): Procesamiento de imágenes y visión computacional
- **NumPy** (2.3.4): Operaciones numéricas
- **Matplotlib** (3.10.7): Visualización de datos
- **Pandas** (2.3.3): Análisis de datos
- **JupyterLab** (>=4.0): Entorno de desarrollo interactivo
- **Pillow**: Procesamiento de imágenes adicional

## Autores

- Sebastián Palacio (spalaciob@unal.edu.co)
- Juan Manuel Sanchez Restrepo (jsanchezrestrepo@unal.edu.co)
- Henrry Uribe Cabrera Ordonez (hcabrerao@unal.edu.co)
- Laura Sanin Colorado (lsaninc@unal.edu.co)

