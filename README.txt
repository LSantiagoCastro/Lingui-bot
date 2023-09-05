# Crear variable de entorno
setx OPENAI_API_KEY "YOUR-API-KEY"

# Preprocesar datos
openai tools fine_tunes.prepare_data -f <LOCAL_FILE>

# Entrenar el modelo mediante finetuning
openai api fine_tunes.create -t <LOCAL_PREPARED_FILE> -m <MODEL>