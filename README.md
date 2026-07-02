Sistema de Detección de Incendios Forestales con Inteligencia Artificial

Sistema integral que utiliza técnicas de Deep Learning (Redes Neuronales Convolucionales) para identificar la presencia de fuego o humo en imágenes del entorno forestal. Este proyecto incluye el modelo entrenado, el dataset procesado y una interfaz web intuitiva para facilitar la vigilancia y alerta temprana.

Características principales

- **Modelo de IA especializado**: Entrenado con un conjunto de datos balanceado para distinguir entre "Incendio", "Humo" y "Sin peligro".
- **Interfaz web interactiva**: Permite cargar imágenes, visualizar resultados y obtener porcentajes de confianza en tiempo real.
- **Escalabilidad**: Diseñado para ser integrado con sistemas de vigilancia por cámaras (CCTV) o drones.
- **Dashboard simple**: Muestra estadísticas básicas y alertas visuales cuando se detecta una anomalía.

Estructura del proyecto

/
├── dataset/                # Conjunto de datos (imágenes clasificadas)
│   ├── fire/               # Imágenes con fuego visible
│   ├── smoke/              # Imágenes con humo
│   └── non_fire/           # Imágenes de bosque seguro (clase negativa)
├── web-app/                # Código fuente de la aplicación web
│   ├── app.py              # Backend (Flask / FastAPI / Django)
│   ├── static/             # Archivos CSS, JS e imágenes del frontend
│   └── templates/          # Vistas HTML
├── models/                 # Modelos pre-entrenados guardados (.h5 o .pth)
├── notebooks/              # (Opcional) EDA y entrenamiento experimental
├── requirements.txt        # Dependencias del proyecto
└── README.md               # Este archivo

Instalación y uso
Sigue estos pasos para ejecutar el proyecto en tu máquina local:

Clona el repositorio:


git clone https://github.com/TU-USUARIO/NOMBRE-DEL-REPO.git
cd NOMBRE-DEL-REPO
Crea un entorno virtual (recomendado):


python -m venv venv
source venv/bin/activate  # En Windows: venv\Scripts\activate
Instala las dependencias:


pip install -r requirements.txt
Ejecuta la aplicación web:


python web-app/app.py
Abre tu navegador y ve a http://localhost:5000.

📊 Entrenamiento del modelo (Opcional)
Si deseas reentrenar el modelo con tu propio dataset o ajustar hiperparámetros, ejecuta el notebook ubicado en:


notebooks/entrenamiento.ipynb
Asegúrate de tener una GPU (NVIDIA CUDA) para acelerar el proceso, o usa Google Colab.
