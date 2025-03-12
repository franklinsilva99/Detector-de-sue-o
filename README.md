<h1>Detección de Sueño con Visión Artificial</h1>
Este proyecto utiliza visión artificial y aprendizaje profundo para detectar signos de sueño en tiempo real a través de la cámara web.

<h2>Descripción General</h2>
El proyecto implementa un sistema que analiza el video de la cámara web para detectar si una persona está mostrando signos de sueño. Utiliza la detección de ojos con clasificadores Haar Cascade y un modelo de aprendizaje profundo (Keras) para clasificar el estado de los ojos (abiertos o cerrados). Si se detecta que los ojos están cerrados durante un cierto período, se activa una alarma de audio.

<h2>Funcionalidades</h2>
<h4>Detección de Ojos:</h4> Utiliza clasificadores Haar Cascade para detectar los ojos en el video de la cámara web.
<h4>Clasificación de Estado de Ojos:</h4> Emplea un modelo de aprendizaje profundo (Keras) para clasificar si los ojos están abiertos o cerrados.
<h4>Detección de Sueño:</h4> Monitorea el estado de los ojos y activa una alarma de audio si se detecta que los ojos están cerrados durante un período prolongado.
<h4>Alarma de Audio:</h4> Utiliza la biblioteca VLC para reproducir un archivo de audio como alarma.
<h4>Visualización en Tiempo Real:</h4> Muestra el video de la cámara web con las detecciones y el estado del sueño en tiempo real.
<h2>Requisitos</h2>
Python 3.x, OpenCV (cv2), Keras, TensorFlow, NumPy y python-vlc
  
<h2>Instalación</h2>
<h4>Clona el repositorio:</h4>
Bash --> git clone https://github.com/cran/DELTD cd [nombre del repositorio]

<h4>Instala las dependencias:</h4>
Bash -->pip install opencv-python tensorflow keras numpy python-vlc.<br>
Asegúrate de tener los archivos haarcascade_lefteye_2splits.xml, haarcascade_righteye_2splits.xml, keras_model.h5 y audio.mp3 en el directorio del proyecto.

<h2>Uso</h2>
Ejecuta el script proyecto_v1.py:<br>
Bash --> python proyecto_v1.py<br>
El video de la cámara web se mostrará en una ventana.<br>

El sistema detectará los ojos y clasificará su estado.<br>

Si se detecta sueño, se activará la alarma de audio.<br>

Presiona la tecla 'q' para salir del programa.<br>

<h2>Estructura del Proyecto</h2>
proyecto_v1.py: Script principal del proyecto.<br>
keras_model.h5: Modelo de aprendizaje profundo entrenado para la clasificación de ojos.<br>
haarcascade_lefteye_2splits.xml: Clasificador Haar Cascade para el ojo izquierdo.<br>
haarcascade_righteye_2splits.xml: Clasificador Haar Cascade para el ojo derecho.<br>
audio.mp3: Archivo de audio para la alarma.<br>
<h2>Notas</h2>
Asegúrate de que la cámara web esté funcionando correctamente.<br>
El rendimiento del sistema puede variar según la iluminación y la calidad de la cámara.<br>
El modelo keras_model.h5 debe estar entrenado con datos de ojos abiertos y cerrados.<br>
Las rutas de los archivos de los clasificadores Haar Cascade y el archivo de audio deben ser correctas.<br>
<h2>Contribución</h2>
Las contribuciones son bienvenidas. Si encuentras algún problema o tienes alguna sugerencia, por favor abre un issue o envía un pull request.

<h2>Licencia</h2>
[Añade la licencia que desees, por ejemplo, MIT]
