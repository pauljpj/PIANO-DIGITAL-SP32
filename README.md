# PIANO-DIGITAL-SP32
Piano electrónico con conectividad en SP32
# 🎹 Proyecto: Piano Digital Educativo

## Introducción
Este proyecto consiste en el desarrollo de un **piano digital educativo** que combina hardware y software para facilitar el aprendizaje musical.  
El sistema integra una **ESP32** para la gestión de teclas y generación de señales MIDI, una **Raspberry Pi** para el procesamiento de datos y una **interfaz gráfica (GUI)** desplegada en pantallas táctiles.  
Además, se implementa un sistema en la nube para almacenar el progreso de los estudiantes y permitir a los padres y profesores hacer un seguimiento en tiempo real.

## Objetivos

### Objetivo general
Desarrollar un piano digital interactivo que permita a estudiantes aprender y practicar música de manera dinámica, registrando su progreso en la nube.  

### Objetivos específicos
- Implementar una **ESP32** para la lectura de las teclas y envío de datos MIDI.  
- Procesar la información en una **Raspberry Pi** con una GUI intuitiva.  
- Desplegar la interfaz en **dos pantallas táctiles** para interacción directa del estudiante.  
- Almacenar en la nube los datos de progreso de cada estudiante.  
- Permitir acceso mediante usuario y contraseña a padres y docentes para revisar avances.  

## Metodología / Desarrollo
1. **Diseño de Hardware**  
   - Teclas conectadas a la ESP32 (entrada digital).  
   - Conversión a mensajes MIDI.  
   - Comunicación ESP32 → Raspberry Pi vía UART/WiFi.  

2. **Procesamiento en Raspberry Pi**  
   - Recepción de datos MIDI.  
   - Visualización en una GUI desarrollada en **Python (Tkinter/PyQt/React con Electron)**.  
   - Registro de avances del estudiante.  

3. **Conexión a la nube**  
   - API para enviar datos de progreso.  
   - Base de datos en la nube (ejemplo: Firebase, MongoDB Atlas o PostgreSQL en AWS).  
   - Acceso web para padres y profesores mediante login.  

## Materiales y Herramientas
- **ESP32 Dev Kit**  
- **Módulo MIDI**  
- **Raspberry Pi 4**  
- **2 pantallas táctiles compatibles con Raspberry Pi**  
- **Software**:  
  - Python  
  - Biblioteca MIDI (mido / rtmidi)  
  - Node.js (para backend de la API)  
  - Base de datos en la nube (Firebase / PostgreSQL)  

## Diagramas
### 📌 Diagrama de Bloques
![Diagrama de Bloques](imagenes/DIAGRAMA_DE_BLOQUES.jpeg)

### 📌 Diagrama de Contexto
![Diagrama de Contexto](imagenes/DIAGRAMA_DE_SOFTWARE.jpeg)

### 📌 HMI VISUAL
![HMI](imagenes/HMI_VISUAL.jpeg)
