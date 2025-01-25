# ESP32 Telegram Bot 🤖🌐

## Descripción

Bot educativo de Telegram desarrollado con ESP32, diseñado para aprender sobre programación de microcontroladores e integración de servicios de mensajería. Ideal para proyectos de iniciación en IoT y automatización.

## Características

* Conexión WiFi con ESP32
* Integración con la API de Telegram
* Manejo de mensajes entrantes
* Ejemplo práctico de comandos básicos (encender/apagar un LED)
* Configuración de seguridad basada en ID de usuario
* Uso opcional de webhooks para la recepción de mensajes en tiempo real

## Requisitos

### Hardware
* Placa de desarrollo ESP32
* Cable USB
* Red WiFi con acceso a Internet

### Software
* Arduino IDE (versión reciente)
* Soporte para ESP32 en Arduino IDE
* Librerías necesarias:
   * **WiFi Library** (incluida en el soporte para ESP32)
   * **Universal Telegram Bot Library**

## Configuración

1. **Configurar la API de Telegram:**
   * Crear un bot con `BotFather` en Telegram
   * Obtener el token del bot y el ID del usuario autorizado

2. **Configurar Arduino IDE:**
   * Instalar el soporte para ESP32 desde el gestor de tarjetas
   * Descargar e instalar las librerías necesarias desde el gestor de librerías

3. **Definir credenciales en el código:**
   * Reemplazar las variables del código con:
      * Credenciales de la red WiFi
      * Token del bot
      * ID de usuario autorizado

## Instalación

```bash
# Clonar este repositorio
git clone https://github.com/tu-usuario/esp32-telegram-bot.git

# Abrir el archivo del proyecto en Arduino IDE
```

## Uso

1. **Subir el código a la placa ESP32:**
   * Conectar la placa al ordenador mediante USB
   * Seleccionar la placa ESP32 y el puerto en Arduino IDE
   * Compilar y subir el código

2. **Ejecutar el bot de Telegram:**
   * Iniciar el bot desde la app de Telegram
   * Enviar comandos como `/encender` o `/apagar` para controlar el dispositivo

## Aprendizaje

Este proyecto enseña los fundamentos de:
* Programación de microcontroladores con ESP32
* Uso práctico de APIs para integrar servicios externos
* Configuración de redes WiFi para IoT
* Desarrollo y seguridad de bots en Telegram

## Contribuciones

¡Las contribuciones son bienvenidas! Si encuentras errores o tienes ideas para mejorar, no dudes en crear un pull request.

## Licencia

Este proyecto está licenciado bajo la Licencia MIT.
