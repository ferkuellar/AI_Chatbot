# AI_Chatbot

# Proyecto de Chatbot Conversacional

## Descripción del Proyecto

Este proyecto consiste en el desarrollo de un chatbot conversacional utilizando técnicas de procesamiento de lenguaje natural (NLP). El chatbot está diseñado para interactuar con los usuarios respondiendo a varias consultas comunes. Utiliza un modelo de aprendizaje profundo para clasificar las intenciones del usuario y proporcionar respuestas adecuadas.

## Archivos del Proyecto

- `chatbot.py`: Archivo principal que contiene el código para ejecutar el chatbot.
- `chatbot_model.h5`: Archivo del modelo entrenado en formato H5.
- `chatbot_model.keras`: Archivo del modelo entrenado en formato Keras.
- `classes.pkl`: Archivo pickle que contiene las clases del modelo.
- `intents.json`: Archivo JSON que define las intenciones y patrones del chatbot.
- `training.py`: Script utilizado para entrenar el modelo del chatbot.
- `words.pkl`: Archivo pickle que contiene las palabras del modelo.

## Estructura de Directorios

├── chatbot.py
├── chatbot_model.h5
├── chatbot_model.keras
├── classes.pkl
├── intents.json
├── training.py
└── words.pkl


## Descripción de los Archivos

### `chatbot.py`

Este archivo contiene el código principal para ejecutar el chatbot. Incluye la lógica para cargar el modelo entrenado, procesar las entradas del usuario y generar respuestas basadas en las intenciones identificadas.

### `chatbot_model.h5` y `chatbot_model.keras`

Estos archivos contienen el modelo de aprendizaje profundo entrenado. `chatbot_model.h5` es el archivo en formato H5, mientras que `chatbot_model.keras` es el archivo en formato Keras.

### `classes.pkl`

Este archivo contiene las clases del modelo en formato pickle. Las clases representan las diferentes intenciones que el chatbot puede identificar a partir de las entradas del usuario.

### `intents.json`

El archivo JSON que define las intenciones, patrones y respuestas del chatbot. Cada intención incluye una lista de patrones que el modelo utiliza para clasificar las entradas del usuario y las respuestas correspondientes que el chatbot proporciona.

### `training.py`

Este script se utiliza para entrenar el modelo del chatbot. Carga los datos de `intents.json`, procesa las palabras y clases, y entrena un modelo de red neuronal utilizando Keras.

### `words.pkl`

Este archivo contiene las palabras del modelo en formato pickle. Representa el vocabulario utilizado por el chatbot para clasificar las intenciones de las entradas del usuario.

## Cómo Ejecutar el Proyecto

1. Clona el repositorio del proyecto.
2. Instala las dependencias necesarias:
   ```bash
   pip install tensorflow keras numpy

3.Ejecuta el script de entrenamiento (opcional si deseas entrenar el modelo desde cero):

```bash
python training.py




