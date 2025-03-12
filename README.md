Detección de Sueño con Visión Artificial
Este proyecto utiliza visión artificial y aprendizaje profundo para detectar signos de sueño en tiempo real a través de la cámara web.

Descripción General
El proyecto implementa un sistema que analiza el video de la cámara web para detectar si una persona está mostrando signos de sueño. Utiliza la detección de ojos con clasificadores Haar Cascade y un modelo de aprendizaje profundo (Keras) para clasificar el estado de los ojos (abiertos o cerrados). Si se detecta que los ojos están cerrados durante un cierto período, se activa una alarma de audio.

Funcionalidades
Detección de Ojos: Utiliza clasificadores Haar Cascade para detectar los ojos en el video de la cámara web.
Clasificación de Estado de Ojos: Emplea un modelo de aprendizaje profundo (Keras) para clasificar si los ojos están abiertos o cerrados.
Detección de Sueño: Monitorea el estado de los ojos y activa una alarma de audio si se detecta que los ojos están cerrados durante un período prolongado.
Alarma de Audio: Utiliza la biblioteca VLC para reproducir un archivo de audio como alarma.
Visualización en Tiempo Real: Muestra el video de la cámara web con las detecciones y el estado del sueño en tiempo real.
Requisitos
Python 3.x
OpenCV (cv2)
Keras
TensorFlow
NumPy
python-vlc
Instalación
Clona el repositorio:

Bash

git clone https://github.com/cran/DELTD
cd [nombre del repositorio]
Instala las dependencias:

Bash

pip install opencv-python tensorflow keras numpy python-vlc
Asegúrate de tener los archivos haarcascade_lefteye_2splits.xml, haarcascade_righteye_2splits.xml, keras_model.h5 y audio.mp3 en el directorio del proyecto.

Uso
Ejecuta el script proyecto_v1.py:

Bash

python proyecto_v1.py
El video de la cámara web se mostrará en una ventana.

El sistema detectará los ojos y clasificará su estado.

Si se detecta sueño, se activará la alarma de audio.

Presiona la tecla 'q' para salir del programa.

Estructura del Proyecto
proyecto_v1.py: Script principal del proyecto.
keras_model.h5: Modelo de aprendizaje profundo entrenado para la clasificación de ojos.
haarcascade_lefteye_2splits.xml: Clasificador Haar Cascade para el ojo izquierdo.
haarcascade_righteye_2splits.xml: Clasificador Haar Cascade para el ojo derecho.
audio.mp3: Archivo de audio para la alarma.
Notas
Asegúrate de que la cámara web esté funcionando correctamente.
El rendimiento del sistema puede variar según la iluminación y la calidad de la cámara.
El modelo keras_model.h5 debe estar entrenado con datos de ojos abiertos y cerrados.
Las rutas de los archivos de los clasificadores Haar Cascade y el archivo de audio deben ser correctas.
Contribución
Las contribuciones son bienvenidas. Si encuentras algún problema o tienes alguna sugerencia, por favor abre un issue o envía un pull request.

Licencia
[Añade la licencia que desees, por ejemplo, MIT]
