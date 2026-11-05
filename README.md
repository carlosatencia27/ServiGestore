# Gestión de Trámites de Tránsito (MVP)

Prototipo (Producto Mínimo Viable) de una aplicación de escritorio para Windows que permite registrar
licencias (expedición inicial y refrendación), trámites vehiculares, seguros y revisiones tecnomecánicas,
calcular automáticamente sus vencimientos y mostrar los documentos vencidos o próximos a vencer.

Desarrollado por **Carlos Daniel Atencia García** como parte de la práctica profesional de Ingeniería de Software
de la Corporación Universitaria Iberoamericana, en SERVI Gestores del Cesar (BARCAB SAS).

> Proyecto académico en desarrollo. Este repositorio **no contiene datos reales** de clientes ni de la empresa.

## Contenido

- `GestionTransito/`: código fuente, manual (`LEEME.txt`), pruebas y scripts de ejecución.
- `docs/Informe_Avance_MVP_Carlos_Atencia.pdf`: informe de avance de la Actividad 3 (requisitos, características
  priorizadas, wireframes y documentación técnica en los anexos).

## Tecnologías

Python 3, CustomTkinter, SQLite, Pillow y PyInstaller. Pruebas con `unittest`.

## Cómo ejecutarlo (Windows)

1. Instalar Python 3 (marcando «Add python.exe to PATH»).
2. Entrar a la carpeta `GestionTransito` y hacer doble clic en `ejecutar.bat`, o desde una terminal:

```
py -m pip install customtkinter pillow
py main.py
```

3. Para cargar datos **ficticios** de demostración (solo en una carpeta de prueba): `py cargar_datos_ficticios.py`.
4. Para ejecutar las pruebas: `python -m unittest pruebas.test_logica`.
5. Para generar un ejecutable: `construir_exe.bat`.

## Estado

- Pruebas unitarias de la lógica: 12 de 12 satisfactorias (28 de octubre de 2026).
- Pendiente: pruebas de usuario (UAT) con el asesor interno, validación de las reglas de vigencia, control de
  calidad y seguridad (protección de datos personales).
