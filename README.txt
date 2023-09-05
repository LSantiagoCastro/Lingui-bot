
LINGUI 

Chatbot inteligente entrenado para responder preguntar y redireccionar 
a los clientes a paginas web predeterminadas en los datos de entrenamiento.

El desempeño de cualquier modelo con fine-tuning es proporcional a la cantidad y calidad de
los datos de entrenamiento. Se recomienda entrenar con mas de 200 preguntas y respuestas



# Crear variable de entorno
setx OPENAI_API_KEY "YOUR-API-KEY"

# Preprocesar datos
openai tools fine_tunes.prepare_data -f <LOCAL_FILE>

# Entrenar el modelo mediante finetuning
openai api fine_tunes.create -t <LOCAL_PREPARED_FILE> -m <MODEL>

