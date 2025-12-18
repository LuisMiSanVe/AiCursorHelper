> [Ver en ingles/See in english](https://github.com/LuisMiSanVe/GeminiCursorHelper/blob/main/README.md)
# 🖱️ Asistente del ratón con IA
[![image](https://img.shields.io/badge/Visual_Studio_Code-0078D4?style=for-the-badge&logo=visual%20studio%20code&logoColor=white)](https://code.visualstudio.com/)
[![Python](https://img.shields.io/badge/python-3670A0?style=for-the-badge&logo=python&logoColor=ffdd54)](https://www.python.org/)
[![image](https://img.shields.io/badge/Google%20Gemini-8E75B2?style=for-the-badge&logo=googlegemini&logoColor=white)](https://aistudio.google.com/app/apikey)

Asistente de IA que te ayuda a localizar y abrir programas usando texto o voz.

## 📝 Explicación de Tecnología
El programa toma una captura de pantalla de tu pantalla actual y se la manda a Gemini con este [prompt](https://github.com/LuisMiSanVe/GeminiCursorHelper/blob/main/GeminiCursorHelper.py#L78) para que identifique la localización del programa solicitado y (si está marcado) que intente abrirlo.

Se recomienda usar el programa con un fondo simple, donde los iconos de los programas son más faciles de ver.

Actualmente, usa `Gemini Flash 2.5`, el modelo más reciente y avanzado, aún así, de vez en cuando cometerá errores, que se esperan que se vayan arreglando con nuevas versiones.

> [!IMPORTANT]
> Sé consciente que Gemini no conoce los programas instalados en tu dispositivo y puede cometer errores, por lo que activa el *check* para dejar que Gemini intente abrir solo si sabes que nada inesperado pueda ocurrir.

## 📋 Prerequisitos
Necesitarás dos cosas para usar este programa: una API Key de Gemini e instalar las librerias necesarias de Python.

Obten tu clave de la API de Gemini yendo aquí: [Google AI Studio](https://aistudio.google.com/app/apikey). Asegúrate de tener tu sesión de Google abierta, y entonces dale al botón que dice 'Crear clave de API' y sigue los pasos para crear tu proyecto de Google Cloud y conseguir tu clave de API. **Guárdala en algún sitio seguro**.  
Google permite el uso gratuito de esta API sin añadir ninguna forma de pago, pero con algunas limitaciones.

En Google AI Studio, puedes monitorizar el uso de la IA haciendo clic en 'Ver datos de uso' en la columna de 'Plan' en la tabla con todos tus proyectos. Recomiendo monitorizarla desde la pestaña de 'Cuota y límites del sistema' y ordenando por 'Porcentaje de uso actual', ya que es donde más información obtienes.

Entonces, descarga o clona el script de Python y ejecuta este comando en la misma carpeta:
```
python pip install pystray pillow speechrecognition google-generativeai pyaudio pyautogui
```
O si falla o tienes una version de Python diferente:
```
py -m pip install pystray pillow speechrecognition google-generativeai pyaudio pyautogui
```

## 💻 Tecnologías usadas
- Lenguaje de programación: [Python](https://www.python.org/)
- Librerías:
  - [tkinter](https://docs.python.org/es/3.13/library/tkinter.html)
  - [pystray](https://pypi.org/project/pystray/)
  - [PIL](https://pypi.org/project/pillow/)
  - [io](https://docs.python.org/3/library/io.html)
  - [threading](https://docs.python.org/3/library/threading.html)
  - [speech_recognition](https://pypi.org/project/SpeechRecognition/)
  - [google.generativeai](https://pypi.org/project/google-generativeai/)
  - [pyautogui](https://pyautogui.readthedocs.io/en/latest/)
  - [re](https://docs.python.org/es/3.13/library/re.html)
- Otros:
  - [Gemini API Key](https://aistudio.google.com/app/apikey)
- IDE Recomendado: [VS Code](https://code.visualstudio.com/)
