# ESP32 Telegram Bot 🤖🌐

[![Tutorail de conexiones](https://img.youtube.com/vi/6V0s_6FMEho/0.jpg)](https://www.youtube.com/watch?v=6V0s_6FMEho)


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

### Paso 1: Crear un bot de Telegram
1. Abre Telegram y busca `BotFather`
2. Usa el comando `/newbot` para crear un bot
3. Proporciona un nombre y un usuario para el bot
4. Copia y guarda el token generado

### Paso 2: Obtener tu ID de usuario
1. Busca `IDBot` en Telegram
2. Usa el comando `/getid` para obtener tu ID de usuario
3. Guarda este ID para configurarlo en el código

### Paso 3: Configurar Arduino IDE
1. **Agregar soporte para ESP32**:
   * Ve a **Archivo > Preferencias** y agrega este enlace en "URL de gestor de tarjetas adicionales":
     ```
     https://raw.githubusercontent.com/espressif/arduino-esp32/gh-pages/package_esp32_index.json
     ```
   * Ve a **Herramientas > Placa > Gestor de tarjetas** y busca `esp32`
   * Instala el paquete para ESP32

2. **Instalar librerías necesarias**:
   * Abre **Herramientas > Gestor de librerías**
   * Busca e instala **Universal Telegram Bot Library** desde [GitHub](https://github.com/witnessmenow/Universal-Arduino-Telegram-Bot)
   * Verifica la instalación de la librería WiFi (incluida con ESP32)

### Paso 4: Configurar credenciales en el código
1. Abre el archivo `.ino` del proyecto en Arduino IDE
2. Reemplaza las siguientes variables:
   * `WIFI_SSID` y `WIFI_PASSWORD` con credenciales de tu red WiFi
   * `TELEGRAM_BOT_TOKEN` con el token de tu bot
   * `AUTHORIZED_USER_ID` con tu ID de usuario de Telegram

## Instalación

```bash
# Clonar este repositorio
git clone https://github.com/tu-usuario/esp32-telegram-bot.git

# Abrir el archivo del proyecto en Arduino IDE
```

## Uso

1. **Subir el código a la placa ESP32:**
   * Conecta la placa al ordenador mediante USB
   * Selecciona la placa ESP32 y el puerto en Arduino IDE
   * Compila y sube el código

2. **Iniciar el bot de Telegram:**
   * Abre tu bot desde la app de Telegram
   * Envía comandos como `/encender` o `/apagar`

## Librería Universal Telegram Bot

* **Repositorio**: [Universal-Arduino-Telegram-Bot](https://github.com/witnessmenow/Universal-Arduino-Telegram-Bot)
* **Descripción**: Librería para integrar bots de Telegram en proyectos de Arduino
* **Instalación**: Disponible en el Gestor de Librerías de Arduino o mediante descarga directa desde GitHub

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
