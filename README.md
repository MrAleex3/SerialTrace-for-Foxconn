# SerialInsight

**SerialInsight** es una herramienta interna desarrollada para gestionar archivos de log para equipos funcionales mediante su número de serie. Automatiza la búsqueda de resultados de prueba y permite generar archivos finales de tipo `PASS` o `FAIL` según la información seleccionada del historial.

## 🚀 Funcionalidades

- 🔎 Búsqueda de seriales dentro de archivos log desde una interfaz gráfica.
- 📄 Muestra los últimos 5 resultados de cada serial.
- ✅ Permite confirmar y generar un archivo limpio con estado `PASS` o `FAIL` .
- ❌ También permite marcar como `FAIL`, incluyendo manejo especial para equipos en modo `DEBUG`.
- 🔁 Conexión y subida automática del archivo final a un servidor de destino definido.
- 🔒 Interfaz protegida contra errores comunes (serial vacío, modelo inválido, archivos inexistentes).
- 🎨 Incluye una interfaz limpia y organizada para el usuario.

## 📷 Interfaz

![image](https://github.com/user-attachments/assets/7b650fae-5792-4395-806f-b033e7ba2c9d)



## 🧰 Requisitos

- Windows 10 o superior.
- Acceso a las rutas de red establecidas en `modelo.ini`.

## 🗂️ Estructura

- `modelo.ini`: Contiene los modelos y sus rutas de entrada y salida.
- `SerialTraceFox.ahk`: Script principal de la herramienta.
- `temporal/`: Carpeta temporal generada automáticamente para manejar los archivos intermedios.

## 📝 Licencia

Este proyecto está bajo la [Licencia MIT](LICENSE).

## 🙋 Autor

**Jose Alejandro**  
Foxconn México · Proyecto personal para portafolio
