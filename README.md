# SerialInsight

**SerialInsight** es una herramienta interna desarrollada para gestionar archivos de log para equipos funcionales mediante su numero de serie. Automatiza la busqueda de resultados de prueba y permite generar archivos finales de tipo `PASS` o `FAIL` segun la informacion seleccionada del historial.

## 🚀 Funcionalidades

### 1. Busqueda Inteligente de Logs
- **Modo Dual:** Soporte para busqueda en 2 servidores.
- **Lectura en Tiempo Real:** Identifica automaticamente el archivo de log mas reciente en el servidor remoto y filtra la informacion relevante.
- **Visualizacion Clara:** Muestra los datos como el `System ID`, `Hora`, `Status`, `Prueba` y `Resultado` en una lista ordenada.

### 2. Historial Extendido (PPID+)
- **Busqueda Profunda:** Capacidad de rastrear un PPID especifico en logs de **hace 7 días o hasta 30 días**.
- **Analisis Multi-archivo:** La app opera sobre multiples archivos de logs historicos basados en patrones de fecha para encontrar todas las ocurrencias de una unidad.

### 3. Gestion de Debug y Validaciones (PASS/FAIL)
- **Interaccion Directa:** Al hacer doble clic en un resultado, se habilitan acciones administrativas.
- **Inyeccion de Resultados:**
  - **Generar FAIL:** Permite forzar el fallo de una unidad y subir el log actualizado al servidor de prueba.
  - **Generar PASS:** Permite dar el pase a una unidad.
- **Manejo de System ID (Debug):** Detecta automaticamente IDs de depuracion (como `DBG-001`) y solicita al usuario el ID correcto antes de procesar el log, asegurando la integridad de los datos.

### 4. Auditoría y Seguridad
- **Logging de Eventos:** Cada accion critica (generar un Pass o Fail) queda registrada en un servidor central de auditoría con:
  - Fecha y Hora.
  - Usuario de Windows y Nombre del Equipo.
  - PPID y System ID original/modificado.
- **Gestion de Red:** Conexion y desconexion automatica de unidades de red para evitar bloqueos o conexiones persistentes inseguras.

## 📷 Interfaz

<img width="702" height="387" alt="image" src="https://github.com/user-attachments/assets/cb71bf0b-e552-47db-ac77-2c32e6d82e00" />

<img width="812" height="382" alt="image" src="https://github.com/user-attachments/assets/e384bd69-781b-4312-8e2a-7ca28dd41c32" />





## 🧰 Requisitos

- Windows 10 o superior.
- Acceso a las rutas de red establecidas en `modelo.ini`.

## 🗂️ Estructura

- `modelo.ini`: Contiene los modelos y sus rutas de entrada y salida.
- `temporal/`: Carpeta temporal generada automaticamente para manejar los archivos intermedios.

## 📝 Licencia

Este proyecto esta bajo la [Licencia MIT](LICENSE).

## 🙋 Autor

**Jose Alejandro**  
Foxconn México · Proyecto personal para portafolio
