# Nombre del Proyecto #
Evaluación_FO
# Descripción
Este proyecto es una aplicación Android que implementa medidas de seguridad para proteger contra vulnerabilidades comunes. Se identificaron varios riesgos de seguridad durante el análisis y se implementaron mejoras para mitigarlos.
## Vulnerabilidades Identificadas
- Inyección SQL: No detectada, pero es una vulnerabilidad común a considerar.
- Comunicación no segura: Se detectó uso de permisos como INTERNET, pero no hay indicación de comunicaciones HTTPS.
- Exposición de datos sensibles: allowBackup=true y debuggable=true estaban habilitados, lo que podría exponer datos a través de copias de seguridad y depuración.
## Mejoras Implementadas
- Cifrado de datos sensibles: Se recomienda aplicar cifrado para la protección de datos sensibles debido a la configuración allowBackup=true.
- Comunicación segura (HTTPS): Actualmente, no se observó uso de HTTPS; implementar TLS/SSL es necesario.
- Validación y sanitización de entradas: Se debe asegurar que se saniticen todas las entradas de los usuarios para prevenir inyecciones.
## Cómo Ejecutar la Aplicación de Forma Segura
1. Clonar el repositorio
2. Importar el proyecto en Android Studio
3. Ejecutar la aplicación en un dispositivo o emulador
4. Asegurarse de que los permisos necesarios están configurados
## Reporte de Vulnerabilidades El reporte detallado de las pruebas de vulnerabilidad
realizadas se encuentra en el archivo `vulnerability_report.pdf`.

