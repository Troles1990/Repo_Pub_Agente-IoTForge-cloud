# IoTForge Agent v2.2.2

Agente de compilación local para [IoTForge](https://iotforge.iaintegracion.space) — plataforma IoT SaaS para LATAM.

## ⬇️ Descarga

**[Descargar IoTForge Agent v2.2.2](https://drive.google.com/drive/folders/1D6iGh9kR7_1XgTj5N-XMpyfhTTdOjZPx?usp=drive_link)**

Descarga todos los archivos y colócalos en la misma carpeta.

---

## ¿Qué hace?

El agente corre en tu PC con Windows y permite compilar sketches de Arduino/ESP32 localmente, sin necesidad de subir tu código a la nube. IoTForge lo detecta automáticamente y lo usa para compilar y flashear tu dispositivo.

## Requisitos

- Windows 10 / 11 (64-bit)
- Cuenta activa en [iotforge.iaintegracion.space](https://iotforge.iaintegracion.space)
- Puerto USB disponible para tu dispositivo (ESP32, etc.)

## Instalación

1. Descarga todos los archivos desde el link de arriba
2. Colócalos en una carpeta, por ejemplo `C:\IoTForgeAgent\`
3. **Todos los archivos deben estar en la misma carpeta** — no mover ni borrar ninguno
4. Ejecuta `IoTForgeAgent.exe`
5. En IoTForge → Settings → Agente, ingresa el token que aparece en el agente
6. Listo — el agente aparecerá como conectado en tu dashboard

## Archivos incluidos

| Archivo | Descripción |
|---|---|
| `IoTForgeAgent.exe` | Agente principal |
| `esptool.exe` | Herramienta de flash para ESP32 |
| `avrdude.exe` + `avrdude.conf` | Herramienta de flash para AVR |
| `dfu-util.exe` | Herramienta de flash DFU |
| `libusb-1.0.dll` | Dependencia USB requerida por dfu-util |
| `IoTForgeCloud.h` | Librería de IoTForge para tus sketches |

## Actualización automática

El agente se actualiza solo. Cuando hay una nueva versión disponible, la descarga y aplica al reiniciar — no necesitas volver a descargar manualmente.

## Placas soportadas

- ESP32 / ESP32-S3 / ESP32-C3 / ESP32-C6 / ESP32-H2 / ESP32-S2
- Placas AVR compatibles con avrdude

## Soporte

- Plataforma: [iotforge.iaintegracion.space](https://iotforge.iaintegracion.space)
- Versión del agente: `v2.2.2`
