# 🛡️ Automatizador de Auditoría y Sanitización de Inventario IT

## 📝 Descripción del Proyecto
Este proyecto es un script de Python diseñado para entornos de **Ciberseguridad y Cloud Computing**. Actúa como un pipeline de ETL (Extract, Transform, Load) que procesa, limpia y valida archivos de inventario de servidores generados automáticamente, los cuales suelen contener formatos irregulares o datos corruptos.

Garantizar que los datos del inventario (Asset Management) sean correctos es el primer paso crítico para cualquier auditoría de seguridad o despliegue de infraestructura automatizada (IaC).

## 🚀 Características Principales (Features)
* **Extracción y Normalización:** Procesa archivos de texto plano línea a línea, unificando separadores inconsistentes (`,` o `;`) y eliminando espacios residuales.
* **Manejo de Excepciones:** El script está protegido contra fallos de lectura (ej. archivo no encontrado) mediante bloques `try-except`.
* **Validación de Integridad:** * Comprueba que los campos obligatorios (como el nombre del servidor) no estén vacíos.
  * Valida estrictamente el formato de las **direcciones IPv4**.
  * Asegura que los sistemas operativos pertenezcan a una lista blanca (Linux, Windows, MacOS).
* **Generación de Reportes:** Exporta los datos validados y genera un archivo de auditoría (`informe_servidores.txt`) detallando las métricas de éxito, los errores encontrados y las IPs únicas.

## 🛠️ Tecnologías y Conceptos Utilizados
* **Lenguaje:** Python 3
* **Estructuras de datos:** Diccionarios, Listas y Sets.
* **Conceptos:** File I/O, Data Cleansing, Algoritmos de validación, Modularidad (Funciones).

## ⚙️ Cómo ejecutar el proyecto
1. Clona este repositorio en tu máquina local:
   ```bash
   git clone [https://github.com/4rmest0/Auditoria-Inventario-Python.git](https://github.com/TU_USUARIO/TU_REPOSITORIO.git)
