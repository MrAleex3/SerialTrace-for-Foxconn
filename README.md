# SerialTrace

Herramienta desarrollada en AutoHotkey para gestionar archivos de log de equipos funcionales mediante su número de serie. Automatiza la búsqueda de resultados de prueba y permite generar los archivos finales `PASS` o `FAIL` según la información seleccionada del historial.

![Interfaz](https://github.com/user-attachments/assets/2b5612e1-fe9e-4ade-8f5e-57e615b2b18b)

![Detalle de resultados](https://github.com/user-attachments/assets/e384bd69-781b-4312-8e2a-7ca28dd41c32)

## Características

### Búsqueda de logs

- Modo dual: soporte para búsqueda en 2 servidores.
- Lectura en tiempo real: identifica automáticamente el archivo de log más reciente en el servidor remoto y filtra la información relevante.
- Visualización de System ID, hora, status, prueba y resultado en una lista ordenada.

### Historial extendido (PPID+)

- Búsqueda profunda: rastrea un PPID específico en logs de hace 7 hasta 30 días.
- Análisis multiarchivo: opera sobre varios logs históricos según patrones de fecha para encontrar todas las ocurrencias de una unidad.

### Gestión de debug y validaciones (PASS/FAIL)

- Interacción directa: con doble clic en un resultado se habilitan las acciones administrativas.
- Inyección de resultados:
  - Generar FAIL: fuerza el fallo de una unidad y sube el log actualizado al servidor de prueba.
  - Generar PASS: da el pase a una unidad.
- Manejo de System ID (debug): detecta automáticamente IDs de depuración, como `DBG-001`, y solicita al usuario el ID correcto antes de procesar el log.

### Auditoría y seguridad

- Registro de eventos: cada acción crítica, generar PASS o FAIL, queda registrada en un servidor central de auditoría con fecha y hora, usuario de Windows y nombre del equipo, PPID y System ID original y modificado.
- Gestión de red: conexión y desconexión automática de unidades de red para evitar bloqueos o conexiones persistentes.

## Requisitos

- Windows 10 o superior.
- Acceso a las rutas de red definidas en `modelo.ini`.

## Estructura

- `modelo.ini`: contiene los modelos y sus rutas de entrada y salida.
- `temporal/`: carpeta temporal que se genera automáticamente para los archivos intermedios.

## Licencia

Este proyecto está bajo la Licencia MIT.

## Autor

Alejandro Espinoza
Foxconn México
