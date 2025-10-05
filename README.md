# MLP_asdasd
https://github.com/WhiteSpaghet/MLP_asdasd
🖥️ Proyecto MLP Interprete – Reconocimiento de Dígitos
Descripción

Este proyecto combina aprendizaje profundo desde cero y una herramienta de alto nivel para construir redes neuronales. Permite:

MLP desde cero usando solo NumPy: implementación de neuronas, capas y propagación hacia adelante.

Intérprete de redes neuronales: un mini-lenguaje textual que se compila en modelos Keras/TensorFlow.

Versión web interactiva: dibuja dígitos y el modelo los predice en tiempo real usando Streamlit.

El objetivo es conectar conceptos matemáticos fundamentales con herramientas de alto nivel, mostrando cómo un framework de Deep Learning funciona como un compilador de operaciones neuronales.

Estructura del Proyecto
mi_proyecto_mlp_interprete/
│
├── app_web/
│   ├── app.py                # Web app con Streamlit para dibujar dígitos
│
├── notebooks/
│   └── proyecto_mlp_colab.ipynb   # Notebook Colab: MLP desde cero, intérprete y entrenamiento MNIST
│
├── src/
│   └── mnist_model.h5        # Modelo entrenado de Keras
│
├── README.md                 # Este archivo
└── requirements.txt          # Librerías necesarias

Instalación y Uso
1️⃣ Clonar repositorio
git clone https://github.com/tu_usuario/mi_proyecto_mlp_interprete.git
cd mi_proyecto_mlp_interprete

2️⃣ Entorno virtual (opcional, recomendado)
python -m venv venv
source venv/bin/activate   # Linux/macOS
venv\Scripts\activate      # Windows
pip install -r requirements.txt

3️⃣ Ejecutar Notebook en Colab

Abrir notebooks/proyecto_mlp_colab.ipynb en Google Colab
.

Ejecutar las celdas en orden:

MLP desde cero con NumPy

Interprete de redes neuronales

Entrenamiento y evaluación MNIST

4️⃣ Ejecutar la Web App (Streamlit)
cd app_web
streamlit run app.py


La aplicación permite dibujar un dígito con el mouse y predecirlo en tiempo real.

Mini-Lenguaje del Intérprete

Sintaxis:

Dense(256, relu) -> Dense(128, relu) -> Dense(10, softmax)


Dense(unidades, activación): capa completamente conectada con la función de activación especificada.

->: indica secuencia de capas.

El intérprete traduce esta sintaxis a un modelo Keras Sequential automáticamente.

Resultados

Precisión final en MNIST: ≈97%

Permite visualizar la evolución de la precisión y pérdida durante el entrenamiento.

Tecnologías y Librerías

Python 3.12

NumPy

TensorFlow/Keras

Streamlit + streamlit-drawable-canvas

Matplotlib

Licencia

MIT License – libre para uso académico y personal.
