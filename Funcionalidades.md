# Interfaz y funcionalidades

---

## Interfaz

Vista principal con la búsqueda por número de serie y el historial de resultados.

<p align="center">
  <img src="https://github.com/user-attachments/assets/2b5612e1-fe9e-4ade-8f5e-57e615b2b18b" alt="Interfaz" />
</p>

---

## Detalle de resultados

Lista ordenada con el System ID, la hora, el status, la prueba y el resultado de cada registro.

<p align="center">
  <img src="https://github.com/user-attachments/assets/e384bd69-781b-4312-8e2a-7ca28dd41c32" alt="Detalle de resultados" />
</p>

---

## Búsqueda de logs

- Modo dual: búsqueda en 2 servidores.
- Identificación automática del archivo más reciente en el servidor remoto.
- Análisis de varios logs históricos para encontrar todas las ocurrencias de una unidad.

---

## Gestión de debug y validaciones PASS/FAIL

- Con doble clic en un resultado se habilitan las acciones administrativas.
- Generar FAIL: fuerza el fallo de una unidad y sube el log actualizado al servidor de prueba.
- Generar PASS: da el pase a una unidad.
- Detecta IDs de depuración y solicita el ID correcto antes de procesar el log.

---

## Auditoría y seguridad

Cada acción crítica queda registrada con fecha y hora, usuario de Windows, nombre del equipo, PPID y System ID original y modificado.

---
<p align="center">
  <a href="README.md">Volver al README principal</a>
</p>
