# SerialTrace

Herramienta desarrollada en AutoHotkey para gestionar archivos de log de equipos funcionales mediante su número de serie. Automatiza la búsqueda de resultados de prueba y permite generar los archivos finales `PASS` o `FAIL` según la información seleccionada del historial.

![AutoHotkey](https://img.shields.io/badge/AutoHotkey-1.1-blue)
![Windows](https://img.shields.io/badge/Platform-Windows-blue)
![Status](https://img.shields.io/badge/Status-Production-success)

- [Interfaz y funcionalidades](Funcionalidades.md)
- [Versión siguiente (SerialInsight 2.0)](https://github.com/MrAleex3/SerialInsight-2.0)

![Vista principal](https://github.com/user-attachments/assets/2b5612e1-fe9e-4ade-8f5e-57e615b2b18b)

## Origen del proyecto

Primera versión de SerialInsight, desarrollada como script de AutoHotkey antes de migrar a la aplicación web. Conserva la misma lógica de búsqueda de logs y generación de resultados PASS/FAIL que se retomó en la versión 2.0.

## Puesta en marcha

**Requisitos**

- Windows 10 o superior.
- AutoHotkey v1.1 instalado.
- Acceso a las rutas de red definidas en `modelo.ini`.

**Estructura**

- `modelo.ini`: contiene los modelos y sus rutas de entrada y salida.
- `temporal/`: carpeta temporal que se genera automáticamente para los archivos intermedios.

## Características

- Modo dual: búsqueda en 2 servidores.
- Lectura en tiempo real: identifica automáticamente el archivo de log más reciente en el servidor remoto.
- Historial extendido (PPID+): rastrea un PPID específico en logs de hace 7 hasta 30 días.
- Análisis multiarchivo sobre varios logs históricos según patrones de fecha.
- Generación de resultados FAIL y PASS, con carga del log actualizado al servidor.
- Manejo de System ID en equipos de depuración.
- Registro de cada acción crítica en un servidor central de auditoría.
- Gestión de red: conexión y desconexión automática de unidades de red.

## Licencia

Este proyecto está bajo la Licencia MIT.

## Autor

Alejandro Espinoza
Foxconn México
