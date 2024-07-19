# AI_Chatbot

Proyecto de Chatbot
Este repositorio contiene el código y los modelos para un chatbot sencillo utilizando procesamiento de lenguaje natural y aprendizaje profundo. El chatbot está diseñado para manejar consultas básicas de servicio al cliente. A continuación, se detalla la estructura del proyecto y sus componentes.

Estructura del Proyecto
chatbot.py: Este script contiene el código principal para ejecutar el chatbot.
traning.py: Este script es responsable de entrenar el modelo del chatbot.
chatbot_model.h5: El modelo entrenado en formato H5.
chatbot_model.keras: El modelo entrenado en formato Keras.
intents.json: El conjunto de datos que contiene los intents, que incluyen los patrones y respuestas.
classes.pkl: Archivo pickle que contiene las clases.
words.pkl: Archivo pickle que contiene las palabras.
Configuración y Uso
Prerrequisitos
Python 3.6 o posterior
TensorFlow
Keras
Numpy
Pickle
Instalación
Clona el repositorio:

sh
Copy code
git clone https://github.com/tuusuario/chatbot.git
cd chatbot
Instala las bibliotecas requeridas:

sh
Copy code
pip install -r requirements.txt
Entrenamiento del Modelo
Para entrenar el modelo del chatbot, ejecuta el script traning.py. Esto procesará los datos en intents.json, creará una bolsa de palabras y entrenará un modelo de red neuronal.

sh
Copy code
python traning.py
Ejecutando el Chatbot
Para ejecutar el chatbot, ejecuta el script chatbot.py. Esto cargará el modelo entrenado e iniciará el chatbot.

sh
Copy code
python chatbot.py
Datos
El archivo intents.json contiene los datos de entrenamiento para el chatbot. Incluye varios intents, cada uno con una lista de patrones y respuestas correspondientes.

Ejemplo:

json
Copy code
{
  "intents": [
    {
      "tag": "greeting",
      "patterns": ["Hola", "Hi", "Hey", "Buenos días", "Buenas tardes"],
      "responses": ["¡Hola! ¿Cómo puedo ayudarte hoy?", "¡Hola! ¿Cómo puedo asistirte?", "¡Hey! ¿En qué puedo ayudarte?"]
    },
    {
      "tag": "despedida",
      "patterns": ["Adiós", "Nos vemos luego", "Chao", "Cuídate"],
      "responses": ["¡Adiós! ¡Que tengas un gran día!", "¡Nos vemos luego! ¡Cuídate!", "¡Chao! No dudes en contactarnos si necesitas algo más."]
    },
    ...
  ]
}
Modelo
El modelo es una red neuronal simple con la siguiente arquitectura:

Capa de entrada
Dos capas ocultas
Capa de salida con activación softmax
El modelo se entrena utilizando el script traning.py y se guarda en formatos H5 y Keras.

Ejemplo de Uso
Para interactuar con el chatbot, ejecuta el script chatbot.py y escribe tus consultas. El chatbot responderá basado en el modelo entrenado.

sh
Copy code
python chatbot.py
Contribuciones
¡Las contribuciones son bienvenidas! Por favor, siéntete libre de enviar un Pull Request.

Licencia
Este proyecto está licenciado bajo la Licencia MIT.

Siéntete libre de personalizar la descripción según tus necesidades específicas.
